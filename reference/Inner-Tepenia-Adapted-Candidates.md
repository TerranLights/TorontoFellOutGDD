# Perk/Trait Candidates Adapted from Inner Tepenia

Perks and traits surveyed from the Inner Tepenia GDD (a sibling project premised on playing a freshly-created robot) that look adaptable to Toronto Fell Out's human, real-time 1st-/3rd-person setting. See `player mechanics/Design-Philosophy.md` for the process rules pulled from the same source.

**Combat-system caveat**: Toronto Fell Out is a real-time 1st-/3rd-person open-world game, not turn-based. Inner Tepenia's combat perks are built around a turn-based AP economy. Anything below flagged ⚠ was originally an AP/turn-based mechanic and needs to be cross-checked against how Fallout: New Vegas or Fallout 4 actually implement the equivalent in real time (V.A.T.S., stamina/AP-for-sprint-and-power-armor, real-time aim/hit resolution) before it gets built — don't port the AP framing directly.

**Setting note**: Toronto Fell Out has no sentient robots/androids (unlike Inner Tepenia, where the player character is one). It may have non-sentient automated defenses roughly analogous to Fallout's Securitrons and Sentry Bots. That means Fallout's own vanilla robot-combat perks (e.g. the FNV `Robotics Expert` already in `to-be-integrated/Fallout_New_Vegas_-_perks_-_full-list.md`) apply directly, and Inner Tepenia's own robot-combat additions below are also fair game — they were written for fighting non-sentient robotic/automated enemies, not for robot player-companions, so nothing about them assumes a sentient-robot setting.

**Fallout-Adapted Traits reconciliation**: we already have all 16 vanilla FNV traits in `to-be-integrated/Fallout_New_Vegas_-_traits_-_full-list.md`. Inner Tepenia had 3 of those permanently blocked because of its robot premise — none of those blockers apply to a human game:
- **Four Eyes** (+Perception wearing glasses, -1 permanent otherwise) — Inner Tepenia needed to invent a robot optical-augmentation slot for this to make sense; a human just wears glasses. Works immediately, zero rework needed.
- **Early Bird** (day/night-dependent stat swing) — only needs a day/night cycle, which an open-world game almost certainly has anyway.
- **Logan's Loophole** (chems last longer, addiction zeroed, level cap locked) — needs an addiction mechanic, which Fallout-style chems already assume exists.

One genuinely new trait (not in real FNV) is worth pulling in alongside Claustrophobia: **Agoraphobia** — the exact mirror (+1 to all stats indoors, -1 outdoors), added by Inner Tepenia's own dev as a requested counterpart to Claustrophobia. Zero rework needed.

**Limb-specific damage/crippling — confirmed planned.** Small Frame's penalty (25% extra limb damage) and the Adamantium Skeleton/Eye for Eye perks (`to-be-integrated/Fallout_New_Vegas_-_perks_-_full-list.md`) all depend on a limb-specific damage/crippling system, same as Fallout has — confirmed as a real system Toronto Fell Out will build, not just decorative flavor text. All three are locked in as import targets; see `TODO.md` for the system itself.

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

## Perks — Robot/Automated-Defense Combat (confirmed applicable)

Written for fighting non-sentient robots/automated defenses — directly relevant now that Toronto Fell Out has Securitron-/Sentry-Bot-style enemies. All ⚠ flagged for the same AP-vs-real-time conversion as above.

- ⚠ **Electronic Disruptor** — EMP and electronic attacks have higher success rates and longer effect durations. Higher rank: a successful electronic attack can chain disruption to one adjacent electronic target at no additional cost.
- ⚠ **Electronic Warfare** — Direct, reliable disruption of enemy electronics and robotic systems in the field, beyond what a single Electronic Disruptor-style trick can manage alone.
- ⚠ **Chain Protocol** — Critical hits on robot enemies have a significantly higher chance to trigger cascade failures; a cascade can spread from the struck component to one adjacent system.
- Inner Tepenia's own rework of **Robotics Expert** (+25% damage against automated defenses; non-alerted automated defenses can be shut down rather than destroyed by sneaking up and deactivating them directly) is functionally identical to FNV's original — no new content here, but confirms the FNV version needs no trimming for this setting.

