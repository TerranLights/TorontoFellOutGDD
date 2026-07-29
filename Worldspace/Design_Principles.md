# World & Quest-Building Design Principles

This document records guiding principles that must be respected when building out main questlines, side questlines, faction content, world events, and character interactions. It is a living document — new principles are added as they are established. Existing principles are binding.

**Provenance note:** these principles were adapted from Inner Tepenia's own design-methodology documents. They are process rules, not specific content — none of them depend on Inner Tepenia's own cast, districts, or lore, so they carry over as binding law for Toronto Fell Out. Where the original included worked examples tied to Inner Tepenia's own characters or lore, those examples have been removed rather than replaced with invented Toronto Fell Out content — per this project's ground rule against inventing new characters, districts, or lore ahead of when they're actually designed.

## Related Reference Documents

**[Enneagram_Dynamics.md](Enneagram_Dynamics.md)** — The binding character behavior ruleset for all confirmed-type characters. Defines integration (behavior in good times) and disintegration (behavior under stress) directions for all nine types, with a per-character application table. Consult this document whenever writing: companion approval/disapproval responses, quest dialogue under stress, romance beat behavior, signal line design, or the emotional arc of any personal questline. It will be referenced constantly during quest design.

---

## I. Romance Questlines — Opportunity Distribution

### The Rule

For every romanceable character, and for every individual step (beat) of their romance sequence, the player must have **at minimum five distinct, plausible opportunities** to complete that beat during normal play.

**Why this rule exists:**

1. **Non-interruption of flow.** The player should never have to stop what they are currently doing, possibly travel across the map, and perform one specific action just to advance a romance beat. If a beat can only be triggered in one specific context, it becomes an interruption. If it can be triggered in five different contexts across the player's normal activity, it becomes something the player encounters naturally.

2. **Missed-but-not-failed beats.** A beat is "failed" only if the player actively does the wrong thing (e.g., pushing past what a character has offered, lying when the beat requires truth, backing down when the beat requires holding ground). A beat that the player simply hasn't encountered yet is not failed — it is waiting. The five-opportunity minimum ensures that a player who missed the beat in one context will encounter it again in another without having to track it deliberately.

**What counts as a distinct opportunity:** A different context, location, initiating condition, or in-game moment that could naturally produce the beat. Opportunities do not need to be identical in surface content — they only need to be internally consistent with the character and the beat type.

**What does not count:** Minor variations on the same single scenario. Five dialogue trees in the same conversation during the same quest moment are not five opportunities; they are one opportunity with branches.

### Application to Toronto Fell Out's Own Cast

