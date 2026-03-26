# Attention
The code in this fork is created entirely by Gemini (3 Flash) and GH Copilot (whatever model it deems fit).

This repo exists in tandem with the original repo, specially providing features to Windows before this is stable enough.

# Status
Compiles, runs to UI. Have quirks while typing. Features yet to be implemented.
- [x] IME stack rewrite/implement for Windows

Works, but have some errors. Probably won't fix those since I've seen EVKey making the same error on my Windows installation.
- [x] Tray icon

Functional, albeit incomplete: missing icon, quick switch,...
- [ ] Further implementation due to dev's abandonment of the Windows' version plan

Some functions are missing; no per-app enable/disable;...

# Help needed
- Multiple functions are using placeholders e.g. file pickers
- Some features in the UI outright just not work


<p align="center">
	<img src="./icons/icon.png" width="90px">
</p>


<img width="1585" height="797" alt="screenshots" src="https://github.com/user-attachments/assets/42930e8a-77fb-4493-aa90-3c0bb9f1ab40" />


**Gõkey** - A Vietnamese input method editor.

- :zap: Excellent performance (Gen Z translation: Blazing fast!)
- :crab: Written completely in Rust.
- :keyboard: Supported both Telex and VNI input method.
- :sparkles: Focused on typing experience and features that you will use.

## Why another Vietnamese IME?

> technical curiosity

## About

This is my attempt to build an input method editor using only Rust. It's not the first, and definitely not the last.

The goal is to create an input method editor that enable users to type Vietnamese text on the computer using
either VNI or TELEX method. Other than that, no other features are planned.

## How to install
- macOS (ARM): Grab the build from https://nightly.link/imchocomint/goxkey-win/workflows/build/main?preview and install like any .app apps
- Windows: Download from Releases

## Build
Clone the repo, then run `cargo build --release`
## Dependencies
- [core-foundation](https://crates.io/crates/core-foundation), [core-graphics](https://crates.io/crates/core-graphics): for event handling on macOS
- [vi-rs](https://github.com/zerox-dg/vi-rs): the Vietnamese Input Engine
