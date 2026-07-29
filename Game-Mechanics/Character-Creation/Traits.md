# Traits

Toronto Fell Out's trait list. Built in two layers: the full Fallout: New Vegas trait list as a foundation (SPECIAL wording updated to [MAPLE-BUD](../to-be-integrated/not-SPECIAL.md)), plus additional traits adapted from Inner Tepenia. See `Design-Philosophy.md` for the process rules these should follow going forward, and `reference/Inner-Tepenia-Adapted-Candidates.md` for the full survey this was drawn from.

**MACHINE → MAPLE-BUD translation used below**, applied case-by-case since the two stat systems don't align 1:1: Might→Might, Agility→Agility, Calculation→Brains, Investigation→Perception, Humanity→Determination, Nerve→Determination (fallback for incidental flat bonuses — dropped where it would double up with an existing penalty on the same stat), Engine→Endurance. Where a bonus targeted a specific skill (e.g. Insight, Hacking), it's translated to that skill's actual MAPLE-BUD governing stat instead (Insight→Perception, Hacking→Science/Brains) rather than the blanket rule above.

**Open items carried over from the source material:**
- ⚠ marks a trait whose effect was originally written for a turn-based AP economy (Inner Tepenia) and needs to be cross-checked against Fallout: New Vegas/Fallout 4's real-time equivalents before it's built.
- **Small Frame**'s penalty (25% extra limb damage) depends on the limb-specific damage/crippling system — confirmed planned, see `TODO.md`.
- **All-In Brawler** and **Engine Overclocker** are contingent on combat systems Toronto Fell Out hasn't designed yet (a charged/heavy "Power Attack" mechanic, and a stamina/resource system respectively) — held as concepts, not final numbers.

---

## Foundation: Ported from Fallout: New Vegas

**Built to Destroy**
- +3% critical hit chance.
- Weapon condition decays 15% faster.

**Claustrophobia**
- +1 to MAPLE-BUD attributes while outside.
- -1 to MAPLE-BUD attributes while indoors.

**Agoraphobia** *(new — direct mirror of Claustrophobia, added alongside it)*
- +1 to MAPLE-BUD attributes while indoors.
- -1 to MAPLE-BUD attributes while outside.

**Early Bird**
- +2 to MAPLE-BUD attributes from 6 a.m. to 12 p.m.
- -1 to MAPLE-BUD attributes from 6 p.m. to 6 a.m.

**Fast Shot**
- Guns and energy weapons you fire are 20% quicker; AP cost for your guns and energy weapons is 20% lower.
- Guns and energy weapons you fire are 20% less accurate.

**Four Eyes**
- +2 Perception when wearing glasses. Bonus does not apply when determining perk requirements.
- -1 Perception, permanent reduction. Penalty still applies when determining perk requirements.

**Good Natured**
- Increases Speech, Medicine, Repair, Science, and Barter skills by +5.
- Decreases Energy Weapons, Explosives, Guns, Melee Weapons, and Unarmed skills by -5.

**Hoarder**
- +25 lbs to total Carry Weight.
- -1 to MAPLE-BUD attributes while current equipment weight is below 160 lbs.

**Hot Blooded**
- +15% damage increase while below 50% health.
- -2 to Perception and Agility while below 50% health.

**Heavy Handed**
- Melee and unarmed do 20% more damage.
- Melee and unarmed do 60% less critical hit damage.

**Kamikaze**
- +10 Action Points.
- -2 Damage Threshold and -15% Damage Resistance.

**Logan's Loophole**
- Chems last twice as long and addiction rates are set to zero.
- Locks the level cap at 30.

**Loose Cannon**
- Attack speed with thrown weapons increased by 30%.
- Thrown weapons have 25% less range.

**Skilled**
- Gain +5 points to every skill.
- You suffer -10% from experience gained.

**Small Frame**
- +1 Agility.
- Fragile limbs (25% extra limb damage).

**Trigger Discipline**
- Guns and energy weapons you fire are 20% more accurate.
- Guns and energy weapons you fire are 20% less quick; AP cost for your guns and energy weapons is 20% higher.

**Wild Wasteland**
- Adds additional "wacky" content and modifies existing content and special encounters.
- Removes access to some "sane" content.

---

## Additional Traits (Adapted from Inner Tepenia)

**Lattice Mind**
- +20% Repair success on jury-rigged/patched-together equipment. Science (hacking) targets that are themselves improvised/non-standard systems require 1 tier lower access threshold.
- -1 Determination.

**Empathic Bridge**
- +20% Speech effectiveness in de-escalation/conflict-avoidance dialogue. +2 Determination.
- -1 Might.

**Narrative Ghost**
- +20% Speech effectiveness for deception and rumor-probing dialogue specifically. Unlocks an extra dialogue option to probe any NPC for rumors/information. Once per reputation-affecting act, retroactively erase that act's reputation consequence entirely — as though it was never traced back to you. Negative reputation gains permanently reduced by 25% across the board, stacking with the once-per-act erasure.
- -1 Determination ("harder to build genuine trust").

**Cut Losses** ⚠
- You can always disengage from combat freely, with no unusual penalty for fleeing *(originally "zero AP cost to flee" — needs a real-time equivalent, since fleeing already has no inherent action-cost in real time; the interesting clause is the one below)*. When reduced to 0 HP, instead of going down, automatically disengage from combat and survive at 50% HP instead — once per combat.
- The active companion's bond/affinity progress is permanently halved.

