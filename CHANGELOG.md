# Changelog

Dates are the release dates. Versions follow `major.minor.patch`; while
SceneKeys is at 0.x, anything may still change.

## 0.9.2 — 2026-09-22

Still stops changing keys on 30 November 2026, like 0.9.0. Settings from 0.9.0
are read as they are. (0.9.1 was never published; its changes are here.)

**Setting up a keyboard**
- Setup says which keyboard it is setting up, and has two steps: press `F5`
  three times in a row to confirm the keyboard sends F-keys first, then say
  what's printed on each key.
- Presets are used only when you choose one. SceneKeys no longer picks one from
  the keyboard's name, so a Huawei laptop isn't taken for a MateBook X.
- A keyboard with no name of its own is called "Bluetooth keyboard" or "USB
  keyboard", never after a guessed maker.
- Keys the keyboard does itself can be marked as printed on the key: keyboard
  backlight, Wi-Fi, Easy-Switch, the maker's app, or something you name. They
  stay F-keys, and SceneKeys says to hold Fn for what's printed.

**The first-use guide**
- Can't be finished without a keyboard, and opens again at each start until
  one is set up. Settings leads back to it until then.
- Has its own English / 简体中文 switch, and moves on by itself once a keyboard
  is added.
- Its examples follow the keyboard you set up.

**Apps**
- Apps SceneKeys knows (about 50) keep their F-keys with nothing to set up,
  including ones already open when SceneKeys starts.
- A new settings file sets up only File Explorer and the desktop. Running apps
  SceneKeys doesn't know are no longer listed; they can still be added.
- New shortcut: **open an app**, from the Start menu's apps or any program.
- While media plays, volume, brightness and playback shortcuts now win over a
  shortcut you gave that app alone too.

**Fixes**
- The desktop no longer claims `F3` is Search.

## 0.9.0 — 2026-09-20

The first public build.
