# Design Philosophy

Ground rules adopted for Toronto Fell Out, ported directly from Inner Tepenia's design-methodology documents (`Skills_Review_-_Verb_vs_Noun_Audit.md`, `Skill_Caps_and_Stat_Synergy.md`, `Skills.md`, `Perk_Framework.md`). These are process rules, not specific content — none of them are turn-based/AP-specific, so they apply as-is to a real-time 1st-/3rd-person game.

## Verb-vs-Noun Skill Audit

A skill must be a **noun** — a stable domain a character can invest in over an entire career — not a **verb**, a one-off action or technique the player performs.

When laying out Toronto Fell Out's skill list, run every candidate skill through this test: "is this a domain someone builds a career around, or is it really a specific move?" Verb-shaped entries (e.g., a specific action like "disarm this trap" rather than a domain like "Traps/Security") get cut or converted into a perk instead of a skill.

## Skill Cap Formula

```
Skill Maximum = 30 + ((Governing Stat Value − 1) × 10)
```

A stat of 1 hard-caps its governed skills at 30; a stat of 8+ is required to reach a skill cap of 100. This fixes the classic problem where a character with a dump-stat in the relevant attribute (e.g., 1 Brains) can still grind a governed skill (e.g., Repair) all the way to 100, becoming a world-class expert despite being mechanically established as bad at that domain.

Temporary bonuses (skill books, chems/consumables, equipment) may push a skill *above* its permanent cap situationally, without raising the underlying cap itself.

## Flat Thresholds, No Dice Rolls

No RNG on any skill/stat check, anywhere — every non-combat gate is binary met/not-met. A companion's skill doesn't grant the player a bonus roll; it lowers the effective detection/success floor while that companion is present.

**Real-time adaptation note:** this rule governs *skill checks* (lockpicking difficulty, dialogue gates, hacking access, environmental interaction), not moment-to-moment combat. Combat itself — being real-time 1st-/3rd-person rather than turn-based — should follow Fallout: New Vegas / Fallout 4's precedent instead: real-time aim/hit resolution, with stat/skill influencing damage, spread, and any V.A.T.S.-style assisted-targeting mechanic, rather than an abstract turn-based hit-chance roll.

## Minimum Five Solutions

Every quest, and every non-story-gated skill check, should have **at least five** distinct ways to pass it — raised deliberately above Fallout: New Vegas's own three-solution target. A "solution" can be: a skill threshold, a specific perk, a stat threshold, a companion's presence, a prior quest/reputation decision, or a substituting item. (Fallout: New Vegas's *Honest Hearts* weight-limit scene, with six solutions, is a good density reference.) Story-gated content is exempt from this rule.

## Perk Design Laws (from Perk_Framework.md)

- **No Good Endings**: every branch of a mutually-exclusive companion/quest resolution must carry a genuine cost. No branch should read as a clean win. (Modeled on Fallout: New Vegas's "For Auld Lang Syne"/Arcade Gannon resolution.)
- **Dual-Outcome Companion Perks + Companion-Mediated Access**: a companion questline resolves into 2+ mutually exclusive companion perks, each of which determines a paired player perk — the player's reward is downstream of the companion's outcome, not chosen independently. Separately, each branch should also unlock exclusive world access (a location/faction/group) mediated through that companion, distinct from the perk itself.
- **Branch count policy**: 2 branches is the floor, 3 is the default target to aim for, 4 is permitted when genuinely earned by the material, 5 is a hard cap. Don't force extra branches just to hit a number.
- **Specificity**: perk effects must be concrete (never "combat improved").
- **Ranks must change behavior**, not just rescale a number.
- **Mutual exclusivity must be genuinely balanced** — if one branch of a mutually-exclusive choice is clearly worse, the design has failed.
- **Fallout Precedence**: where a perk's territory overlaps with an existing Fallout: New Vegas or Fallout 4 perk, treat that game's implementation as the default reference point, and only design freely where it's genuinely new ground.
