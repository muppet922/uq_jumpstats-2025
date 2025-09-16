# JumpStats Plugin Counter-Strike 1.6 2025 (uq.sma)

## Overview
This is a Counter-Strike 1.6 AMXX plugin for advanced jump statistics, originally by kzuq^BorJomi (version 2.42). It provides detailed stats and HUD feedback for various jump types (LongJump, CountJump, Double CountJump, LadderJump, Bhop, etc.), helping players improve their movement skills. The plugin is inspired by kz_ljs_xm and Exolent's work.

## Features
- Tracks and displays stats for many jump types: LJ, CJ, DCJ, MCJ, Ladder, Bhop, DropBhop, and more
- HUD and chat output for jump distance, prestrafe, speed, sync, and other metrics
- Customizable thresholds for jump ranks (good, pro, holy, leet, god)
- SQL and web stats support
- Admin commands for stats reset and configuration
- Menu and chat commands for toggling features
- Extensive cvar configuration for colors, HUD positions, and more

## Requirements
- **AMX Mod X**
- **Counter-Strike 1.6 server**
- The following includes from the [Kreedz repository](https://github.com/Theggv/Kreedz/) are required:
  - `kreedz_api.inc`
  - `settings_api.inc`
  - `uq_jumpstats_const.inc`
  - `uq_jumpstats_stocks.inc`

Place these `.inc` files in your `amxmodx/scripting/include/` directory.

## Installation
1. Download and place `uq.sma` in your `amxmodx/scripting/` folder.
2. Make sure you have the required `.inc` files from the [Kreedz repository](https://github.com/Theggv/Kreedz/) in your `include` folder.
3. Compile `uq.sma` using the AMXX compiler.
4. Place the resulting `uq.amxx` in your `amxmodx/plugins/` folder.
5. Add `uq.amxx` to your `amxmodx/configs/plugins.ini`.
6. Restart your server.

## Usage
- Players can use chat commands like `/ljstats`, `/strafe`, `/showpre`, `/duck`, `/speed`, `/edge`, `/jof`, etc. to toggle and view various stats.
- Admins can use `amx_reset_uqtops` to reset all tops.
- All cvars are prefixed with `kz_uq_` for customization (see source for full list).

## Output Example
When a player performs a jump, the plugin displays:
- Jump type (e.g., LongJump, CountJump)
- Distance jumped
- Prestrafe speed
- Sync percentage
- Number of strafes
- HUD color feedback based on performance

Example HUD output:
```
[TAG] LJ: 245.12 units | Pre: 276.44 | Sync: 85% | Strafes: 7
```

## Credits
- kzuq^BorJomi (author)
- Developers of kz_ljs_xm and Exolent
- [unique-kz.com](http://unique-kz.com/)

## License
This plugin is provided as-is. See the original repository for license details.
