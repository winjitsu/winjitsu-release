# Acknowledgments & Third-Party Attributions

Winjitsu incorporates patterns, algorithms, and private API research from several outstanding open-source macOS projects. We are grateful for the contributions of these communities.

## Technical Attributions

### 1. Hammerspoon

- **Source:** [Hammerspoon/hammerspoon](https://github.com/Hammerspoon/hammerspoon)
- **Ported Logic:** Window focus orchestration sequence (AXRaise -> AXMain -> Carbon Process Activation).
- **Workarounds:** Finder desktop focus workaround (300ms timer pattern).
- **Files:** `WindowManipulator.swift`, `CarbonBridge.m`
- **License:** MIT
- **Copyright:** Copyright (c) 2014-2025 Hammerspoon contributors.

### 2. Yabai

- **Source:** [koekeishiya/yabai](https://github.com/koekeishiya/yabai)
- **Technical Research:** Mapping of private SkyLight (SLS) event numbers (e.g., window move/resize/creation) and the functional pattern of the SLS window metadata iterator chain.
- **Ported Logic:** Connection-context event routing pattern.
- **Files:** `SLSBindings.h`, `SLSEventListener.swift`, `SLSWindowQuery.swift`
- **License:** MIT
- **Copyright:** Copyright (c) 2019–2025 Nikita Bobko (koekeishiya).

---

## Implementation Rationale & Heuristics

The following technical patterns represent "Industry Best Practices" for robust macOS window management. Winjitsu utilizes these heuristics as functional necessities:

### **1. Mission Control Tracking (The "Dock Observer" Pattern)**

- **Problem:** macOS provides no public API to detect when the user enters or exits Mission Control or App Exposé.
- **Solution:** The macOS Dock process (`com.apple.dock`) emits undocumented Accessibility notifications (`AXExposeShowAllWindows`, etc.). Observing the Dock process is the only reliable way for third-party tools to synchronize their UI (like borders) with system-level spatial transitions.

### **2. Focus Stealing (The "Carbon Activation" Hack)**

- **Problem:** Modern AppKit `activate()` calls are often ignored by macOS if another app has taken focus recently (to prevent focus stealing).
- **Solution:** Utilizing the legacy Carbon API `SetFrontProcessWithOptions` provides a more authoritative signal to the Window Server, ensuring that focus transitions are snappy and predictable.

### **3. Display Stability (The "Finder Workaround")**

- **Problem:** Rapid focus switching or space changes can cause macOS to "bounce" focus back to the desktop or the Finder, especially if no window is active on the target space.
- **Solution:** A short delay (300ms) before final activation ensures the Window Server has stabilized its internal space-state before the focus operation is committed.

---

For full license text, please refer to the [THIRD-PARTY-LICENSES.md](https://github.com/winjitsu/winjitsu-release/blob/main/THIRD-PARTY-LICENSES.md) file.
