# Security

AuxTray handles one thing worth protecting: the sign-in to your AC Freedom account. It keeps the password in the
macOS Keychain, sends it only to AC Freedom, and keeps the session AC Freedom returns in the app's preferences.

## Reporting a problem privately

If you find a way AuxTray could expose an account, a password or a session, or could be made to send commands
nobody asked for, please do not open a public issue. Use **Report a vulnerability** on this repository's
[Security tab](https://github.com/atefalshehri/AuxTray/security). That reaches the maintainer privately.

Say what you found and how to see it happen. You will get an answer, though this is a hobby project and it may
take some days.

## Only from this page

AuxTray is not registered with Apple, so macOS cannot tell you who made a copy of it. Allow only a copy that you
downloaded from this repository's [releases](https://github.com/atefalshehri/AuxTray/releases). Each release lists
the SHA-256 of its disk image. To check a download against it:

```bash
shasum -a 256 ~/Downloads/AuxTray-0.2.0.dmg
```

## What is not in AuxTray's hands

AuxTray talks to a cloud service run by the units' maker. Problems in that service, or in the units themselves,
are theirs to fix. If you find one, tell them.

The constants AuxTray uses to talk to that service come from the maker's own phone app and are not secrets of
anyone's account.
