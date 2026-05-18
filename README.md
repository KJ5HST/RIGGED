<p align="center">
  <picture>
    <source media="(prefers-color-scheme: light)" srcset="assets/logo-light.png">
    <img alt="Rigged" src="assets/logo-dark.png" width="640">
  </picture>
</p>

<p align="center"><strong>One window. Every radio.</strong></p>

<p align="center"><em>Pre-release. Demoed at Hamvention 2026.</em></p>

---

This is where ham radio software stops being eight programs in a trench coat. Rigged runs FT8, CW, the keyer, interfaces to logbooks, manages the audio path, the works — one window, any OS, any radio that Hamlib supports. One copy of Hamlib for all features. No tabbing between four apps to make one QSO. No port conflicts.

This page is informational. The app is a proof of concept, and I'm seeking input from the public. Check out the YouTube videos for demonstrations:

## Videos

- [Life At Terminal Velocity](https://youtu.be/MazhoI204Zk)

Contact me at KJ5HST@Deppe.com if you want me to demonstrate for your club, or do a live stream.

---

## What works today

###Drag-and-drop UI
 - Any number of workspaces with any number of profiles with any number of views
 - Every panel drops onto any view.
 - Rename, duplicate, delete, build your own.
 - Export/Import to share your setup with your friends or install on another computer.

###Native FTX-1 driver
- Hamlib not required
- 91 CAT commands
- 17 operating modes
- every menu setting
- Hardware-verified on Field and Optima configurations

###Native digital modes
- FT8
- FT4
- JT65
- WSPR

###Remote control
- Same app, different location
- Self discovery
- Audio over TCP -- server, client, or both

###Cross-platform
- Mac
- Windows
- Linux 
- Web client available in any modern browser

###Nine languages
- English
- German
- French
- Spanish
- Italian
- Japanese
- Russian
- Hebrew
- Arabic (with RTL).

---

## What we just shipped

Last thirty days, structural — boring but necessary:

- Auto-discovery works on machines with multiple network interfaces. USB-tethered iPhone alongside Wi-Fi no longer confuses the discovery beacon.
- Audio recordings save to the right place under user data, regardless of where the app was started from.
- More reliable remote sessions — closed a couple of subsystem gaps that only surfaced under real-world remote demos.

Currently in a feature freeze for a post-Hamvention cleanup sprint. No new features until the rough edges above are green.

---

## What's coming next

**Asked for at Hamvention 2026:**

- **JS8 Call** integration for HF text and APRS-style messaging.
- **iOS and Android** clients for grid-down EmComm — tablets and phones outlast laptops on battery.
- **Mac App Store** distribution alongside direct download.
- **A real landing page** and an early-access list (you found it, and list started)

**Longer horizon:**

- Multi-manufacturer native drivers. The architecture was built for it; Icom and Kenwood are next candidates.
- Winlink RMS hosting.
- White-label OEM builds for radio manufacturers.

---

## Not yet

No install, no signup, no buy button — not yet. This page is a snapshot of where the work is right now. Overwhelming positive feedback at Hamvention and in video comments are a green light to continue development.

Watch this repo for updates.

---

<sub>Copyright 2024–2026 Terrell Deppe (KJ5HST). All rights reserved. Source private.</sub>
