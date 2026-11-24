# Bleh Overlay

Bleh is a Windows overlay for Minecraft Java Edition focused on BedWars player
stats, tab-list tools, and configurable in-game utilities. It includes an
injector that downloads and verifies the overlay DLL from GitHub Releases.

[Download the latest release](https://github.com/Maksym2607/Bleh-Overlay/releases/latest) ·
[Try the custom-rank preview](https://maksym2607.github.io/Bleh-Overlay-Custom-Ranks/rank-preview.html) ·
[Report a bug](https://github.com/Maksym2607/Bleh-Overlay/issues)

## Features

- **BetterTab:** sortable player stats, team detection, configurable columns,
  player heads, and support for manual tab entries.
- **Stats views:** in-game GUI, tab list, and player search.
- **Custom ranks:** match players by username or UUID and preview rank
  animations and text effects.
- **Nick remapping:** show a chosen real name and stats for nicked players in
  BetterTab; saved remaps expire after 14 days.
- **BedWars tools:** optional shop-click behavior, match utilities, and
  configurable automation.
- **Tags and profiles:** Seraph and Urchin tag support, with client-aware tab
  styling where available.
- **Injector updates:** stable releases by default, with an optional
  pre-release update channel.

## Install

1. Download the Bleh injector from the
   [latest GitHub release](https://github.com/Maksym2607/Bleh-Overlay/releases/latest).
2. Run the injector and select your Minecraft instance.
3. Inject Bleh. The injector downloads the matching DLL from the latest
   published release and verifies its SHA-256 digest before use.
4. Open the in-game overlay with **Insert** (the default toggle key).

The first download requires an internet connection and a published release.
The injector can reuse its verified DLL cache when offline. In injector
**Settings**, enable **Pre-release updates** to check pre-release tags; stable
releases are selected by default.

## Custom ranks

Ranks are maintained in the
[Bleh custom-ranks repository](https://github.com/Maksym2607/Bleh-Overlay-Custom-Ranks).
Use the [interactive preview](https://maksym2607.github.io/Bleh-Overlay-Custom-Ranks/rank-preview.html)
to try the available animations and text effects, then copy or download a
sample `ranks.json` entry.

See the in-repository [custom-ranks guide](Bleh/CUSTOM_RANKS.md) for supported
keys, colors, effects, and examples.

## Commands

Use `/bleh help` in-game to see the commands available in your build. Common
commands include:

| Command | Description |
| --- | --- |
| `/bleh stats <player>` | View a player's stats. |
| `/bleh remap <nick> <name>` | Display a chosen name for a nick in BetterTab for 14 days. |
| `/bleh add <player>` | Add a player to the manual tab list. |
| `/bleh remove <player>` | Remove a manual tab entry. |
| `/bleh clearcache` | Clear cached stats and saved remaps. |

## Compatibility and notes

- Bleh and its injector are Windows-only.
- The overlay targets Minecraft Java Edition 1.8.9. Support can vary between
  clients and releases; check the release notes if a feature does not work in
  your client.
- For Hypixel stat fetches, an API key can improve reliability; keyless mode is
  also available.
- Remaps are user-supplied and do not verify a player's identity.

## Build from source

Build on Windows with Visual Studio C++ tools, CMake, and the Slint C++ 1.16.1
SDK. From the repository root, configure and build with:


## License

The project is licensed under the [MIT License](LICENSE).
