# Project Tandem Android source

The complete public source tree is under [`source/`](source/). It contains the
Android frontend, OpenGL ES/EGL renderer, AAudio backend, touchscreen controls,
shared recompilation runtime, and EOS integration interfaces.

The repository intentionally excludes game images, generated `gen/` output,
APK/so files, EOS credentials, keystores, and the proprietary EOS SDK runtime.
Obtain the SDK from Epic under its developer terms and keep it outside Git.

Configure with Android SDK/NDK, CMake, Ninja, Python 3, and a private dependency
directory passed as `-DTANDEM_EXTERNAL_ROOT=/path/to/dependencies`. The public
source contains the exact build inputs and documents the required boundary in
[`source/BUILDING-PUBLIC.md`](source/BUILDING-PUBLIC.md).

The Android app reads `eos.json` from private application storage. Never commit
that file, client secrets, tokens, signing keys, or build output.
