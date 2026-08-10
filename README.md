# Winjitsu

### Keyboard-first window control for macOS.

Command your workspace at the speed of thought—whether your windows are neatly arranged or organically overlapping.

[**Download Latest Release**](https://github.com/winjitsu/winjitsu-release/releases/latest/download/Winjitsu-Installer.pkg) | [**Official Website**](https://winjitsu.app) | [**Privacy Policy**](https://winjitsu.app/privacy)

---

## Is Winjitsu Open Source?

**No. Winjitsu is proprietary software.** 

This repository serves as our public distribution hub to publish official pre-built binary releases (`.pkg`), host documentation, and maintain public attributions for the open-source projects that inspired or informed our technical research. 

- The desktop application binaries published here are **free to download and use**.
- We offer a **Free Forever (Core)** tier alongside a **Pro** upgrade.

---

## Philosophy: Canvas, Not a Cage

Most macOS window management tools force a binary choice:

1. **The Chaos:** Free-floating windows you hunt through with mouse clicks and endless `Cmd+Tab` cycling.
2. **The Cage:** Rigid tiling window managers that fight macOS, locking everything into a rigid grid.

**Winjitsu introduces a different paradigm.**

We treat your desktop as a **freeform canvas**, not a spreadsheet. Winjitsu provides spatial order without restriction, giving you keyboard efficiency without fighting native macOS behaviors or forcing your windows into rigid constraints.

---

## Key Features

- **Directional Window Focus (HJKL):** Move focus spatially in the direction you mean—even across overlapping, stacked, or irregular window layouts.
- **Focus Preview Borders (Pro):** An active visual outline shows you exactly where focus will land before you commit.
- **Window Stack & Container Cycling:** Fully stack windows on top of each other and flip through them fluidly in place like a deck of cards.
- **Mission Control Keyboard Navigation:** Search, select, close windows, or force-quit apps directly in Mission Control—100% keyboard driven.
- **Space-to-Space Window Moving (Pro):** Move windows directly to any of your macOS Desktops without dragging.
- **Edge-Specific Resizing (Pro):** Independently grow or shrink any single window edge (left, right, top, bottom) instead of just snapping.
- **Native Harmony:** Works seamlessly with macOS Spaces, Mission Control, and Stage Manager—no SIP modification required.

---

## Licensing & Pricing

Winjitsu is available in two tiers:

| Feature Tier | Price | Licensing Terms |
| :--- | :--- | :--- |
| **Winjitsu (Core)** | **$0 (Free Forever)** | Essential spatial navigation (HJKL), basic stack cycling, standard grid snapping, and 100% local privacy. Free forever with no account or payment info required. |
| **Winjitsu Pro** | **$19 USD (One-Time)** | Unlocks Focus Preview Borders, interactive Mission Control actions (close/quit), Desktop Space tossing, edge-specific resizing, snap history undo, and custom snap sequences. Lifetime license for 1 Mac + free 1.x updates. |

> **30-Day Pro Trial:** Every new download includes a **full 30-day trial of all Pro features**—no credit card, email, or account required. After 30 days, Pro features gracefully lock, while **Core features remain free forever**.

---

## Privacy & Local-First Design

Winjitsu is built with an **offline-first, private-by-default architecture**. Because macOS window control requires Accessibility permissions, Winjitsu is designed so that your window titles, contents, and keystrokes **never leave your Mac**. There is nothing to opt out of—there is no telemetry or behavioral tracking collected in the first place.

### What Stays Local:
- Window titles, contents, and application geometry
- Document names and file contents
- Keystrokes, mouse activity, and clipboard data
- Screenshots and screen recordings

### Network Activity:
Winjitsu operates primarily offline. Network calls are limited strictly to:
1. **License Validation (Pro):** A periodic check (approx. every 30 days) transmitting only an encrypted license token and a pseudonymous machine ID.
2. **Software Updates:** Optional background version checks via the Sparkle framework (can be toggled in Settings).
3. **Optional Diagnostic Reports:** Only generated and sent if you explicitly initiate a support ticket.

Read the complete policy at [winjitsu.app/privacy](https://winjitsu.app/privacy).

---

## Installation

1. Download the latest [`Winjitsu-Installer.pkg`](https://github.com/winjitsu/winjitsu-release/releases/latest/download/Winjitsu-Installer.pkg).
2. Open the package and follow the standard macOS installation wizard.
3. Upon first launch, grant **Accessibility** permissions when prompted by macOS (`System Settings > Privacy & Security > Accessibility`).

---

## Credits & Attributions

Winjitsu stands on the shoulders of the macOS developer community. We extend our deep gratitude to:

- **[Hammerspoon](https://github.com/Hammerspoon/hammerspoon):** Our original laboratory for prototyping spatial window orchestration and Carbon process activation heuristics.
- **[Yabai](https://github.com/koekeishiya/yabai) & [AeroSpace](https://github.com/nikitabobko/AeroSpace):** For pioneering SkyLight (SLS) window server research and pushing the boundaries of macOS window management.
- **[Rectangle](https://github.com/rxhanson/Rectangle):** For establishing clean standards in open-source window snapping.

For full license texts and detailed attribution breakdowns, see [ACKNOWLEDGMENTS.md](ACKNOWLEDGMENTS.md) and [THIRD-PARTY-LICENSES.md](THIRD-PARTY-LICENSES.md).

---

## Support & Links

- **Website:** [winjitsu.app](https://winjitsu.app)
- **General Inquiries:** [contact@winjitsu.app](mailto:contact@winjitsu.app)
- **Privacy Inquiries:** [privacy@winjitsu.app](mailto:privacy@winjitsu.app)

*Command your workspace at the speed of thought.*
