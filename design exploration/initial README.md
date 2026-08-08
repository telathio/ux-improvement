# The Telath Design System

Telath is a play-by-post fantasy forum that has been written continuously for decades.
Years of threads, a wiki the community played into existence, and a world no single person
owns. This repository holds the visual system for it.

The system exists to make that history **feel** as old, as continuous, and as much the users'
as it actually is, while making the site itself easier to read earlier or later in the day, which is when much of Telath gets written.

---

## What's here

| File | What it is |
|---|---|
| `telath.css` | Custom properties plus base type and colors. |
| `Telath Brand Guidelines` | The guidelines document that includes color palette, type, wordmark, sigils, iconography, imagery, interface parts, do's/dont's. |
| `Initial Designs` | Various pages and components used by the game and its players, offered as both images and Figma files with components. |
| `uploads/` | Source artwork such as region arms as vectors and restyled world maps or wiki assets. |

Open any `.html` file in a browser. They're self-contained.

---

## The three rules

Everything else in the system follows from these.

**1 · Dark first.** Telath is "read at night." Every surface is built on the void, and light
is something the interface uses carefully.

**2 · Tool and world are different voices.** Anything the *site* says is sans or mono.
Anything the *world* says — titles, places, prose, a character's own words - is Garamond.
The two never mix inside one line.

**3 · Player creations stay theirs.** House assets get the brand treatment. Player art never does.

---

## Palette

| Token | Hex | Use |
|---|---|---|
| `--tel-void` | `#0D0E12` | masthead, footer, overlays |
| `--tel-page` | `#131418` | page background |
| `--tel-keep` | `#1B1C21` | raised surfaces — posts, cards, inputs |
| `--tel-hairline` | `#2A2B31` | 1px separators, never thicker |
| `--tel-granite` | `#45464E` | structure, resting icons, disabled |
| `--tel-wardlight` | `#8FB7D9` | **the** interactive color |
| `--tel-sigil` | `#A894D9` | magic and canon events only |

Text runs `#EDEEF1` → `#D2D4DA` → `#93969F` → `#888B95`. That last value is the floor: it clears AA on both the page ground and the raised surface. Never go dimmer.

**The grounds are near-neutral on purpose.** They carry a trace of blue, which is enough to feel on the cooler side but not enough to read as a color. All the chroma in the system is saved for wardlight and sigil, which is what lets two accents do so much work. 

One interactive color means a player can scan a thread and know instantly what is clickable. There is no success green and no error red; use the mono system voice and an icon instead. 

---

## Type

Three faces, each with one job.

- **EB Garamond** — the wordmark, thread titles, region and character names, and every word
  a player writes. Prose sets at 20/1.68 with a 68-character measure.
- **Public Sans** — the chrome. Navigation, buttons, forms, moderation tools. 15px default.
- **IBM Plex Mono** — the system voice. Dice rolls, edit notices, timestamps, canon stamps,
  section labels. Always small, always letterspaced.

Rules worth stating outright:

- **Mono is never a sentence.** If it needs a comma, it belongs in sans.
- **Nothing anyone reads goes below 13px.** Mono labels are the one exception, at 9-11px
  uppercase with 0.14-0.24em tracking — labels, counts and timestamps only.
- **Garamond time is story time; mono time is site time.** A dateline in Garamond is where
  and when a scene happens. A timestamp in mono is when someone hit "post."

---

## Sigils and heraldry

For vectorized sigils, the system uses two shapes: a circle and a diamond.

- **The circle contains** — a bounded thing: a region, a city, a guild, a house.
- **The diamond marks** — an event or a claim: a canon moment, a magical effect, a change to world political state.
- **Together they seal** — ratified history, used where staff might present canon, such as a new timeline.

Drawing rules: one flat color, no gradients or bevels. A solid field with the charge knocked out of it, so the mark is readable at any size. Scales to 20px, where only the charge survives. 

---

## Iconography

Two layers that never mix.

**UI glyphs** — adopt Phosphor or Lucide. 24 grid, 1.5px stroke, granite at rest, wardlight on hover and active, 20px rendered, 44px hit target. Single-weight only: duotone icons introduce a second value per glyph and the palette can't absorb it.

**World marks** — Heraldry for regions, factions, races, orders. These are not interface; they never appear inside a button.

---

## Imagery

The most important section in the system.

**House assets** are cooled toward wardlight, but the polarity depends on what they are. Textures, banners and atmosphere desaturate and tint light-on-void. 
**Documents — maps, charters, ledgers — stay dark ink on cool paper**, set into the page as a plate with a granite rule around it.

**Never invert a map.** Light lines on a dark ground appears like a schematic or a heads-up display; it makes the world feel engineered rather than drawn. A map is a made object someone carried. It should look printed.

**Player art is never touched.** Not filtered, not recolored, not cropped. The brand *contains* player art with a hairline frame and consistent sizing; it does not change it.

---

## Contributing

The system is small on purpose, and it stays useful only if it stays small. Proposed changes, questions, and arguments are always welcome.

*Brand guidelines v1.0 · August 2026 · by and for the community of Aelyria*
