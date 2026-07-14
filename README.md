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
https://github.com/reykeplays-dev/fabula-ultima-monster-manual/releases/latest/download/module.json
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


