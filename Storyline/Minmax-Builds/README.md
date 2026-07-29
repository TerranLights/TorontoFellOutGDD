# Minmax-Builds — Status and Open Questions

**Status: concept confirmed kept, but tentative.** The user has confirmed they want to hold onto the idea of dedicated, per-stat-combination "minmax build" content — flavor text, unique interactions, and secret-ending hooks written specifically for characters who built extreme, specialized stat combinations at character creation. Nothing in this folder should be treated as locked or as blocking other work; it's parked here deliberately, exactly as tentative as the concept it documents.

This README exists to explain what the concept is, flag the one real open design question standing in the way of populating it, and describe the folder-naming convention and per-folder file set to use once that question is resolved. **Nothing below should be read as an answer to that open question** — it's presented as a live decision for the user, not something this pass resolved on its own.

---

## The Concept

A "minmax build" is an archetype defined by pushing a small number of [MAPLE-BUD](../../to-be-integrated/not-SPECIAL.md) stats to a high floor (originally: 3 stats at 8+) while leaving the rest wherever they land. Each archetype gets its own small folder of content: quest hooks that suit that specific build, secret-ending triggers it can reach that other builds can't, and flavor interactions for playing at the high and low extremes of its defining stats. `Single-Stat_-_Max.md` and `Single-Stat_-_Min.md` (this folder's root files, already rewritten for Toronto Fell Out) are the one-stat version of the same idea; the 35 numbered subfolders below are the three-stat version, inherited from Inner Tepenia's own MACHINE-stat system.

---

## Open Question: Does This Scheme Include Luck and/or Utility? — NOT DECIDED HERE

Inner Tepenia's MACHINE attribute system has **7 stats** (Might, Agility, Calculation, Humanity, Investigation, Nerve, Engine), so its three-stat combinatorial scheme is C(7,3) = **35** combinations — exactly the 35 numbered folders currently sitting in this directory.

Toronto Fell Out's [MAPLE-BUD](../../to-be-integrated/not-SPECIAL.md) system has **8 stats** (Might, Agility, Perception, Luck, Endurance, Brains, Utility, Determination). Two of those — **Luck** and **Utility** — don't have obvious MACHINE equivalents:

- **Luck** has no dedicated skill of its own (per `Skills.md`) — it grants a flat bonus to every other skill instead. It's an open question whether a stat that works this way even makes sense as one leg of a three-stat "specialization" archetype, since maxing Luck doesn't specialize a character into a domain the way maxing Might or Brains does.
- **Utility** (crafting/repair/jury-rigging) has no clean MACHINE analogue either — Engine is closer to operational endurance/efficiency than hands-on craft, and Inner Tepenia's crafting-adjacent flavor was spread across Engine and Calculation rather than concentrated in one stat.

**This is a real, unresolved combinatorial design decision, not something to quietly pick a side on:**

- **If Luck and/or Utility are excluded** from this specific build-archetype scheme (keeping a Might/Agility/Perception/Endurance/Brains/Determination-only pool of 6 stats), the scheme stays at C(6,3) = **20** combinations — smaller than Inner Tepenia's 35.
- **If both are included** (all 8 MAPLE-BUD stats eligible), the scheme becomes C(8,3) = **56** combinations — larger than Inner Tepenia's 35.
- **If only one of the two is included** (7 eligible stats), the scheme lands back at C(7,3) = **35** — same count as Inner Tepenia, coincidentally, but built from a different 7 stats.

**Do not resolve this. Flag it for the user.** Whichever way it goes changes the folder count, the naming convention below, and which stats can headline a build archetype at all.

---

## Folder-Naming Convention (once the above is resolved)

