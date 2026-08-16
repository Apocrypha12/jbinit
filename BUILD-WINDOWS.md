# Building from Windows

This project requires Apple's iPhoneOS SDK, Apple `ld`, and `hdiutil`, so the
Windows entry point is the included GitHub Actions workflow running on macOS.

1. Authenticate GitHub CLI with `repo` and `workflow` scopes.
2. Fork this repository to the authenticated account.
3. Push the local branch `codex/build-jbinit` to that fork.
4. Wait for **Build jbinit ramdisk** to finish.
5. Download the `jbinit-ios15-arm64` artifact.

The artifact contains `jbinit`, `launchd`, `jb.dylib`, `ramdisk.dmg`, and a
SHA-256 checksum manifest. It does not contain kernel patches.