## Reskin-With-Tweaking Candidates

- **Reclaimer's Hands** (trait pattern) — "Descended from someone who could actually operate/understand pre-collapse tech, giving a bonus specifically on pre-War systems." Strong thematic fit for Toronto Fell Out — reskin as descending from a pre-War engineer, TTC maintenance worker, or similar.
- **District Capstone perk pattern** — Each of Inner Tepenia's 12 districts resolves its capstone questline into exactly 2 mutually exclusive perks tied to a real ideological choice (e.g., integrate-and-reform vs. enforce-strict-oversight, each with genuinely different combat/utility/social effects). The content (astrology-named districts) doesn't port, but the structure maps cleanly onto Toronto's own boroughs/factions/districts.
- **Zukelli Native-style hyper-specific unlock** — A single very high stat/skill threshold (e.g., two skills at 10, two stats at 6+) plus a personal favor to one named NPC, granting safe passage with an entire in-world group and unique dialogue tied to that connection. Good pattern for a signature "you really committed to this path" unlock tied to a specific Toronto location or community.
- **Cold-Blooded Optimizer** (trait) — Crafting/chemistry bonus plus reduced material cost, at a social-stat penalty. The specific compound it references ("siligel") is Inner Tepenia-specific, but the "efficient, cold, calculating crafter" archetype reskins cleanly onto whatever chem/crafting system Toronto Fell Out builds.
- **Ripple Intuitive** (trait) — Bonus reading a volatile/escalating situation, plus a bonus exploiting environmental hazards triggered in combat (fire, explosives, hazardous terrain), at a penalty under high stress. "Ripple" is Inner Tepenia's power-grid-crisis term specifically, but the underlying archetype — a crisis-reader who turns chaos into an advantage — is generic.
- **All-In Brawler** (trait) — Massive Might-scaled bonus damage on power/charged melee attacks, at the cost of a much worse post-attack vulnerability window. Portable only if Toronto Fell Out ends up with an equivalent charged/heavy-attack melee system (both FNV and Fallout 4 have some version of this).
- ⚠ **Engine Overclocker** (trait) — Emergency AP-burst: once per combat, gain temporary AP when at 0, followed by a burnout penalty (temp stat loss) for the rest of the encounter. Same AP-vs-real-time caveat as the perks above — the "spend a resource for a burst, pay for it after" shape is worth keeping, the AP framing isn't.

## Traits — Port With Just a Name Change

