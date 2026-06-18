# Winjitsu

### A keyboard-driven precision instrument for macOS.

**Winjitsu** is a workspace control instrument designed for users who think spatially and prefer to keep their hands on the keyboard. It treats your desktop as a freeform canvas, allowing you to navigate, move, and resize windows using intuitive, fully customizable keyboard shortcuts.

[**Download Latest Release**](https://github.com/winjitsu/winjitsu-release/releases/latest/download/Winjitsu-Installer.pkg) | [**Official Website**](https://winjitsu.app)

---

## The Philosophy

Terminal users developed a spatial keyboard-navigation model that never really existed on the desktop. Winjitsu is an attempt to bring that model to ordinary windows.

Most window managers force a binary choice:

1.  **The Chaos:** Free-floating windows you hunt through with clicks and endless alt-tabbing.
2.  **The Cage:** Rigid tiling systems that fight macOS, locking everything into a spreadsheet-like grid.

**Winjitsu provides a different paradigm.**
We believe your desktop is a **canvas**, not a spreadsheet. Winjitsu provides order without restriction, giving you keyboard efficiency without fighting the native behavior of macOS.

> _"It's not a terminal; it's not a grid; it's a desktop canvas that finally understands direction and layers."_

---

## Key Features

- **True Spatial Navigation:** Move focus in the direction you mean—even in overlapping, stacked, or irregular layouts.
- **Mission Control, Keyboard-First:** Navigate, close windows, and move them between Spaces without touching the mouse.
- **Visual Feedback:** Clear preview borders show you exactly where focus will land before it moves.
- **Stack Cycling:** Fully stack windows on top of each other and cycle through them fluidly.
- **Granular Window Shaping:** Resize one edge at a time, nudge precisely, and shape windows instead of just snapping them.
- **Native Harmony:** Designed to augment macOS, not replace it. Works seamlessly with Spaces, Mission Control, and Stage Manager.

---

## Privacy & The Technical Truth

Winjitsu is built with an **offline-first philosophy**. Because window managers require Accessibility permissions to function, we believe absolute transparency is the only way to build trust.

### Local-First Operation

All window management operations are performed locally on your Mac. Winjitsu does **not** use its permissions to transmit:

- Window titles or contents
- Document names or contents
- Screenshots or recordings
- Your keystrokes or clipboard
- Application activity logs

### Network Activity

Winjitsu operates primarily offline. It touches the internet for only three reasons:

1.  **License Validation (Pro):** A periodic check (approx. every 30 days) to confirm a Pro license is valid. This transmits only a cryptographic token and a pseudonymous machine ID.
2.  **Software Updates:** Using the Sparkle framework to check for newer versions (can be disabled in Settings).
3.  **Optional Diagnostic Reports:** Only sent if you explicitly choose to submit a support report. You have total control over generating, reviewing, and sending these reports.

For the exhaustive policy, visit [winjitsu.app/privacy](https://winjitsu.app/privacy).

---

## Installation

1.  Download the [Winjitsu-Installer.pkg](https://github.com/winjitsu/winjitsu-release/releases/latest/download/Winjitsu-Installer.pkg).
2.  Run the installer and follow the prompts.
3.  Upon first launch, macOS will prompt you to grant **Accessibility** permissions. This is required for Winjitsu to move and resize windows.

## Pricing

Winjitsu is available in two tiers:

- **Winjitsu (Core):** Basic spatial navigation and standard shortcuts. Free forever.
- **Winjitsu Pro:** Unlimited shortcuts, Mission Control navigation, advanced stack cycling, and visual feedback. One-time purchase.

_Every installation includes a 30-day trial of Pro features—no account or payment info required._

---

## Credits & Gratitude

Winjitsu wouldn't exist without the incredible work of the macOS utility community. A special thanks to [Hammerspoon](https://github.com/Hammerspoon/hammerspoon) for providing our original development laboratory, and to the developers of [Yabai](https://github.com/koekeishiya/yabai), [AeroSpace](https://github.com/nikitabobko/AeroSpace), [Rectangle](https://github.com/rxhanson/Rectangle), and others, for the inspiration and pushing the boundaries of what's possible on a Mac.

For the full list of attributions and verbatim license texts, see [ACKNOWLEDGMENTS.md](ACKNOWLEDGMENTS.md) and [THIRD-PARTY-LICENSES.md](THIRD-PARTY-LICENSES.md).

---

## Support & Community

- **Website:** [winjitsu.app](https://winjitsu.app)
- **Contact:** [contact@winjitsu.app](mailto:contact@winjitsu.app)
- **Privacy:** [privacy@winjitsu.app](mailto:privacy@winjitsu.app)

_Precision control for the spatial mind._
