# Perk/Trait Candidates Adapted from Inner Tepenia

Perks and traits surveyed from the Inner Tepenia GDD (a sibling project premised on playing a freshly-created robot) that look adaptable to Toronto Fell Out's human, real-time 1st-/3rd-person setting. See `player mechanics/Design-Philosophy.md` for the process rules pulled from the same source.

**Combat-system caveat**: Toronto Fell Out is a real-time 1st-/3rd-person open-world game, not turn-based. Inner Tepenia's combat perks are built around a turn-based AP economy. Anything below flagged ⚠ was originally an AP/turn-based mechanic and needs to be cross-checked against how Fallout: New Vegas or Fallout 4 actually implement the equivalent in real time (V.A.T.S., stamina/AP-for-sprint-and-power-armor, real-time aim/hit resolution) before it gets built — don't port the AP framing directly.

## Perks — Port Almost As-Is

- **Derelict's Eye** — Unlocked by finding and successfully restoring a genuinely derelict, pre-collapse structure (archaeological reclamation of something dormant since the war, not routine repair of functioning infrastructure — no quest marker points to it). Effect: permanent at-a-glance recognition of what any ruined pre-war structure originally was and what it'd take to restore it. Near-perfect fit for a ruined 2097 Toronto as-is.
- **Silver Tongue** — Persuasion checks get a flat bonus; a higher rank grants a retry after a failed check.
- **Lie Detector** — Always know when an NPC is lying; choose to call it out or hold it as leverage.
- **Fly on the Wall** — Witness an event unseen, then make NPCs forget you were there.
- **Diplomat** — Treated as a legitimate party (not a messenger) in formal negotiations.
- **Ferocious Loyalty** — When the player drops below 50% HP, active companions gain a defense bonus. (Originally an FNV port already.)
- **Last Stand** — A generic "second wind"/refuse-to-go-down mechanic; only the flavor text ("refuses to go offline") was robot-specific.
- **Jury Rigging** — Repair any item using a roughly similar item. (FNV original.)
- **Thermal Engineer** / **Power Grid Manager** / **Precision Maintenance** — Technical/engineering perks around crafting, repair quality, and utility-system upkeep. Generic crafting-skill content, directly relevant to Toronto Fell Out's Utility skill.
- **Junk Rounds** / **Vigilant Recycler** / **Mad Bomber** — FNV-original crafting perks (scrap ammo crafting, ammo-recovery-from-energy-weapons, explosive recipes).
- **Field Repair Protocols** — Emergency mid-combat self-repair, no workbench needed. Reskin as a mid-combat first-aid/stimpak-style perk for a human character.
- ⚠ **AP-based reworks of FNV combat perks** (Quick Draw as 0-AP draw, Nerves of Steel as AP-banking, etc.) — useful as a *reference for how Inner Tepenia converted FNV's real-time perks into turn-based ones*, but for Toronto Fell Out we want the reverse direction: start from FNV/Fallout 4's original real-time implementations of these same perks (Quick Draw's actual equip-speed bonus, Nerves of Steel's actual AP-regen rate in V.A.T.S., etc.) rather than Inner Tepenia's turn-based versions.

## Reskin-With-Tweaking Candidates

- **Reclaimer's Hands** (trait pattern) — "Descended from someone who could actually operate/understand pre-collapse tech, giving a bonus specifically on pre-War systems." Strong thematic fit for Toronto Fell Out — reskin as descending from a pre-War engineer, TTC maintenance worker, or similar.
- **District Capstone perk pattern** — Each of Inner Tepenia's 12 districts resolves its capstone questline into exactly 2 mutually exclusive perks tied to a real ideological choice (e.g., integrate-and-reform vs. enforce-strict-oversight, each with genuinely different combat/utility/social effects). The content (astrology-named districts) doesn't port, but the structure maps cleanly onto Toronto's own boroughs/factions/districts.
- **Zukelli Native-style hyper-specific unlock** — A single very high stat/skill threshold (e.g., two skills at 10, two stats at 6+) plus a personal favor to one named NPC, granting safe passage with an entire in-world group and unique dialogue tied to that connection. Good pattern for a signature "you really committed to this path" unlock tied to a specific Toronto location or community.

## Traits — Port With Just a Name Change

- **Lattice Mind** — Bonus to repair/jury-rigging on improvised gear, at the cost of a penalty elsewhere (originally a Hacking-adjacent tradeoff).
- **Empathic Bridge** — Bonus to de-escalation dialogue, at a physical-stat cost.
- **Narrative Ghost** — Bonus to Deception/rumor-probing dialogue, a once-per-act retroactive reputation-consequence erasure, and a permanent reduction to negative reputation gain, at a social-stat cost. A strong "information broker who leaves no trace" identity with no robot-specific content.
- **Cut Losses** — Zero-cost fleeing and a once-per-encounter auto-survive-lethal-hit effect, at the cost of permanently halving companion affinity/bond gain. A clean "self-preservation over loyalty" archetype.
- **Greener Pastures** — Flat, unconditional bartering bonus, at the cost of a hard cap on how high one district's reputation can ever go. Notable design lesson from Inner Tepenia's own revision history: every *conditional* version of this trait (novelty flags, time-based cooldowns) broke under scrutiny/exploits, and they settled on an unconditional flat effect instead — worth keeping in mind when designing Toronto Fell Out's own traits.
- **Fists First** — Bonus damage on the opening attack of combat, at the cost of losing de-escalation dialogue options entirely.
- ⚠ **AP-Economy trait cluster** (High-Output Frame, Efficient Design, Overclocked Prototype, Fragile but Fast, Steady Nerves, Minimalist Frame, Echo Chamber) — all pure AP-economy tradeoffs (extra AP per turn, cheaper movement cost, front-loaded alpha-strike damage, etc.), with only cosmetic robot flavor text. The tradeoff *shapes* (extra resource now for a drawback later, cheaper stamina cost, etc.) are worth keeping, but need to be re-expressed in whatever real-time stamina/AP-adjacent system Toronto Fell Out ends up with (closer to Fallout 4's AP/sprint/power-armor model than to a turn-based economy) rather than ported as literal AP-per-turn numbers.