**Greener Pastures**
- +10% Barter effectiveness, always active, no trigger condition.
- Reputation with any single district/borough can never rise above "Liked" — the top tier is permanently locked out everywhere. *(Design note: every conditional version of this trait's bonus — novelty flags, cooldowns — broke under scrutiny in the source material; keep it a flat, unconditional bonus.)*

**Fists First**
- Attacks made as the opening action of combat deal +15% damage.
- De-escalation/conflict-avoidance dialogue options are never available in any conversation.

**No Mercy**
- +20% critical hit chance and +50% critical damage against robots. +40% critical hit chance and double critical damage against humans.
- In already-tense/hostile scenes involving a human, whenever a violent option exists, it automatically becomes the next step — no player choice at that point.

**Frontier Hardened**
- +20% Survival and Outdoorsman effectiveness while outdoors/away from settled areas. +15% Repair specifically on field repairs made away from proper facilities. +1 Endurance while outdoors/away from settled areas.
- -1 Determination while indoors/within settled areas.

**Humanity Anchor**
- +1 Determination. +20% Insight effectiveness specifically when interacting with the active companion. Bond/affinity progress with the active companion accelerates.
- -10% skill gain specifically in Science, Chemistry, and Energy Weapons.

**Tunnel Rat** *(renamed from Undergrid Phantom)*
- +20% Repair. +15% Sneak specifically in low-light or underground environments (subway, sewers, PATH tunnels).
- -1 Might.

**Sonic Resonance**
- +20% Speech effectiveness when performing publicly. Reputation gains in one district/borough of your choosing progress faster.
- -1 Might.

**Demagogue** *(production dependency: only meaningful if Toronto Fell Out has enough crowd/group dialogue content — not yet confirmed)*
- +20% Speech effectiveness specifically when addressing groups or public gatherings.
- Every NPC's first impression of this character defaults to skeptical/wary, regardless of stats.

**Load-Bearing**
- +2 Might.
- -1 Agility.

**Cold Calculation**
- +2 Brains.
- -1 Determination.

**Information Warfare** *(explicitly tentative upstream — not locked in)*
- +20% Science effectiveness. Unlocks a new offensive action, Data Leak — a debuff that exposes a target's weakness rather than dealing direct damage (temporary defense reduction, or disabling one of the target's tactical options for a short duration).
- -1 Determination. Using Data Leak costs reputation/standing with whoever gets exposed.

**Cold-Blooded Optimizer**
- +20% Chemistry effectiveness when synthesizing chems/compounds. -20% material cost when repairing/crafting via efficiency-optimized methods. +2 Brains.
- -2 Determination.

**Ripple Intuitive**
- +20% Insight effectiveness when reading a volatile/escalating situation. +25% effect from environmental hazards triggered in combat (fire, explosives, hazardous terrain).
- -1 Brains while under high stress.

**All-In Brawler** *(contingent — needs an equivalent charged/heavy "Power Attack" melee mechanic, not yet designed)*
- Power Attacks deal a large Might-scaled bonus to damage, on both normal and critical hits.
- Post-attack vulnerability window worsens substantially (reduced defense for a longer duration than the base penalty).

**Engine Overclocker** ⚠ *(contingent — needs a real-time stamina/resource system, not yet designed)*
- +1 Endurance. Once per combat, when your stamina/resource pool is fully depleted, immediately gain a burst of temporary resource for an emergency action.
- After using the burst: -2 Endurance and -2 Agility until the end of combat (burnout).

### AP-Economy Trait Cluster ⚠

All seven of these were built around Inner Tepenia's turn-based AP economy. Toronto Fell Out doesn't have a designed stamina/resource system yet, so these are held here as **tradeoff shapes** to convert once one exists — not literal numbers to implement as-is.

- **High-Output Frame** — more resource per encounter, at a stat penalty once badly hurt.
- **Efficient Design** — cheaper movement cost, at an Agility penalty.
- **Overclocked Prototype** — a strong opening-turn resource burst, at a worse resource rate for the rest of the encounter (alpha-strike playstyle).
- **Fragile but Fast** — +2 Agility, at the cost of taking damage making your next action(s) more expensive (stacking).
- **Steady Nerves** — resource regeneration counts a relevant stat as higher than it is, at an Agility penalty.
- **Minimalist Frame** — faster movement while lightly loaded, at a resource penalty while encumbered.
- **Echo Chamber** — unpredictable small resource swings (bonus near powered infrastructure/during blackouts, penalty from interference) — reskin the "Arcanet node" flavor onto whatever Toronto Fell Out's own power-grid/blackout content ends up being.

---

## Not Pursuing (Yet)

Unfinished or blocked upstream in Inner Tepenia's own file, not for any robot-specific reason — revisit only if/when resolved:

- **Bridge Feedback** — needs a "jacked in" neural-interface mechanic Toronto Fell Out doesn't have.
- **["Broad Strokes" working title]** — bonus side still undecided upstream (three candidates floated, none chosen); penalty side (never notices small environmental details, hard override) is portable whenever the bonus gets picked.
- **One-Way Exchange** — unresolved upstream due to a real production cost (tagging every "informed" skill check's information source throughout the game).
