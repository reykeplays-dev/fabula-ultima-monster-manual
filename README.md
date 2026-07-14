# Fabula Ultima Monster Manual

A growing collection of creatures adapted for **Fabula Ultima** and prepared for use with the **Project FU** game system in **Foundry Virtual Tabletop**.

The module contains ready-to-use NPC actors, creature artwork, encounter tables, and utility macros intended to make it easier for Game Masters to build encounters and populate Fabula Ultima adventures.

> **Work in progress:** This compendium is under active development. Creature statistics, artwork, organization, and supporting tools may change as the collection grows.

## Contents

The module currently includes three Foundry compendium packs:

- **Fabula Monster Manual** — NPC actors built for the Project FU system.
- **Encounter Tables** — rollable tables that reference creatures from the monster compendium.
- **Monster Manual Macros** — utility macros for searching the compendium, selecting scenes or backgrounds, and rolling encounters.

The included creature artwork is organized into the following broad categories:

- Beasts
- Constructs
- Demons, devils, and other supernatural creatures
- Elementals
- Humanoids
- Monsters
- Plants
- Undead
- Dragons

## Requirements

- **Foundry Virtual Tabletop:** Version 13 or later
- **Game System:** [Project FU](https://foundryvtt.com/packages/projectfu)
- **Tested Project FU Version:** 4.16.0

This is a content module and does not replace the Project FU game system. Project FU must be installed and enabled in the world where this module will be used.

## Installation

### Install with the Foundry manifest URL

1. Open Foundry Virtual Tabletop.
2. Select **Add-on Modules** from the Configuration and Setup screen.
3. Click **Install Module**.
4. Paste the following URL into the **Manifest URL** field:

```text
https://github.com/YOUR-GITHUB-USERNAME/fabula-ultima-monster-manual/releases/latest/download/module.json
```

5. Click **Install**.
6. Launch a world using the Project FU system and enable **Fabula Ultima Monster Manual** under **Manage Modules**.

### Manual installation

1. Download the latest module ZIP from the repository's Releases page.
2. Extract it into Foundry's `Data/modules` directory.
3. Confirm the resulting folder is named:

```text
fabula-ultima-monster-manual
```

4. Restart Foundry if it was already running.
5. Enable the module from **Manage Modules** inside a Project FU world.

## Using the Compendiums

After enabling the module, open the **Compendium Packs** tab in Foundry. The following packs should be available:

- `Fabula Monster Manual`
- `Encounter Tables`
- `Monster Manual Macros`

Actors can be dragged from the monster compendium into the world or directly onto a scene. Macros may be imported to the hotbar or executed from the compendium.

The encounter tables reference actors in the module's `fu-mm` compendium. Renaming the module ID or pack name may break those references.

## Repository Structure

```text
fabula-ultima-monster-manual/
├── assets/
├── packs/
│   ├── encounter-tables/
│   ├── fu-mm/
│   └── macros/
├── .gitattributes
├── module.json
└── README.md
```

The LevelDB files inside `packs/` are binary files. The included `.gitattributes` file marks them appropriately for Git.

## Creating a GitHub Release

Foundry's manifest installer expects the release assets to use consistent filenames.

For each release:

1. Update the `version` value in `module.json`.
2. Update the version number in the `download` URL in `module.json`.
3. Place the complete module inside a folder named `fabula-ultima-monster-manual`.
4. Compress that folder as:

```text
fabula-ultima-monster-manual.zip
```

5. Create a GitHub release with a matching tag, such as `v0.1.0`.
6. Attach both of these files to the release:

```text
module.json
fabula-ultima-monster-manual.zip
```

The `manifest` URL uses GitHub's `releases/latest/download/` path, while the `download` URL points to the versioned release asset.

## Development Notes

The module ID and registered compendium pack names should remain stable:

```text
Module ID: fabula-ultima-monster-manual
Actor Pack: fu-mm
Encounter Table Pack: encounter-tables
Macro Pack: macros
```

Changing these identifiers can invalidate UUID links stored in actors, macros, roll tables, journals, or other Foundry documents.

The uploaded development archive also contained an unregistered `packs/dnd-mm` database. It is not included in the documented release structure because it is not declared in `module.json`. If it is an intentional fourth compendium, it must be given a permanent pack name, label, document type, and manifest entry before release.

## Attribution and Disclaimer

This is an unofficial, fan-created project intended for use with Fabula Ultima. It is not affiliated with or endorsed by Need Games, Rooster Games, the creators of Fabula Ultima, Foundry Gaming LLC, or the Project FU development team.

Creature concepts inspired by other games or media remain the property of their respective owners. This project should not redistribute copyrighted text or artwork without permission. Adapted statistics and original supporting material should be presented as independent fan content.

## License

No license was included in the uploaded module pack. Add a `LICENSE` file before publishing the repository and update the license link in `module.json` to match your chosen license and the rights you hold to the included content and artwork.

## Contributing and Issues

Use the GitHub repository's issue tracker to report incorrect statistics, broken actor links, missing artwork, macro problems, or compatibility issues. When reporting a problem, include the Foundry version, Project FU version, module version, and the affected creature or compendium entry.
