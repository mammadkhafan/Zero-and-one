# OpenRoad — Native ARM64 port

This repository is the working destination for converting the OpenRoad Godot project to native compiled game logic for Android ARM64.

## Source import
The original Godot project has been copied into `reference/` from [mammadkhafan/-](https://github.com/mammadkhafan/-). Its gameplay scripts are GDScript and therefore are **not** native machine code.

## Native conversion status
- [x] Import original project source for reference.
- [ ] Port gameplay and world logic from GDScript to C++/GDExtension.
- [ ] Build the GDExtension for Android ARM64.
- [ ] Integrate the native extension into the Godot Android export.
- [ ] Build and verify an installable APK.

A normal Godot APK can run without compiling on the phone, but GDScript still executes through Godot's script runtime. This repository's target is stricter: move the game logic into precompiled native ARM64 code. No APK is claimed to exist until the native port is complete and the build succeeds.

## Reference
See `reference/README.md` for the original project's features and known limitations.
