**English** | [Русский](CHANGELOG_RU.md)

# Changelog

## [0.1.3] — 2026-11-27

### Engine & Custom Maps
- Fixed crashes when connecting to KZ and custom servers with split-texture (`*T.mdl`) or non-standard `.mdl` files, and increased the 64-bit engine memory pool limit to 256 MiB.

### MOTD & Server Compatibility
- Fixed false `Kicked :"protector_detected"` kicks on DopBan-protected servers: MOTD now preserves explicit `http://` pages instead of forcing HTTPS upgrades, allows MOTD cookie verification to finish in the background when the MOTD window is closed quickly, and keeps MOTD cookies working inside embedded frames.

---

## [0.1.2] — 2026-11-27

### Renderer & Large Maps
- Fixed `Out of memory` crashes (`csgl3`) when loading large KZ maps: replaced fixed-size renderer memory blocks with dynamically growing arenas, fixed a per-map level allocation leak, and raised lightmap atlas, surface, and texture limits.

---

## [0.1.1] — 2026-11-27

### Audio & Voice
- Improved SDL2 audio buffering and underrun recovery to eliminate crackling and stuttering; `soundinfo` now displays SDL callback frames and underrun count.
- Added optional background audio/voice muting when unfocused (`snd_mute_losefocus`, enabled by default, configurable in **Options -> Audio**).

### Window & Alt-Tab
- Fullscreen mode now properly minimizes to the taskbar on Alt-Tab instead of staying behind other windows.

### HUD, Menus & Console
- Fixed AMXX menus closing when switching to Spectator.
- Repositioned the HUD Layout Editor toolbar below the `Spectator Banner` so it can be grabbed directly with the mouse, and made the toolbar draggable by its header.
- Developer console now preserves scroll position when scrolled up during active chat/logging and resumes auto-scrolling when returning to the bottom or submitting a command.

### Performance
- Reduced dynamic HUD rendering cost and optimized high-FPS frame pacing CPU overhead.

---

## [0.1.0] — 2026-11-26

### Initial Public Release (x64)
- **64-bit Split-Loop Engine**: 500+ visual FPS with authentic 100/133 Hz movement physics (`fps_max`, `fps_override`).
- **Tactical Glass Visor UI & HUD Editor**: Modern RmlUi interface, interactive scoreboard with Steam avatars & jumpstats telemetry, crosshair customizer, and full drag-and-scale HUD Editor.
- **Low-Latency Input (`Reflex-Lite`)**: Adaptive GPU/frame pacing (`hnsru_reflex`).
- **OpenGL 3 Renderer (`r_gl3`)**: Modern hardware-accelerated renderer with optional classic fallback.
- **Audio & Voice**: Smooth volume ramping, soft clipping, category volume controls, and high-resolution Steam voice (`voice_hq`).
- **Networking & Server Browser**: Multi-threaded A2S server browser and multi-host FastDL downloads.
- **Auto-Updater**: Signed release and `-beta` update channels with in-game patch notes (`hnsru_changelog`).