- **Lattice Mind** — Bonus to repair/jury-rigging on improvised gear, at the cost of a penalty elsewhere (originally a Hacking-adjacent tradeoff).
- **Empathic Bridge** — Bonus to de-escalation dialogue, at a physical-stat cost.
- **Narrative Ghost** — Bonus to Deception/rumor-probing dialogue, a once-per-act retroactive reputation-consequence erasure, and a permanent reduction to negative reputation gain, at a social-stat cost. A strong "information broker who leaves no trace" identity with no robot-specific content.
- **Cut Losses** — Zero-cost fleeing and a once-per-encounter auto-survive-lethal-hit effect, at the cost of permanently halving companion affinity/bond gain. A clean "self-preservation over loyalty" archetype.
- **Greener Pastures** — Flat, unconditional bartering bonus, at the cost of a hard cap on how high one district's reputation can ever go. Notable design lesson from Inner Tepenia's own revision history: every *conditional* version of this trait (novelty flags, time-based cooldowns) broke under scrutiny/exploits, and they settled on an unconditional flat effect instead — worth keeping in mind when designing Toronto Fell Out's own traits.
- **Fists First** — Bonus damage on the opening attack of combat, at the cost of losing de-escalation dialogue options entirely.
- **No Mercy** — A deliberate asymmetric crit bonus: +20% crit chance/+50% crit damage against robots, +40% crit chance/double crit damage against humans. Cost: in already-tense/hostile scenes involving a human, any violent dialogue option auto-fires with no player choice. Since Toronto Fell Out does have robotic enemies, both halves of the asymmetry apply as designed — no trimming needed.
- **Agoraphobia** — +1 to all stats indoors, -1 outdoors. The direct mirror of Claustrophobia (already in our FNV trait import); see the reconciliation note above.
- **Frontier Hardened** — Bonus to Survival/Outdoorsman-type effectiveness outdoors, plus a bonus to field repairs made away from proper facilities, at a penalty indoors. Generic frontier-survivor archetype — a strong fit given Toronto Fell Out's ruined-outdoors/wilderness content.
- **Humanity Anchor** — Bonus reading the active companion specifically, plus faster companion bond-building, at a skill-gain penalty elsewhere. Generic companion-focused roleplay trait, no robot content.
- **Undergrid Phantom** — Repair bonus plus a Sneak bonus specifically in low-light/underground environments, at a physical-stat penalty. Location-named ("Undergrid" = their setting's underground network) but renames trivially — a natural fit for Toronto's own PATH tunnels/subway/sewers.
- **Sonic Resonance** — Bonus to Speech/Narrative-type checks performing publicly, plus faster local reputation gain, at a physical-stat penalty. Generic performer archetype.
- **Demagogue** — Bonus to Speech/Narrative-type checks addressing crowds, at the cost of every NPC's first impression defaulting to skeptical/wary. Portable, contingent on Toronto Fell Out having enough crowd/group dialogue content for the bonus to matter.
- **Load-Bearing** — Flat +2 Might/-1 Agility. No content dependency at all; trivially portable.
- **Cold Calculation** — Flat stat trade (their Calculation/Humanity pairing reskins directly onto Brains/Determination: +2 Brains/-1 Determination). "Cold logic over social warmth" archetype.
- **Information Warfare** — Hacking-adjacent bonus, unlocks an action that exposes a target's weakness rather than dealing direct damage, at a social-stat cost plus a reputation cost when actually used. No robot-specific content.
- ⚠ **AP-Economy trait cluster** (High-Output Frame, Efficient Design, Overclocked Prototype, Fragile but Fast, Steady Nerves, Minimalist Frame, Echo Chamber) — all pure AP-economy tradeoffs (extra AP per turn, cheaper movement cost, front-loaded alpha-strike damage, etc.), with only cosmetic robot flavor text. The tradeoff *shapes* (extra resource now for a drawback later, cheaper stamina cost, etc.) are worth keeping, but need to be re-expressed in whatever real-time stamina/AP-adjacent system Toronto Fell Out ends up with (closer to Fallout 4's AP/sprint/power-armor model than to a turn-based economy) rather than ported as literal AP-per-turn numbers.

## Not Pursuing (Yet)

These are unfinished or blocked in Inner Tepenia's own file, not because of anything robot-specific — not worth chasing until they're resolved upstream (or we just resolve the same open question ourselves):

- **Bridge Feedback** — Investigation bonus while "jacked in," at a social-stat cost while jacked in. Needs their neural-interface ("Bridge Unit") mechanic; no equivalent in Toronto Fell Out unless we invent a hacking-rig/VR mechanic later.
- **["Broad Strokes" working title]** — Explicitly unfinished upstream: three bonus candidates floated (Speech, Survival/Outdoorsman, combat-initiative), none chosen. Penalty side (never notices small environmental details, hard override) is settled and portable whenever the bonus side gets picked.
- **One-Way Exchange** — Explicitly flagged as unresolved upstream due to a real production cost: it requires tagging which specific skill checks throughout the game use NPC-given information versus self-discovered information. Not worth taking on until that tagging cost is worth paying.