Inner Tepenia's 35 folders are named by number + first-letter code of the three MACHINE stats involved, e.g. `01-MAC` = Might + Agility + Calculation. Toronto Fell Out's equivalent convention, once the Luck/Utility question is settled, should use the same pattern with MAPLE-BUD initials instead: e.g. a Might + Agility + Perception build would be coded `MAP`, a Brains + Utility + Determination build would be coded `BUD`, and so on. The exact eligible-stat pool (6, 7, or 8 stats) determines the final combination count and the specific list of codes — don't generate the list until the pool is confirmed, since regenerating it after picking the wrong pool means renumbering everything.

---

## The Existing 35 MACHINE-Coded Folders: Stale, Pending Rename

The 35 folders currently in this directory (`01-MAC` through `35-INE`) are a direct, untouched copy from Inner Tepenia. **They are not current Toronto Fell Out content.** Their names use Inner Tepenia's MACHINE stat initials, and their populated files (`Secret-Ending_Triggers.md`, `Unique_Interactions_-_High.md`, `Unique_Interactions_-_Low.md` — `Questlines_and_Possibilities.md` is empty in every one) are full of Inner Tepenia-specific lore: Concordia's districts, its factions, its NPCs, its Arcanet.

**Left as-is deliberately, not cleaned up in this pass:** renaming or repopulating them now would mean guessing at the Luck/Utility answer above. They're harmless dead weight sitting in the folder until that question is resolved — at which point the correct move is likely to delete all 35 (or renumber/rename them if the resolved pool happens to also total 35) and regenerate the set fresh from the confirmed stat pool, rather than trying to patch Inner Tepenia content in place. **Do not mistake any of these 35 folders for current Toronto Fell Out canon in the meantime.**

---

## Per-Folder File Set (template, to replicate once populated)

Each build-archetype folder — present in Inner Tepenia's 35 folders and the empty `z-template/` folder — uses this same four-file shape:

- **`Questlines_and_Possibilities.md`** — quest hooks and questline ideas this specific build is especially suited to pursue or unlock. (Empty in every one of Inner Tepenia's existing 35 folders — never actually populated there either, so there's no real content to adapt even for the stats that do carry over.)
- **`Secret-Ending_Triggers.md`** — NPC-offered and world/environmental triggers (per-stat-combination) that lead toward that build's best-fitting secret endings. Once Toronto Fell Out's own secret-ending taxonomy is populated (see `Storyline/Endings/Secret-Endings/Secret_Endings_Design_Framework.md`), this is where a Minmax-specific ending's actual trigger would be documented, subject to the same **World Trigger law** as every other secret ending — a discoverable physical object or location, never a hidden stat check or NPC-initiated approach.
- **`Unique_Interactions_-_High.md`** — special interactions available across Toronto Fell Out's (currently nonexistent) districts/locations when all three of this build's defining stats are high, in the same "minimum 5 per location" density as Inner Tepenia's own samples.
- **`Unique_Interactions_-_Low.md`** — the inverse: special interactions for the same three stats all sitting low (an underdog/unlucky variant, distinct from the single-stat-low flavor in `Single-Stat_-_Min.md`).

**Do not populate any of these for real yet.** Two blockers stand in the way, independent of each other: the Luck/Utility combinatorial question above, and the fact that Toronto Fell Out has zero designed districts, factions, or NPCs for "per-location interaction" and "NPC trigger" content to reference (see the project's own ground rule against inventing that content ahead of time). Once both are resolved, this file set is the shape to build from.

---

## Summary of What's Actually Done vs. Open

| Item | Status |
|---|---|
| `Single-Stat_-_Max.md` | Rewritten for MAPLE-BUD — done |
| `Single-Stat_-_Min.md` | Rewritten for MAPLE-BUD — done |
| Luck/Utility inclusion in the 3-stat scheme | **Open — flagged for the user, not decided here** |
| MAPLE-BUD-initial folder-naming convention | Described above, not yet applied (depends on the open question) |
| The 35 existing `##-XXX` folders | Left as-is, flagged stale/pending-rename, not renamed or repopulated |
| Per-folder file set (4 files) | Template documented above, not populated |
