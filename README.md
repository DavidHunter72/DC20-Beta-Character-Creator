# DC20 Beta 0.10 — Character Creator

A fully self-contained, single-file character creator for **DC20 RPG Beta 0.10** by The Dungeon Coach.

No build step. No server. No dependencies (except an icon font via CDN). Just open `dc20-character-creator.html` in any modern browser.

## Features

- **10-step guided character creation** covering all of Level 1
- **13 ancestries** — Human, Elf, Dwarf, Halfling, Gnome, Orc, Dragonborn, Angelborn, Fiendborn, Giantborn, Goblin, Beastkin, Leshy
- **13 classes** — Barbarian, Bard, Champion, Cleric, Commander, Druid, Hunter, Monk, Rogue, Sorcerer, Spellblade, Warlock, Wizard (filterable by Martial / Spellcaster / Hybrid)
- **All subclasses** with Paragon tags — 2 per class, 26 total
- **Point Buy attribute system** (12 points, start at −2, cap at +3)
- **10 backgrounds** with suggested skill lists
- **16 skills + 8 trades** with Intelligence-adjusted points
- **24 spells** filterable by school (Astromancy, Elemental, Enchantment, Invocation, Nullification, Transmutation)
- **12 maneuvers** across Attack, Defense, Grapple, and Utility types
- **40 talents** across General, Class-specific, Paragon, and Multiclass categories
- **Calculated stats** — HP, PD, AD, Save DC, Grit Points, Attack Check, Rest Points, Death's Door
- **Live character sheet** with all chosen options summarized
- **Export to JSON** — machine-readable character data
- **Export to HTML** — printable, styled character sheet

## Usage

### Locally
```
open dc20-character-creator.html
```
Or just double-click the file. It works in Chrome, Firefox, Safari, and Edge.

### GitHub Pages
1. Fork this repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Your creator will be live at `https://yourusername.github.io/dc20-character-creator/`

### Hosting anywhere
Upload `dc20-character-creator.html` to any static host — Netlify, Vercel, Cloudflare Pages, GitHub Pages, etc.

## Export Formats

### JSON (`character_name_dc20.json`)
Structured character data for use in other tools, VTTs, or automation:
```json
{
  "system": "DC20 Beta 0.10",
  "name": "Thorin Emberveil",
  "level": 1,
  "ancestry": { "primary": "Dwarf", "secondary": null },
  "class": { "name": "Barbarian", "type": "martial", "subclass": "Elemental Fury" },
  "attributes": { "might": 3, "agility": 0, "charisma": -1, "intelligence": 0 },
  "stats": { "hp": 13, "pd": 9, "ad": 12, "saveDC": 14, ... },
  ...
}
```

### HTML Sheet (`character_name_dc20_sheet.html`)
A clean, print-ready character sheet with a full stat block, spell/maneuver/talent tables, and equipment list. Print it directly from your browser.

## Ruleset Coverage (Beta 0.10)

This tool implements the following from the official DC20 Beta 0.10 rulebook:

| Section | Coverage |
|---------|----------|
| Attribute Point Buy | ✅ Full |
| Ancestry System | ✅ 13 ancestries with trait descriptions |
| Class System | ✅ All 13 classes with HP/SP/MP |
| Subclasses | ✅ All 26 subclasses with Paragon tags |
| Background System | ✅ 10 backgrounds |
| Skills (16 skills) | ✅ Full list, Intelligence-adjusted points |
| Trades (8 trades) | ✅ Full list |
| Spells (24) | ✅ Descriptions, school, cost, range |
| Maneuvers (12) | ✅ All types covered |
| Talents (40) | ✅ General, Class, Paragon, Multiclass |
| Stat Calculations | ✅ HP, PD, AD, Save DC, Attack, Grit, etc. |
| Combat Mastery | ✅ Level 1 value (CM = 1) |
| Starting Equipment | ✅ Weapons and armor selection |

**Not covered** (beyond scope of Level 1 creation): leveling, magic item system, monster stat blocks, full spell enhancement lists.

## Credits

- **DC20 RPG** created by [The Dungeon Coach](https://www.youtube.com/@TheDungeonCoach)
- Character creator built from DC20 Beta 0.10 rulebook content
- This is an unofficial fan tool — not affiliated with The Dungeon Coach

## License

This project is an unofficial fan tool. The DC20 game system and all related content belong to The Dungeon Coach. This tool is free to use, modify, and share for personal and fan use.
