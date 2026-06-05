# NuclearMapPlayerNames

Client-side Nuclear Option mod that shows multiplayer usernames next to player-controlled aircraft on the dynamic map.

## Install

The easiest way to install and update this mod is with **NOMM**, the Nuclear Option Mod Manager:

- NOMM: https://github.com/Combat787/NOMM
- Latest NOMM download: https://github.com/Combat787/NOMM/releases/latest

You can also install manually from this repository's Releases page. Download the latest `NuclearMapPlayerNames-v*.zip` archive and extract it into your Nuclear Option `BepInEx/plugins/` folder. The archive already contains the plugin folder layout.

## About this repository

This GitHub repository is a release mirror for NOMNOM/NOMM automatic updates. The canonical source code and development history live in the Forgejo monorepo:

- Source: https://forge.dikka.dev/lab/nuclear_option_mods

## Metadata

- NOMNOM id: `dev.dikka.nuclearmapplayernames`
- Author: dikkadev
- Tags: QoL, Map, Multiplayer
- Release asset format: one `.zip` per release

## Details

`NuclearMapPlayerNames` is a client-side `Nuclear Option` BepInEx mod that shows multiplayer usernames next to player-controlled aircraft on the dynamic map.

The stock game already shows a player's username in the hover tooltip. This mod keeps that behavior but adds always-visible map labels so you do not have to hover over every aircraft to identify real players.

## Features

- Shows usernames next to real/player-controlled aircraft on the dynamic map
- Ignores AI aircraft and unoccupied aircraft
- Config toggle to restore stock hover-only behavior
- Optional setting to show labels only when the map is maximized
- Configurable rendered font size, visual text scale, and label offset
- Option to hide your own aircraft label, enabled by default

## Requirements

- `Nuclear Option`
- `BepInEx 5`

## Installation

1. Install BepInEx for `Nuclear Option`.
2. Build the mod or download a release archive.
3. Extract the `NuclearMapPlayerNames` folder into `BepInEx/plugins/`.

The final layout should look like this:

```text
BepInEx/
  plugins/
    NuclearMapPlayerNames/
      NuclearMapPlayerNames.dll
```

## Configuration

Config entries are created automatically after the mod loads.

Main config file:

- `BepInEx/config/dev.dikka.nuclearmapplayernames.cfg`

Important settings:

```ini
[Map Player Names]
## Show multiplayer usernames next to player-controlled aircraft on the dynamic map.
Show Player Names = true

## Only show player names when the dynamic map is maximized.
Show Only On Maximized Map = false

Hide Local Player Name = true
Font Size = 12
Text Scale = 0.6
Offset X = 2
Offset Y = 4
```

