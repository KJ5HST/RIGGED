<p align="center">
  <picture>
    <source media="(prefers-color-scheme: light)" srcset="assets/logo-light.png">
    <img alt="Rigged" src="assets/logo-dark.png" width="640">
  </picture>
</p>

<p align="center"><strong>One window. Every mode. No WSJT-X.</strong></p>

<p align="center"><em>Pre-release. Demoed at Hamvention 2026.</em></p>

---

Ham radio software stops being eight programs in a trench coat. Rigged runs FT8, CW, the keyer, the logbook, the audio path, the works — one window, any OS, any radio your driver supports. No Hamlib config. No virtual audio cables. No tabbing between four apps to make one QSO.

This page is informational. There's no install yet.

---

## What it replaces

| You currently run | Rigged ships built in |
|---|---|
| WSJT-X / JTDX | Pure Java FT8, FT4, JT65, WSPR decoder (16 digital modes) |
| flrig / rigctld / Hamlib | Direct CAT control + Hamlib emulation for legacy apps |
| Log4OM / N1MM+ / Logger32 | QSO log with QRZ + LoTW upload |
| VAC / BlackHole / VB-Cable | Direct USB audio + TCP streaming |
| fldigi / Winlink | Built-in digital modes + Winlink P2P |
| Separate contest loggers | Contest profiles with rate tracking and dupe checking |

---

## What works today

- **Profiles and drag-and-drop UI.** Eleven profiles in the box — Digital, CW, POTA, Contest, DX, Ragchew, Emcomm, Net, Satellite, WSPR, Default. Three views per profile by default; rename, duplicate, delete, build your own. Every panel drops onto any view.
- **FTX-1 driver.** 91 CAT commands, 17 operating modes, every menu setting. Hardware-verified on Field, Optima, and SPA-1 heads.
- **Native digital modes.** FT8, FT4, JT65, WSPR decoded server-side, pure Java. Remote sessions don't break decode timing.
- **Local and remote, same app.** Audio over TCP. One installer, one flag — server, client, or both.
- **Hamlib bridge.** rigctld emulation keeps WSJT-X, fldigi, and the rest happy while you migrate.
- **Cross-platform.** Mac, Windows, Linux native packages, plus a web client in any modern browser.
- **Nine languages.** English, German, French, Spanish, Italian, Japanese, Russian, Hebrew, Arabic (with RTL).

---

## Rough edges we're chasing

- **Audio waterfall hiccups** — a roughly 1 Hz silence pattern during remote streaming.
- **Radio-connect plugin** auto-flips to RPC after a local disconnect; takes extra clicks to return to local.
- **Sidebar slow to sync** on Windows remote — the UI looks blocked until it catches up.
- **Winlink UI corners** — silent failure on a bad callsign, "sent" status while the message is still queued, a stale Retry button after a failed send, the outbox occasionally vanishing on a new compose, toasts that clear too fast, error banners with no reason text.
- **Daylight theme** — the primary button renders green-ish, not the cyan it should be.

---

## What we just shipped

Last thirty days, structural — boring but necessary:

- Fixed the long-standing "is it connected?" confusion. The sidebar, the plugins, and the backend all read the same connection state now, instead of three different ones disagreeing with each other.
- Auto-discovery works on machines with multiple network interfaces. USB-tethered iPhone alongside Wi-Fi no longer confuses the discovery beacon.
- The sidebar Reconnect button shows up when it should, on the platforms it should.
- Audio recordings save to the right place under user data, regardless of where the app was started from.
- More reliable remote sessions — closed a couple of subsystem gaps that only surfaced under real-world remote demos.

Currently in a feature freeze for a post-Hamvention cleanup sprint. No new features until the rough edges above are smoked green.

---

## What's coming next

**Asked for at Hamvention 2026:**

- **JS8 Call** integration for HF text and APRS-style messaging.
- **iOS and Android** clients for grid-down EmComm — tablets and phones outlast laptops on battery.
- **Public alpha** with mock CAT, so operators without an FTX-1 can evaluate the UX.
- **Mac App Store** distribution alongside direct download.
- **A real landing page** and an early-access list.

**Longer horizon:**

- Multi-manufacturer drivers. The architecture was built for it; Icom and Kenwood are next candidates.
- Winlink RMS hosting.
- White-label OEM builds for radio manufacturers.

---

## Not yet

No install, no signup, no buy button — not yet. This page is a snapshot of where the work is right now, posted while the brand and the website catch up to the software.

Watch this repo, or [follow KJ5HST on GitHub](https://github.com/KJ5HST), for updates.

---

<sub>Copyright 2024–2026 Terrell Deppe (KJ5HST). All rights reserved. Source private.</sub>
