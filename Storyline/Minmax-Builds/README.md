# Minmax-Builds — Status and Open Questions

**Status: concept confirmed kept, but tentative.** The user has confirmed they want to hold onto the idea of dedicated, per-stat-combination "minmax build" content — flavor text, unique interactions, and secret-ending hooks written specifically for characters who built extreme, specialized stat combinations at character creation. Nothing in this folder should be treated as locked or as blocking other work; it's parked here deliberately, exactly as tentative as the concept it documents.

This README exists to explain what the concept is, flag the one real open design question standing in the way of populating it, and describe the folder-naming convention and per-folder file set to use once that question is resolved. **Nothing below should be read as an answer to that open question** — it's presented as a live decision for the user, not something this pass resolved on its own.

---

## The Concept

A "minmax build" is an archetype defined by pushing a small number of [MAPLE-BUD](../../to-be-integrated/not-SPECIAL.md) stats to a high floor (originally: 3 stats at 8+) while leaving the rest wherever they land. Each archetype gets its own small folder of content: quest hooks that suit that specific build, secret-ending triggers it can reach that other builds can't, and flavor interactions for playing at the high and low extremes of its defining stats. `Single-Stat_-_Max.md` and `Single-Stat_-_Min.md` (this folder's root files, already rewritten for Toronto Fell Out) are the one-stat version of the same idea; the 35 numbered subfolders below are the three-stat version, inherited from Inner Tepenia's own MACHINE-stat system.

---

## Stat Pool — RESOLVED 2026-07-29

**Confirmed: 35 combinations, drawn from the 7 skill-bearing MAPLE-BUD stats — Might, Agility, Perception, Endurance, Brains, Utility, Determination. Luck is excluded.**

Rationale: Luck has no dedicated skill of its own (per `Skills.md`) — it grants a flat bonus to every other skill instead, rather than defining a domain the way Might, Brains, or any other stat does. A "Luck-heavy build" doesn't specialize a character into anything distinct, so it doesn't earn a slot in a build-archetype scheme the way a genuinely skill-bearing stat does. Utility stays in the pool — it governs three real skills (Repair, Engineering, Chemistry) and specializes a character just as concretely as any other stat.

This isn't a coincidental match to Inner Tepenia's own 35 (from their 7-stat MACHINE system, all of which are skill-bearing) — it's the same underlying rule applied to Toronto Fell Out's own stat system: combine only the build-defining, skill-bearing stats. Toronto Fell Out's 7-stat pool just happens to also total 7, for a real structural reason rather than a borrowed number.

---

## Folder-Naming Convention — Confirmed Code List

Using single-letter MAPLE-BUD initials in canonical order (M, A, P, E, B, U, D — Luck's "L" simply doesn't appear in any code, since it's excluded from the pool), all 35 three-letter combinations:

MAP, MAE, MAB, MAU, MAD, MPE, MPB, MPU, MPD, MEB, MEU, MED, MBU, MBD, MUD,
APE, APB, APU, APD, AEB, AEU, AED, ABU, ABD, AUD,
PEB, PEU, PED, PBU, PBD, PUD,
EBU, EBD, EUD,
BUD

(15 codes starting with M, 10 starting with A, 6 starting with P, 3 starting with E, 1 starting with B — the same triangular-number pattern Inner Tepenia's own 35 followed, just built from a different 7-letter alphabet.)

Folder naming convention going forward: `##-XXX` (e.g. `01-MAP`, `35-BUD`), matching Inner Tepenia's own `##-MAC`-style format, numbered in the order listed above.

---

## The Existing 35 MACHINE-Coded Folders: Stale, Pending Rename

The 35 folders currently in this directory (`01-MAC` through `35-INE`) are a direct, untouched copy from Inner Tepenia. **They are not current Toronto Fell Out content.** Their names use Inner Tepenia's MACHINE stat initials, and their populated files (`Secret-Ending_Triggers.md`, `Unique_Interactions_-_High.md`, `Unique_Interactions_-_Low.md` — `Questlines_and_Possibilities.md` is empty in every one) are full of Inner Tepenia-specific lore: Concordia's districts, its factions, its NPCs, its Arcanet.

**Now that the stat pool is confirmed (also 35, but a different 7-letter alphabet — see above), the correct move is to delete all 35 MACHINE-coded folders and regenerate a fresh set of 35 using the MAPLE-BUD-coded names above, empty of content.** Not yet done in this pass — a mechanical folder-rename/regenerate step, separate from actually deciding the stat pool. **Do not mistake any of the existing 35 MACHINE-coded folders for current Toronto Fell Out canon in the meantime.**

---

## Per-Folder File Set (template, to replicate once populated)

Each build-archetype folder — present in Inner Tepenia's 35 folders and the empty `z-template/` folder — uses this same four-file shape:

- **`Questlines_and_Possibilities.md`** — quest hooks and questline ideas this specific build is especially suited to pursue or unlock. (Empty in every one of Inner Tepenia's existing 35 folders — never actually populated there either, so there's no real content to adapt even for the stats that do carry over.)
- **`Secret-Ending_Triggers.md`** — NPC-offered and world/environmental triggers (per-stat-combination) that lead toward that build's best-fitting secret endings. Once Toronto Fell Out's own secret-ending taxonomy is populated (see `Storyline/Endings/Secret-Endings/Secret_Endings_Design_Framework.md`), this is where a Minmax-specific ending's actual trigger would be documented, subject to the same **World Trigger law** as every other secret ending — a discoverable physical object or location, never a hidden stat check or NPC-initiated approach.
- **`Unique_Interactions_-_High.md`** — special interactions available across Toronto Fell Out's (currently nonexistent) districts/locations when all three of this build's defining stats are high, in the same "minimum 5 per location" density as Inner Tepenia's own samples.
- **`Unique_Interactions_-_Low.md`** — the inverse: special interactions for the same three stats all sitting low (an underdog/unlucky variant, distinct from the single-stat-low flavor in `Single-Stat_-_Min.md`).

**Do not populate any of these for real yet.** The stat pool is now resolved, but one blocker remains: Toronto Fell Out has zero designed districts, factions, or NPCs for "per-location interaction" and "NPC trigger" content to reference (see the project's own ground rule against inventing that content ahead of time). Once that's resolved, this file set is the shape to build from.

---

## Summary of What's Actually Done vs. Open

| Item | Status |
|---|---|
| `Single-Stat_-_Max.md` | Rewritten for MAPLE-BUD — done |
| `Single-Stat_-_Min.md` | Rewritten for MAPLE-BUD — done |
| Luck/Utility inclusion in the 3-stat scheme | **Resolved 2026-07-29 — 35 combinations, Luck excluded, Utility included** |
| MAPLE-BUD-initial folder-naming convention | **Resolved — full 35-code list documented above** |
| The 35 existing `##-XXX` folders | Still the old MACHINE-coded set — pending deletion/regeneration with the confirmed MAPLE-BUD codes |
| Per-folder file set (4 files) | Template documented above, not populated — blocked on districts/factions/NPCs existing |
