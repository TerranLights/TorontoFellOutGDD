# TODO

Organized by priority tier, adopted 2026-07-29 (modeled loosely on Inner Tepenia's own TODO.md tiering — see that file for what to avoid: declared item scoped there but never consistently enforced, so items just piled up forever). **Keep `DONE.md` current** — move an item there the moment it's resolved, don't leave it checked-off-but-inline in any tier below.

## Blocking / Decisions Required

Core decisions that a lot of other design work depends on — resolve these before building much further on top of them.

- [ ] **Decide the main storyline's real objective**, revealed after the CN Tower/radio "false victory." Four candidate directions drafted (quarantine reveal, awakened automated defense system, buried pre-war asset, rival frequency-user faction), plus a proposed combined structure weaving all four together. Still fully open: what the buried asset actually is, who's enforcing the quarantine, the automated system's original standing orders, and who the rival faction turns out to be. See `Reference/Main-Storyline-Candidates.md`.
- [ ] **Figure out who's enforcing the quarantine** (Option 1 of the main storyline candidates). Narrowed by the confirmed Great Lakes DMZ placement: whichever successor polities actually border the region (Quebec and the People's Democratic Republic of New England are the most geographically obvious candidates; the Midwest Republic is also plausible) are the natural shortlist, jointly or otherwise — still needs an actual decision. This is the central antagonist question for the whole main storyline. See `Reference/Main-Storyline-Candidates.md`.
- [ ] **Decide the player's "immediate-immediate-immediate" opening goal** — the Goodsprings/Doc-Mitchell-equivalent hook that comes *before* the CN Tower climb and organically leads the player toward it. The CN Tower is a mid-early-game landmark (roughly FNV's Novac/REPCONN beat), not the literal opening — see the structural clarification in `Reference/Main-Storyline-Candidates.md`, cross-referenced against `to-be-integrated/New_Vegas_plot-beat_reference.txt` (a general FNV beat-by-beat reference kept on hand for these analogies).
- [ ] **Design a real-time stamina/resource system for combat.** Blocks several traits/perks held as concepts pending this: **Cut Losses**, **Adrenaline Engine**, **Last Stand**, the whole **AP-Economy trait cluster** (7 traits), and (separately) **All-In Brawler** needs an equivalent charged/heavy "Power Attack" melee mechanic. See `Game-Mechanics/Character-Creation/Traits.md` and `Game-Mechanics/Perks/Perks.md`.

## High Priority

- [ ] Flesh out the mechanics for each skill's uses, applications, and checks. Start with the skills under **Utility**:
  - [ ] Repair quality
  - [ ] Crafting recipes
  - [ ] Trap disarming
  - [ ] Jury-rigged weapon mods
  - [ ] etc.
- [ ] **Review and decide** on a hidden-system replacement for Karma (no Karma, no Sanity — something thematically native to this game). Four candidates drafted — Cohesion, Frost/Thaw, Grace, Static — see `Reference/Hidden-System-Candidates.md`. Once decided, update every remaining "Karma" mention in `Game-Mechanics/Perks/Perks.md`: the Level 50 perk trio (Ain't Like That Now, Just Lucky I'm Alive, Thought You Died) plus **Cannibal** and **Ghastly Scavenger**, all still using Karma verbatim from the FNV import.
- [ ] **Design the quarantine-perimeter-as-map-boundary mechanic** (confirmed direction): the open world's actual edge-of-map implementation IS the quarantine perimeter — checkpoints, patrols, getting shot at if the player tries to leave, no invisible walls or impassable-terrain excuses. Needs real design: how the boundary is detected, what the checkpoint encounters actually look like, whether it's escalating warnings before lethal force or immediate. See `Reference/Main-Storyline-Candidates.md`.

## Medium Priority

