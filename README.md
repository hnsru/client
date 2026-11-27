**English** | [Русский](README_RU.md)

# HNSRU Client (x64)

A custom 64-bit Counter-Strike 1.6 client built for **HNS, KZ, and Surf** — featuring the **Tactical Glass Visor** interface, **Split-Loop** 500+ visual FPS with authentic 100/133 physics, **Reflex-Lite** low-latency input, and built-in automatic updates.

- **Download Page & Live Changelog:** https://hnsru.github.io/client/
- **Changelog:** [CHANGELOG.md](CHANGELOG.md)
- **Full Feature Overview:** [docs/ANNOUNCEMENT.md](docs/ANNOUNCEMENT.md)
- **Releases:** https://github.com/hnsru/client/releases

## Installation

1. Download the latest [`hnsru.exe`](https://github.com/hnsru/client/releases/latest/download/hnsru.exe) from the Releases page.
2. Place `hnsru.exe` in your Half-Life / Counter-Strike 1.6 root folder (next to `hl.exe` and `cstrike`).
3. Make sure Steam is running, then launch `hnsru.exe`.

## Update Channels

| Channel | How to use | Behavior |
|---|---|---|
| **Release** (default) | Launch `hnsru.exe` normally | Automatically checks on startup and while running. Updates and restarts cleanly from the Main Menu; while in-game, shows a subtle `CLIENT OUTDATED` banner at the top without interrupting play. |
| **Beta** | Add `-beta` launch flag | Opts into preview builds from the beta channel (`-beta` is preserved across automatic restarts). |

You can review the latest patch notes anytime from the Main Menu or console with `hnsru_changelog`.
