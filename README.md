# Safe Browser


## Overview

This repository holds the build tools needed to build the Safe browser for macOS, Windows, and Linux.  In particular, it fetches and syncs code from the projects we define in `package.json` and `src/brave/DEPS`:

  - [Chromium](https://chromium.googlesource.com/chromium/src.git)
    - Fetches code via `depot_tools`.
    - sets the branch for Chromium (ex: 65.0.3325.181).
  - [safe-browser-core](https://github.com/adrianhrinko/safe-browser-core.git)
    - Mounted at `src/brave`.
    - Maintains patches for 3rd party Chromium code.
  - [adblock-rust](https://github.com/brave/adblock-rust)
    - Implements Brave's ad-block engine.
    - Linked through [brave/adblock-rust-ffi](https://github.com/brave/adblock-rust-ffi)

As it is based on the Brave project, see [original brave-browser repository](https://github.com/brave/brave-browser) for more information.
