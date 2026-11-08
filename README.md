# CSD Nano Dashes — V2, V3, V4

Racelogic-style SimHub dashboards for the **Conspit CSD Nano** (2.99", 800 × 268).

**By DIRTYNUT** · Free for personal use · Not open source — see [License](#license)

---

## Compatibility

| | |
|---|---|
| **Supported** | Conspit CSD Nano 2.99" (800 × 268), on any wheelbase |
| **Mounting** | Magnetic pogo-pin mount on Conspit ARES / ARES Platinum, or USB-C on other setups |
| **Not supported** | Conspit 310 APEX and 300GT wheel screens — same size, but their screens run Conspit Link's built-in dashes, not custom SimHub dashes |
| **Requires** | SimHub on a Windows PC |

## What's included

Three styles, each with three dashes — one per Nano — plus an Inputs screen.

| Style | Look |
|---|---|
| **V2 – Clean Racelogic** | Big bold numbers, color-coded sector panels. The segmented bar across the top of the lap screen shows lap distance traveled. |
| **V3 – Full Livery** | Slanted race-livery panels, 3D numbers, delta screen turns full green/red with chevrons. |
| **V4 – Hypercar Night** | Lap progress ring, precision delta bar, sector rows with live timing. |

| Screen | Shows |
|---|---|
| **Lap Time** | Current lap, lap number, best / last / predicted lap |
| **Delta** | Live delta to your best lap of the session |
| **Sectors** | Split times like the game, colored vs your best lap: purple = session best, green = faster, yellow = slower, light blue = the sector you're in |
| **Inputs** (V4 only) | Brake / throttle bars, 5-second input trace, ABS and TC lights, peak brake %, time to peak brake (vs your previous braking zone), wheel lock, FFB % and FFB clipping % for the lap |

### Sectors details

- **iRacing tracks with more than 3 sectors:** the panels show the two sectors before the one you're in plus the live one (e.g. S4 / S5 / S6 LIVE), and a thin strip along the bottom shows every sector of the lap.
- In iRacing each panel shows that sector's own time; in LMU and other sims they show split times like the game's timing screen.
- If you have the **Lovely plugin** installed (used by Lovely Dashboard), iRacing sector times come from it; otherwise the dash times the sectors itself.
- **Spotter view:** when a car is alongside, the Sectors screen switches to CAR LEFT / CAR RIGHT / 3 WIDE, then switches back half a second after the car clears.

### Inputs details

FFB and clipping: iRacing. Wheel lock: LMU / rFactor 2. Where a sim doesn't send that data, those boxes show `--`.

### Delta and timing

- **Le Mans Ultimate:** delta comes straight from the game's own telemetry, so it matches the in-game delta to 3 decimals.
- **iRacing:** uses iRacing's own delta to your session best.
- **Other sims:** SimHub's delta.
- Like the game, the delta starts after your first full timed lap.
- Timing shows **IN PITS** in the garage / pit lane and **OUT LAP** on the out lap, and starts when you cross the line.

---

## Download

**Latest: v2.14** — download `CSD_Nano_Dashes_v2.14.zip` from the [Releases page](../../releases/latest), then follow the install steps below.

---

## Install

### Step 1 — Install the dashes

1. Close SimHub completely (also right-click its icon in the system tray by the clock and choose **Exit**, if it's there).
2. Extract the zip, then copy the `Nano V...` folders into SimHub's DashTemplates folder:
   ```
   C:\Program Files (x86)\SimHub\DashTemplates\
   ```
   If you installed SimHub somewhere else, use `DashTemplates` inside that SimHub folder. If you're updating, choose **Replace the files**.

### Step 2 — Install the fonts (once)

The dashes use the **Barlow Condensed** font. Without it SimHub swaps in a default font and the layouts won't look right.

1. Open any of the dash folders, then its `_SHFonts` folder, e.g.
   ```
   DashTemplates\Nano V2 - Lap Time\_SHFonts
   ```
2. Select all six `.ttf` files (click one, then press **Ctrl+A**).
3. Right-click them and choose **Install for all users**.
   On Windows 11 you may need to click **Show more options** first.
   Use **Install for all users**, not just **Install** — SimHub may not see fonts that are installed for one user only.
4. Click **Yes** if Windows asks for permission.

All the dashes use the same fonts, so you only do this once.

Fonts included (in each `_SHFonts` folder): Barlow Condensed SemiBold, SemiBold Italic, ExtraBold, ExtraBold Italic, Black, Black Italic.

### Step 3 — Start SimHub and assign the dashes

1. Start SimHub. The dashes appear in Dash Studio under **CSD Nano**.
2. In SimHub's settings for each CSD Nano, pick one dash per screen (Lap Time / Delta / Sectors) from the version you like.

---

## Troubleshooting

- **Fonts look wrong:** redo Step 2 with **Install for all users**, then fully exit and restart SimHub.
- **Delta shows `-.---`:** normal until you've completed one timed lap after your out lap, same as in the game.
- **Spotter never shows:** it uses SimHub's spotter, which needs to be supported by the sim. It stays off while you're stopped (garage, pit box).
- **Something else looks off:** send a photo of the Nano along with which version and sim you're using.

---

## License

**Copyright © 2026 DIRTYNUT. All rights reserved.**

This is **not** open-source software. The dashboards are shared free of charge for personal use only. See [LICENSE.txt](LICENSE.txt) for the full terms. In short:

**You may**
- Download, install and use the dashboards on your own sim rig for personal, non-commercial use.
- Change settings or tweak the dashboards for your own private use on your own rig.
- Share a **link** to the original post or download page.

**You may not**
- Copy, re-upload, redistribute, mirror or share the files (original or modified) with anyone else.
- Sell, rent, license or charge for access to them in any way, including paid downloads, memberships, Patreon-style tiers, or bundling with any product, hardware or service.
- Publish or distribute modified versions, or anything derived from these files.
- Use the files, scripts, layouts or designs to make a competing or look-alike dashboard product, free or paid.
- Remove or change the license, copyright notice, or author credit.

### Third-party components

- The bundled **Barlow Condensed** fonts are **not** covered by this license. They are Copyright 2017 The Barlow Project Authors and licensed under the **SIL Open Font License 1.1** (see `OFL.txt` next to the fonts).
- SimHub, Conspit, CSD Nano, Le Mans Ultimate and other names are trademarks of their respective owners. These dashboards are an independent project and are not affiliated with or endorsed by them.

Provided "as is", without warranty of any kind. For any use not covered here, ask the author first.

**Owner: DIRTYNUT**