- [ ] Design the limb-specific damage/crippling system (confirmed planned — a real Fallout-style mechanic, not just flavor text). Needed to make **Small Frame** (trait), **Adamantium Skeleton**, and **Eye for Eye** (perks) actually functional rather than decorative. See `Game-Mechanics/Perks/Perks.md` and `Game-Mechanics/Character-Creation/Traits.md`.
- [ ] **Name Toronto Fell Out's own terminology** for several confirmed-to-exist-but-unnamed concepts currently left as Fallout placeholders in `Game-Mechanics/Perks/Perks.md`: the V.A.T.S.-equivalent targeting system, the Stimpak-equivalent healing item, and the default in-world currency (plus deciding on the tentative "Canadian Tire money" secondary currency). See `Reference/Open-Worldbuilding-Decisions.md`.
- [ ] **Decide Toronto Fell Out's own bestiary** for creatures/items currently assuming Fallout's own monster roster in `Game-Mechanics/Perks/Perks.md` (Ghastly Scavenger, Purifier, Mile in Their Shoes, Them's Good Eatin'). Ghouls are confirmed in-setting; super mutants, centaurs, night stalkers, spore plants/carriers, and deathclaws are still open. See `Reference/Open-Worldbuilding-Decisions.md`.
- [ ] **Start designing actual characters/companions** once ready — `Game-Mechanics/Core-Mechanics/Companion-System.md` and `Game-Mechanics/Core-Mechanics/Reputation-System.md` establish the general rules (Double Gate romance, Forbidden Traits, Personal Questline Design Rule, Wild Child routes, reputation tiers) but there's no cast yet to apply them to. Includes designing **Muttchow** (the confirmed non-human/creature companion slot's signature character — Toronto Fell Out's own Dogmeat/Rex).
- [ ] **Decide the Minmax-Builds stat-combination scope**: keep the pool at 35 combinations (matching Inner Tepenia's 7-stat MACHINE scheme, excluding Luck and/or Utility) or expand to 56 (all 8 MAPLE-BUD stats)? See `Storyline/Minmax-Builds/README.md`.
- [ ] **Decide what to do with the 35 stale MACHINE-coded `Storyline/Minmax-Builds/` subfolders** (01-MAC through 35-INE) — leave them in place as clearly-flagged-stale dead weight until the stat-combination scope above is decided, or move them into `Original-Basis-Materials/` now to declutter the live tree?
- [ ] **Fold two new design principles into `Game-Mechanics/Core-Mechanics/Companion-System.md`**, surfaced while stripping `Worldspace/Design_Principles.md`'s Post-Romance Mini-Questline section: (1) chosen vulnerability vs. stress vulnerability (a companion *choosing* to be unguarded reads categorically differently from breaking down under pressure), (2) relational conflict rather than external conflict (post-romance content can put the relationship itself at the center instead of needing an external threat/mystery).

## Long-Term / Low Urgency

- [ ] Once Toronto Fell Out's own factions/districts are designed: reskin **Fight the Power!** and **Sneering Imperialist** (perks currently reference NCR/Legion/Brotherhood of Steel and generic tribal/raider factions) onto real in-world factions.
- [ ] **Decide whether Toronto Fell Out wants a "bypass the main crisis" secret-ending category**, analogous to Inner Tepenia's Hidden Paths (e.g. a way to sidestep the main storyline's central conflict entirely). See `Storyline/Endings/Secret-Endings/Secret_Endings_Design_Framework.md`.
- [ ] **Design mechanics for the 8 candidate perk names** logged in `Game-Mechanics/Perks/Perks.md`'s "Candidate Perk Names" section (Wirehead, Junk Whisperer, Scrap Savant, Steady Voice, Soft Hands, Talk 'Em Down, Ghostwriter, Whisper Network, No Trace, Tether, Ride or Die, Steadying Presence, Cold Logic, Clinical Mind, Storm Sense, Chaos Reader, Redline, Bush-Hardened) — names only reserved so far, no mechanics designed.
- [ ] **Name the AP-Economy trait cluster** (`Game-Mechanics/Character-Creation/Traits.md`) — several use robot-chassis language ("Frame," "Prototype") that won't suit a human character; revisit alongside the real-time stamina/resource system design above.
- [ ] **Revisit "Adrenaline Engine"'s name** — flagged during the 2026-07-29 renaming pass since "Engine" still echoes an Inner Tepenia MACHINE stat name; kept for now, not fully settled.

## Done
Resolved items are archived in `DONE.md`, not kept inline here.