Inner Tepenia's version of this file included a full set of per-character opportunity arrays — five or more concrete contexts documented for every beat of every romanceable character's arc. Toronto Fell Out has no designed companions or romanceable characters yet (see `Companion-System.md` and the project's zero-districts/zero-factions/zero-companions constraint), so there is nothing to populate here. Those arrays are not reusable as-is — they were written beat-by-beat against Inner Tepenia's own specific characters, districts, and questlines.

**When Toronto Fell Out designs its first romanceable character**, build that character's opportunity array directly under this section, following the same discipline: state each beat, then list five or more distinct context-types (not five variations on one scene) that could plausibly produce it during normal play. Revisit the arrays once actual questline content exists, to confirm the opportunities are still internally consistent with what got built.

---

## II. Romance Gate Visibility

**This section is intentionally short — the substance already lives in `Game-Mechanics/Core-Mechanics/Companion-System.md`**, under its "Gate Display — Visible Stat Check" heading. That section already correctly adapts this rule for Toronto Fell Out: romance gates use the same visible stat-check UI as every other stat check in the game (per this file's own Flat Thresholds rule in `Universal_Rules.md`/`Design-Philosophy.md`), both the passing and failing dialogue options are shown regardless of whether the player meets the threshold, and a failed check displays as [current/required] followed by the character's Signal line.

Consult `Companion-System.md` directly for the full rule, the design rationale (consistency, legibility of the Signal, replayability), and the Fallout: New Vegas precedent it's built on. Nothing further needs to be derived here — re-deriving the same rule in two files risked them drifting out of sync with each other as one gets edited and the other doesn't.

---

## III. Post-Romance Mini-Questlines

### Overview

A post-romance mini-questline is a short, focused arc that fires only after a romance has been fully established with a companion — after the romance perk has been granted and the companion's player home has been unlocked (see `Companion-System.md`'s "Romance Reward — Companion Player Homes" section). It is distinct from both the companion questline and the romance beat sequence itself. It is not a reward for completing the romance; it is content that is only possible *because* the romance exists.

This is not a common design pattern. Most games treat the romance as the destination and end there. The post-romance mini-questline treats the established relationship as a starting condition and asks what can be built from that foundation that couldn't have existed before it.

**Overlap note:** `Companion-System.md` already documents the mechanical reward for completing one of these — "Post-Romance Mini-Questline Reward: The Significant Object" (a protected, weightless, examinable quest item, never a perk). That reward mechanic is not repeated here. What follows are the guiding design *principles* for what the mini-questline's content itself should look like — material `Companion-System.md` doesn't yet cover.

### Guiding Principles

**1. The content must be only possible because the relationship exists — not merely gated by it.**

This is the foundational distinction. A gated beat is a locked door — any sufficiently credentialed player can open it. Post-romance content should be something that genuinely *could not have happened* before: either because the companion would not have permitted it, or because the physical space (the home) was not yet accessible, or because the specific trust required to receive this layer had not been built. If the content could plausibly have appeared in the pre-romance arc, it does not belong here.

**2. Chosen vulnerability, not stress vulnerability.**

The pre-romance arc can and often does show a companion breaking down under pressure — disintegration under stress (see `Enneagram_Dynamics.md`), a difficult quest beat, a moment the player witnesses rather than being given. Post-romance content should show something categorically different: the companion *choosing* to be unguarded. This is a distinct register. "You saw me at my worst" is stress vulnerability. "I am showing you this because I decided to" is chosen vulnerability. The post-romance mini-questline operates in the second register. A companion who has decided to open a door is doing something entirely different from one who had a door forced open by circumstances.

**3. Relational conflict rather than external conflict.**

Pre-romance questlines use external stakes — a faction threat, a mystery, a danger — to develop the relationship as a byproduct. A post-romance mini-questline can afford to put the relationship itself at the center. A disagreement. A discovery that complicates something between them. A moment where the player and companion want different things and have to navigate it as a couple. No external villain required. The relationship is both the subject and the arena.

**4. Deepens rather than resolves.**

Pre-romance has a clear destination: the romance. Post-romance has a different structure. The question is no longer "will this happen?" but "what does it mean that it did?" The arc should leave the player knowing something about the companion — or about the relationship, or about what the player's own character is to this person — that they did not know before. It does not resolve anything. It opens a new layer.

**5. Short, concentrated, emotionally dense.**

This is a *mini*-questline by design. One to three beats, not a second full companion arc. The compression is intentional — intimacy does not always require space to sprawl. A single domestic moment that opens something new can carry more weight than an extended sequence. The brevity is part of what distinguishes it from the pre-romance arc.

### Structural Template

While each companion's post-romance mini-questline will be unique to their character, the following sequence describes the general shape:

1. **Inciting access:** Something becomes visible, discoverable, or accessible from within the companion's home — or from within the new register of the relationship — that could not have been noticed before. Not a main-quest event. Something domestic, intimate, noticed. An object. A habit. Something the player sees now that they are here.

2. **The reveal:** Something about the companion's interior — a piece of their past, a thing they made or kept or lost, a thought they have been carrying — becomes available to the player. The companion offers it. Not because they were asked. Because they decided to.

3. **A moment of real chosen vulnerability:** The companion in a state they would not have permitted before the romance. Distinct from stress collapse — this is deliberate openness. The player must be present for it, not just witness it.

4. **The player's response:** A dialogue choice or a player action that determines how the player receives what they have been given. This is not a pass/fail gate. It shapes the texture of the relationship going forward.

5. **The relationship deepens.** No new status is conferred — the romance already exists. What changes is the quality of it. The player leaves knowing something they did not know when they arrived.

### Application

Post-romance mini-questline beats should be flagged as such in individual companion romance designs, documented separately from the main romance beat sequence, and never treated as prerequisites for the romance itself. They are content that the romance makes possible, not content that completes it. Not every companion needs one — only those whose character and backstory naturally support this layer.

Toronto Fell Out has no designed companions yet, so there is nothing to flag here. When a companion's post-romance mini-questline is designed, list it under this section along with a pointer to where its Significant Object reward is documented in that companion's own file.

---

## IV. Unmarked Discovery Content

### The Rule

**Any piece of lore large enough, cross-cutting enough, or personally connected enough to the player character's own origin must never be implemented as a quest, of any size, in any DLC or the main game.** No marked quest. No unmarked-but-tracked quest. No journal entry, no map marker, no XP, no quest-log listing of any kind. It is not an in-game feature — it is background lore, existing purely for a sufficiently diligent, patient, and curious player to piece together entirely through optional means (environmental storytelling, incidental dialogue, item and terminal descriptions, cross-referenced observation across multiple locations), with no game system ever pointing the player toward it or rewarding its discovery mechanically.

**Fallout: New Vegas precedent (binding):** modeled directly on FNV's own unmarked quests — content with no Pip-Boy listing, no map marker, and no XP reward, discoverable only by players who go looking without being told to. Inner Tepenia's own treatment of its equivalent piece of lore (the Cradle, a nationwide fabrication-synthesis-chamber network tied to its own player character's origin) went one step further than FNV's own unmarked quests: it wasn't tracked as an unmarked quest in the game's own systems at all. It was simply true, sitting in the world, for whoever found it. That same standard — not just unmarked, but untracked — is the target here.

**What this does and doesn't restrict:** this rule governs world-spanning lore of that scale specifically — its full shape, its historical lineage, and especially any link to the player character's own creation or origin. It does not restrict ordinary regional questlines that happen to touch related subject matter at a purely local scale (a threat to one district's own infrastructure or a personal mystery confined to one neighborhood, for instance, is legitimate quest material on its own local terms). What must never happen is treating the wider, world-spanning version of that lore as a directed, marked, or XP-rewarding quest objective anywhere in the game.

### Why

The reward for the player here isn't a perk, an item, or a stat boost. It's the reward itself: understanding something true and enormous about the world that the game never told them to go find. This is the same design register as the Significant Object reward in Section III above — a thing given because a certain depth of engagement was reached, not because a checklist was completed — extended here to a piece of world-lore rather than a companion relationship. Making a piece of world-spanning lore into a tracked quest, however minor, would convert the largest-scale, widest-reaching piece of lore in the entire game into a checklist item. Leaving it unmarked keeps it what it's actually meant to be: a reward for diligence, patience, and curiosity, available only to the player who exercises those things without being asked to.

### Application

**Toronto Fell Out doesn't yet have an equivalent piece of world-spanning lore to protect this way.** The buried asset under the CN Tower's false-victory hook (see `Reference/Main-Storyline-Candidates.md`, Option 3) is the closest current candidate — it's explicitly described there as "the unifying secret" behind multiple storyline threads — but what it actually is remains undecided, and nothing should be built or written against this rule until it's designed.

This principle is a template, not a one-off exception — whenever Toronto Fell Out designs a piece of lore this large, this cross-cutting, or this personally connected to the player character, it should default to the same unmarked-and-untracked treatment unless there's a specific reason to do otherwise.
