# Companion System

Adapted from Inner Tepenia's companion system as a set of general design principles. Toronto Fell Out has no ready-made characters or companions yet, so nothing here is tied to a specific roster — this file establishes the rules the eventual cast will be built against. Stat/trait references use [MAPLE-BUD](../to-be-integrated/not-SPECIAL.md) in place of Inner Tepenia's MACHINE system.

**Deliberately not carried over:**
- **The Fragmentation Matrix** (Bond/Grief tracking tied to a re-spec/"Identity Fragmentation" mechanic) — Toronto Fell Out has no re-speccing, so the entire system it depends on doesn't apply.
- Inner Tepenia's specific cast, its always-present hologram companion (Calethina), its Zodiac-district roster distribution, and its DLC-specific companion-allocation rules — all tied to content Toronto Fell Out doesn't have (yet, or possibly ever).
- The **Reputation System** these principles lean on (Wild Child, faction/district standing) has its own file: `Reputation-System.md`.

---

## Party Composition

**Open question, not yet decided:** Inner Tepenia uses a single companion slot, justified specifically by an always-present secondary character (Calethina) that already gave the player a second relationship at all times — without an equivalent, that justification doesn't automatically carry over. Two shapes are worth weighing:
- **Single companion slot** (Inner Tepenia's model) — simpler, makes each companion choice a stronger individual commitment.
- **Fallout: New Vegas's model** — one humanoid companion + one non-humanoid (creature) companion simultaneously (e.g., Dogmeat/Rex). Worth considering if Toronto Fell Out wants a companion-animal alongside a human companion.

Whichever is chosen, the underlying design rationale should still hold: preserve a protagonist-with-support feel rather than a full multi-character party, and recruiting a new (human) companion requires dismissing the current one.

## Companion Slot Rules

- Dismissing a companion returns them to a fixed location in the world (they do not disappear from it).
- Dismissed companions retain all relationship progress and questline state.
- A companion's personal questline can only advance while they are the active companion.
- Re-recruiting a dismissed companion is always available unless a specific story event has permanently changed their status.

## Major NPCs Who Are Not Companions (pattern)

Not every character with a deep, consequential relationship to the player needs to occupy the companion slot. A character can have a complete questline and a real ongoing relationship with the player expressed through some other recurring mechanic instead — a radio show that reacts to how their questline resolved, a shop or fixed establishment they run, a recurring location the player revisits. This is a legitimate design pattern, not a fallback for characters who "don't fit" as companions — reserve it for characters whose payoff genuinely depends on staying anchored to a role or place rather than joining the party.

## Combat Interaction — Applying Healing Items to a Companion

Ported directly from Fallout: New Vegas. The active companion's interact wheel includes a healing-item option that displays their current HP; selecting it consumes one of the player's own healing items (Toronto Fell Out's own Stimpak-equivalent — name TBD, see `reference/Open-Worldbuilding-Decisions.md`) to heal them directly. This is a manual, player-initiated action, distinct from any passive regeneration effect a perk or trait might separately grant.

---

## Romance: The Double Gate

Romance requires two independent conditions to be met simultaneously. Failing either one closes the route.

**Gate 1 — Questline prerequisite:** the player must have completed the relevant relationship-building questline content with this character. The relationship has to be built through shared experience and choices, not just dialogue options. Same for all characters.

**Gate 2 — MAPLE-BUD stat/trait threshold:** each character has a specific profile of what they find attractive, derived from their personality, sensibilities, and history. The player's stats and traits must meet that profile. Unique per character.

- **Perks are explicitly excluded from Gate 2.** Stats and traits are chosen at character creation — they define who the player character fundamentally *is*. Perks are acquired through play — what the character has learned and done. The romance gate is about identity, not accumulated experience.
- **Gate 2 checks permanent base stats only — not temporary boosts.** Food, chems, equipment, or any other time-limited effect don't count. Permanent increases (from character creation or gameplay means such as the Intense Training perk) count in full.
- **Gate ordering:** Gate 1 always comes before Gate 2. The companion quest completes first; the stat check fires second, at the first organic moment the character would naturally move toward romance. If the build meets the threshold, the romance beat sequence begins. If not, the signal line (below) fires and the door closes for that playthrough — but the relationship itself doesn't end.

### Threshold Design Per Character

When designing each romanceable character, specify:
- Which MAPLE-BUD stat(s) are required and at what level.
- Which traits are **forbidden** for this character (see Forbidden Traits below).
- The in-world rationale — what this person finds attractive and why, grounded in their personality.

Examples of how thresholds might read:
- A character who values physical presence → Might threshold
- A character who values intelligence and wit → Brains threshold
- A character who values genuine emotional depth → Determination threshold
- A character who admires courage and directness → Endurance threshold (or Might, depending on flavor)
- A character who values perceptiveness → Perception threshold
- A character who values capability and reliability → Endurance threshold

Multiple stats may be required.

### Forbidden Traits — A Categorically Different Gate

Each romanceable character has **1 to 3 forbidden traits** — specific traits from the full trait pool (`Traits.md`) that, if the player selected them at character creation, permanently disqualify that character's romance route.

**Why this is categorically different from a stat threshold, not just a variant of it:** a stat threshold represents growth — a player who falls short today can still reach it later. A forbidden trait represents an unchangeable character-creation choice, permanent for the entire playthrough. **There is no path to growing out of a forbidden trait.**

**Design process for assigning them** (adapted from Inner Tepenia's Forbidden Trait Design Method):
1. Derive candidates only from three sources already established for that character: **personality**, **personal history**, and **personal sensibilities/professional instinct** — never invent a dealbreaker from nowhere.
2. Aim for **1–3 forbidden traits per companion, never pad to hit 3** — two precise, well-justified traits beat three where the third is a stretch.
3. **The same trait can be a dealbreaker for multiple companions for entirely different in-character reasons** — reuse is fine as long as each character's specific rationale is written out.
4. When nothing in the existing trait pool fits precisely, design a new trait — but ground it in something concrete and reusable beyond that one companion, not a bespoke one-off.
5. **Flag near-miss candidates rather than force them** — if a trait is thematically close but represents a genuinely different violation, name the overlap explicitly and let a human call it.

**Implementation precedence:** a forbidden-trait check is evaluated *first* and takes total precedence over the standard stat-gate display. If the player holds a forbidden trait, the game shows that character's own distinct rejection line instead of the normal passing/failing stat-check dialogue — the two never display simultaneously.

**A distinct tone:** forbidden-trait rejections read as a genuinely closed door — not a "not yet," but a "this isn't something that changes" — separate from the ordinary stat-threshold Signal below, which implicitly invites growth.

### The Signal

When a player has completed the questline prerequisite but does not meet the **stat** threshold (a forbidden trait is handled entirely separately and takes precedence), the character makes an honest, casual, in-voice remark that reveals what they're looking for — without breaking the fiction or explaining the system. Short, in character, closes the romantic door without closing the relationship.

Register examples (not final lines — written per character in voice):
- *"Sorry, friend. I like them smart."*
- *"Not trying to be rude here, but come back once you've lifted some weights."*
- *"You're good people. Just not my type."*

Delivered once, not repeated unless the player re-initiates. On a replay with a different build, the player who heard it knows what to work toward.

### Gate Display — Visible Stat Check

Romance gates use the same visible stat-check UI as every other stat check in the game (per `Design-Philosophy.md`'s Flat Thresholds rule) — no special UI treatment. Both the passing option and the failing option appear in dialogue simultaneously, regardless of whether the player meets the threshold.

- **Passing option:** all thresholds met — stats display in brackets, followed by the dialogue line.
- **Failing option:** one or more thresholds not met — failed stats display as [current/required], met stats display normally, followed by the Signal.

The visible failed threshold is what makes the Signal legible — the player can see exactly which stats they're short on and what to build toward on a replay.

### Romance Exclusivity — Monogamy Rule

General principle: **monogamy once a committed romance is established.**

**Before full romance:** the player can engage in casual encounters freely with a separate pool of sexually-available characters (minimal stat/quest gating, no full romance arc required), with no relationship consequences.

**Once the player has fully romanced one character:**
- Any subsequent sexual encounter — with a casual partner or by triggering a second full romance — starts a timer.
- After a set period *(placeholder — exact duration TBD)*, the romanced companion discovers it and reacts with fury; the romance perk is immediately lost. Total loss, no partial penalty.
- **Second full romance — symmetric loss:** if the player triggers a second full romance (not just a casual encounter), both characters find out and both romance perks are lost simultaneously.

### Sexuality — Canon Rule

**Human female characters (companions and sexually-available NPCs):** bisexual by default — pursue the player regardless of gender presentation.

**Human male characters (companions and sexually-available NPCs):** heterosexual, fixed-gender attraction — will only pursue a player character presenting as the gender they're attracted to.

**Mechanical consequence:** every romanceable companion still gates on the standard stat/trait check (Gate 2). On top of that, romanceable human male companions gate on an **additional gender check** — the player must be presenting as the gender he's attracted to, checked independently of and in addition to the stat threshold. Human female companions carry no such additional gate.

This applies uniformly across both the romance roster and the casual pool.

---

## Personal Questline Design Rule — The Player's Unique Capability

Every companion's personal questline should hinge on something the player is able to do that the companion herself cannot — not because she's incapable in general, but because the player has some specific access, standing, or capability she genuinely lacks. This gives the player real, active agency in resolving what the character can't resolve alone, rather than making the player a bystander who watches the companion's own resources solve her problem off-screen.

**Critical caution — the categorical block must come first.** A stat-based approach only satisfies this rule if the *category* of action is something the companion is structurally excluded from — by access, role, or history — not merely something the player happens to meet a higher threshold on. Establish why she structurally cannot engage with this at all before varying *how* the player succeeds.

**No single required stat, perk, or skill — minimum 5 viable stat-based approaches.** Whatever the final player-only step is, it must not be gated behind one specific stat, perk, or skill check — design at least 5 distinct approaches, ideally spread across different stats/skills, so that whatever the player invested in, at least one route is open. This is the same discipline as `Design-Philosophy.md`'s Minimum Five Solutions rule, applied specifically to companion-quest resolution.

**Plus non-stat, world-state-based approaches — target 7–12, absolute floor of 3.** Stat-based approaches alone can still soft-lock a player who built entirely outside the covered stats. Additional routes should key off something else the player can plausibly have going for them: faction/district reputation earned elsewhere (see `Reputation-System.md`), knowledge or an item gained from unrelated content, an ally/relationship that happens to be relevant. Every route must make sense within the character's established world — no route invented just to hit the number.

**Recommended pattern — reputation with a faction/district the companion herself is on bad terms with.** Where a companion has an established negative or wary relationship with a specific faction or district, one of her non-stat routes should ideally be the player's own *positive* reputation there (per `Reputation-System.md` — doesn't need to be Idolized, just genuinely positive) opening a door she couldn't open herself. Not a requirement for every companion — don't invent an antagonism just to satisfy this pattern.

**Recommended pattern — a Wild Child route.** Aim for at least one non-stat route usable specifically by a player who holds **Wild Child** status (Fame Range 3 + Infamy Range 3 simultaneously, per `Reputation-System.md`) with some relevant faction or district. Wild Child is rare by design and creates genuine, mechanically real gaps and anomalous access precisely because the holder can't be categorized by the normal reputation system. Like the pattern above, reach for it where it genuinely fits, not as a requirement for every companion.

**Vary the flavor.** Don't default to the same mechanical shape (e.g., "an institution can't file the player, so someone forced into individualized handling surfaces information as a side effect") for every companion. Established alternate flavors worth drawing on:
- **Gossip/rumor flavor** — the player becomes unavoidable talk in an informal information economy; what's being searched for surfaces as a byproduct of people talking, not any institution processing anything.
- **Confessional/psychological flavor** — a person or space built around sitting with irreconcilable truths engages with the player's own contradiction on its own terms.
- **Persuasion/leverage flavor** (modeled on Fallout: New Vegas's Arcade Gannon companion quest) — someone chooses to gamble on the player specifically *because* their unresolved, paradoxical reputation makes them a wildcard worth betting on, with the door left open to betray that arrangement later.
- **Fear/intimidation** — someone cooperates because refusing feels more dangerous than complying.
- **Opportunism** — someone tries to exploit the player's notoriety for their own ends, and the player can leverage that back.

When designing a new one, ask what kind of reaction *this specific* faction or district would actually have to an unresolvable contradiction, rather than reaching for the same default mechanic every time.

---

## Romance Reward — Companion Player Homes

**Romancing a companion unlocks that companion's personal home as a player home.** Universal for all romanceable companions. **Romance is the gate — a companion's home is not accessible to the player at any point before the romance is established.** Once confirmed, the home stays available for as long as the romance status is maintained.

**Home access is tied to romance status and is lost if the romance ends** — under the monogamy rule above, losing the romance perk revokes home access along with it. The home belongs to the companion; the player was a guest by virtue of the relationship.

Any content, beat, or interaction that requires the player to be inside a companion's home cannot be part of the pre-romance arc — it must be reserved for post-romance content.

Companion-unlocked homes exist **in addition to** the regular player homes available in the main game; they don't replace or supersede standard home options.

### Post-Romance Mini-Questline Reward: The Significant Object

The romance perk and home access are the rewards for establishing the romance. Completing a **post-romance mini-questline** — where one exists — carries a separate reward: a **physical object** of deep personal significance to the companion, given to the player because the relationship has reached a depth of trust where parting with it is possible.

This object is a **quest item**: it cannot be sold, dropped, lost, pickpocketed, or broken down. It's examinable in the inventory UI — selecting it produces a written description of what the object is and what it means that the companion gave it. It persists in the player's inventory for the remainder of the playthrough regardless of the subsequent state of the romance.

The object is not a perk. It confers no mechanical bonus. It's a record — a thing the player carries — of what the relationship became.
