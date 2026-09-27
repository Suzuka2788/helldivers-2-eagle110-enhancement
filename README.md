# Suzuka‘s Eagle 110mm enhancement v2.3.1

Enhances Eagle 110mm Rocket Pods with 12 rockets per attack: six from each pod, a 4-second firing window, and a 0.33-second salvo interval.

## Settings

HD2 Arsenal provides **2, 3, 4, or 5 base uses per rearm**. The default is **3**. This is the use count before ship upgrades; the game's additional-use upgrade is left to the game.

## Installation

Requires **Bingus Shared Loader v15 or newer / API 1**. Close the game, replace the previous Eagle 110mm enhancement package, choose the base-use option in HD2 Arsenal, confirm, deploy, and restart. Do not enable multiple versions together.

## Compatibility and verification

Targets game.dll SHA-256 `2e2c3b7c2500646dadd5f2b4c6e0504dbb7e7896139f64cddc0d1813c718f51e`. Other DLL versions are disabled without writing. Complete component mappings and target records were checked read-only against this game version. A previous package produced all four successful runtime-write statuses; the renamed package and all four choices passed package, Lua syntax, and offline behavior tests. The renamed package and ship-upgrade stacking have not been separately confirmed in game.

The mod validates records before writing and reads values back afterward. If a policy fails, it attempts to restore changes it owns and reports whether restoration was confirmed.

Log: `%LOCALAPPDATA%\CowboyBingus\Helldivers2\Logs\SuzukaEagle110Boost.log`. Successful application reports `STATUS=APPLIED_ALL`. At the default 3-use setting, the use-count field needs no write; the rocket enhancements still apply.

Game updates require renewed verification. This release does not guarantee compatibility with future updates.

## Credits

Uses [Bingus Shared Loader](https://github.com/CowboyBingus/BingusSharedLoader) and field reference data extracted with [FileDiver](https://github.com/xypwn/filediver).
