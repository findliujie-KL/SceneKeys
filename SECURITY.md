# Security and privacy

## What SceneKeys can see

SceneKeys uses a Windows low-level keyboard hook so that it can replace an
F-key press with a shortcut. The hook is told about every key press, so this
section says exactly what is done with that.

- **Only `F1`–`F12` are acted on.** Every other key is passed straight through.
- **Ctrl, Alt, Shift and Win are only checked for whether they are held down**,
  at the moment an F-key is pressed.
- **Nothing is written down.** No key press is stored, logged, counted or
  timed. There is no keystroke history anywhere in the app or on disk.
- **No network code.** SceneKeys never connects to anything. It has no update
  check, no statistics and no crash reporting.
- **About the app in front,** SceneKeys asks Windows for the program's file
  name and whether it is playing media. It never reads window titles, page
  addresses, documents or audio.
- **On disk** it keeps one readable text file, `settings.ini`, holding your
  keyboards, shortcuts and per-app settings.

## Reporting a vulnerability

Please report anything security related privately, through GitHub's
**Security → Report a vulnerability** on this repository, rather than in a
public issue. Please include what you did, what happened, and the Windows
version you saw it on. You'll get an answer as soon as possible; this is a
one-person project, so please allow a few days.

## Checking your download

Every release lists the SHA-256 checksum of each file. To check one:

```powershell
Get-FileHash .\SceneKeys-0.9.0-setup.exe -Algorithm SHA256
```

Downloads are not signed with a code-signing certificate yet, so Windows
SmartScreen may warn that the publisher is unknown, and some antivirus products
may report a false positive because of the keyboard hook. If one does, please
open an issue naming the product and its version.
