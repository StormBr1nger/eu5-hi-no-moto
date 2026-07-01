# Mod Structure

Folder markers:

- 🟩 **Mod folders** — real EU5 mod folders loaded by the game.
- 🟦 **Development folders** — planning, documentation, research, assets, and tools for mod development.
- ⬜ **Repository files** — Git and project control files.

```text
hi-no-moto/
├── ⬜ .git/                  # Git repository data
├── ⬜ .gitignore             # Git ignore rules
├── ⬜ README.md              # Main project overview
├── ⬜ ROADMAP.md             # Project phases and plan
├── ⬜ CHANGELOG.md           # Change history
├── ⬜ LICENSE.md             # License placeholder
├── ⬜ MOD-STRUCT.md          # Repository and mod folder structure
│
├── 🟦 docs/                  # General project documentation
│   ├── README.md
│   ├── vision.md
│   ├── design-pillars.md
│   ├── terminology.md
│   └── references.md
│
├── 🟦 design/                # Game design documents
│   ├── README.md
│   ├── core-loop.md
│   ├── political-system.md
│   ├── clan-system.md
│   ├── warfare.md
│   └── economy.md
│
├── 🟦 history/               # Historical research and planning
│   ├── README.md
│   ├── timeline.md
│   ├── periods.md
│   ├── clans.md
│   └── provinces.md
│
├── 🟦 assets/                # Working references, concepts, and source images
│   ├── maps/
│   ├── flags/
│   ├── icons/
│   └── references/
│
├── 🟦 tools/                 # Helper scripts and automation
│   └── scripts/
│
├── 🟩 in_game/               # Actual EU5 in-game mod files
│   └── ...
│
├── 🟩 loading_screen/        # Actual EU5 loading screen mod files
│   └── ...
│
└── 🟩 main_menu/             # Actual EU5 main menu mod files
    └── ...
```

## Mod Descriptor Location

The launcher descriptor file is stored beside the main mod folder, not inside it:

```text
Europa Universalis V/mod/
├── hi-no-moto/               # Repository and mod folder
└── hi-no-moto.mod            # Launcher descriptor
```

## Folder Logic

```text
🟩 Game-loaded folders:
in_game/
loading_screen/
main_menu/

🟦 Development folders:
docs/
design/
history/
assets/
tools/

⬜ Repository control:
.git/
.gitignore
README.md
ROADMAP.md
CHANGELOG.md
LICENSE.md
MOD-STRUCT.md
```

Development folders are kept in Git because they contain project planning and design work. They are not part of the game-loaded mod content.
