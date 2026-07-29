# Perks

Toronto Fell Out's perk list. Built in two layers: the full Fallout: New Vegas perk list as a foundation (stat requirements translated from SPECIAL to [MAPLE-BUD](../to-be-integrated/not-SPECIAL.md): Str→Might, Per→Perception, Agl→Agility, End→Endurance, Int→Brains, Cha→Determination, Luck unchanged), plus additional perks adapted from Inner Tepenia. See `Design-Philosophy.md` for the perk design laws these should follow going forward, and `reference/Inner-Tepenia-Adapted-Candidates.md` for the full survey this was drawn from.

**Open items carried over from the source material:**
- ⚠ marks a perk whose effect was originally written for a turn-based AP economy (Inner Tepenia) and needs to be cross-checked against how Fallout: New Vegas/Fallout 4 actually implement the equivalent in real time before it's built.
- **Fight the Power!** (references NCR/Legion/Brotherhood of Steel armor) and **Sneering Imperialist** (references tribal/raider characters) need reskinning onto Toronto Fell Out's own factions once those exist.
- **Robotics Expert** appears twice in the source (Level 10 and Level 12) — a duplication artifact, not two distinct perks. The Level 10 entry's second sentence ("10% chance that the Mysterious Stranger will finish off a target in V.A.T.S.") looks misattributed and probably belongs to **Mysterious Stranger** instead. **Mysterious Stranger**'s own listed effect ("+50% damage with fire-based weapons") also looks misattributed — it matches **Pyromaniac** almost verbatim. Flagged, not resolved.
- **Eye for Eye** and **Adamantium Skeleton** (Level 14) both depend on the limb-specific damage/crippling system — confirmed planned, see `TODO.md`.
- **Terminology placeholders still in FNV's own words below, pending Toronto Fell Out's own names** (all confirmed to exist as concepts — see `reference/Open-Worldbuilding-Decisions.md`):
  - **V.A.T.S.** — Toronto Fell Out confirmed to have its own bullet-time/assisted-targeting system; name not yet decided. Every "V.A.T.S." mention below is a stand-in for it.
  - **Stimpak** — confirmed to have its own healing-item equivalent; name not yet decided.
  - **Bottle caps** — needs Toronto Fell Out's own default currency name (tentatively separate from a possible secondary "Canadian Tire money"-style currency — see the reference file).
  - **Pip-Boy** → already resolved to **Slip-Toy** and updated throughout.
  - **Hardcore** → confirmed to carry over as-is ("Hardcore Mode"), no change needed.
- **Creature/item references still assuming Fallout's bestiary, pending Toronto Fell Out's own** (see `reference/Open-Worldbuilding-Decisions.md`): **Ghastly Scavenger** (super mutant/feral ghoul), **Purifier** (centaurs, night stalkers, spore plants, spore carriers, deathclaws, super mutants), **Mile in Their Shoes** (night stalkers, night stalker squeezin's), **Them's Good Eatin'** (thin red paste, blood sausage). Ghouls are confirmed to exist in-setting; the rest are open.

---

## Foundation: Ported from Fallout: New Vegas

### Universal

**Intense Training** *(Level 10)*
You can put a single point into any of your MAPLE-BUD attributes.

### Level 2

**Black Widow**
+10% damage to the opposite sex and unique dialogue options with certain characters.

**Cherchez La Femme**
+10% damage to the same sex and unique dialogue options with certain characters.

**Friend of the Night** *(Perception 6, Sneak 30)*
Your eyes adapt quickly to low-light conditions.

**Heave, Ho!** *(Might 5, Explosives 30)*
+50% thrown weapon velocity and range.

**Hunter** *(Survival 30)*
In combat, you do 75% more critical damage against animals and mutated animals.

**Junk Rounds** *(Luck 6, Repair 45)*
You can craft ammunition using scrap metal and tin cans.

**Light Touch** *(Agility 6, Repair 45)*
While wearing light armor you gain +5% critical hit chance and your enemies suffer a -25% critical hit chance.

**Old World Gourmet** *(Endurance 6, Survival 45)*
+25% addiction resistance. +50% health bonus from snack foods. Scotch, vodka, and wine now give you health in addition to their normal effects.

**Rapid Reload** *(Agility 5, Guns 30)*
All of your weapon reloads are 25% faster than normal.

**Retention** *(Brains 5)*
Skill magazines last for 3 real-time minutes.

**Swift Learner** *(Brains 4, ranks: 3)*
You gain an additional 10% whenever experience points are earned.

### Level 4

**Cannibal**
When you're in Sneak mode, you gain the option to eat a human corpse to regain hit points, but lose Karma.

**Comprehension**
You gain one additional skill point for reading books and double the skill points for reading magazines.

**Educated** *(Brains 4)*
You gain two more skill points every time you advance in level.

**Entomologist** *(Brains 4, Survival 45)*
You do an additional 50% damage every time you attack a mutated insect.

**Rad Child** *(Survival 70)*
Regenerate 2 HP per second per 200 rads accumulated.

**Run 'n Gun** *(Guns 45 or Energy Weapons 45)*
Halved spread with one-handed ranged weapons while walking or running.

**Travel Light** *(Survival 45)*
While wearing light armor or no armor, you run 10% faster.

### Level 6

**Bloody Mess**
+5% overall damage; more violent death animations.

**Demolition Expert** *(Explosives 50, ranks: 3)*
+20% damage with explosives.

**Ferocious Loyalty** *(Determination 6)*
When you drop below 50% HP, companions gain +50 DR.

**Fortune Finder** *(Luck 5)*
Considerably more bottle caps will be found in stockpiles.

**Gunslinger**
+25% accuracy in V.A.T.S. with one-handed weapons.

**Hand Loader** *(Repair 70)*
When using Guns, you are twice as likely to recover cases and hulls. You also have all hand load recipes unlocked at any reloading benches.

**Lead Belly** *(Endurance 5 or Survival 40)*
-50% radiation taken from food and water sources.

**Mad Bomber** *(Repair 45, Explosives 45)*
Enables you to create special explosive recipes at any workbench.

**Shotgun Surgeon** *(Guns 45)*
When using shotguns, regardless of ammunition used, you ignore an additional 10 points of a target's Damage Threshold.

**The Professional** *(Sneak 70)*
Your Sneak Attack Criticals with revolvers, pistols, and submachine guns (guns and energy weapons) all inflict an additional 20% damage.

**Toughness** *(Endurance 5, ranks: 2)*
+3 DT permanently.

**Vigilant Recycler** *(Science 70)*
When using Energy Weapons, you are twice as likely to recover drained ammunition. You also have more efficient recycling recipes available at workbenches.

### Level 8

**Commando**
+25% accuracy in V.A.T.S. with two-handed weapons.

**Cowboy** *(Guns 45, Melee 45)*
+25% damage done by dynamite, hatchets, knives, revolvers, and lever-action guns.

**Grunt** *(Guns 45, Explosives 20)*
25% more damage with 9mm pistols and SMGs, .45 pistols and SMGs, service rifles, assault and Marksman carbines, light machine guns, frag grenades, grenade rifles and launchers, and combat knives.

**Home on the Range** *(Survival 70)*
Whenever you interact with a campfire, you have the option of sleeping, with all the benefits that sleep brings.

**Living Anatomy** *(Medicine 70)*
Shows health and Damage Threshold of any target. +5% bonus to damage against humans and non-feral ghouls.

**Pack Rat** *(Brains 5, Barter 70)*
Items with a weight of two pounds or less now weigh half as much.

**Quick Draw** *(Agility 5)*
Makes weapon equipping and holstering 50% faster.

**Rad Resistance** *(Endurance 5, Survival 40)*
+25% radiation resistance permanently.

**Scrounger** *(Luck 5)*
Considerably more ammunition in stockpiles.

**Sneering Imperialist**
+15% damage and +25% accuracy in V.A.T.S. to various tribal and raider characters.

**Tribal Wisdom** *(Survival 70)*
-50% limb damage from animals, mutated animals, and mutated insects; +25% to Poison Resistance; ability to eat mutated insects in sneak mode.

**Stonewall** *(Might 6, Endurance 6)*
+5 DT against melee and unarmed attacks and cannot be knocked down during combat.

**Strong Back** *(Might 5, Endurance 5)*
+50 Carry Weight.

**Super Slam!** *(Might 6, Melee Weapons 45)*
All melee (except thrown) and unarmed attacks have a chance of knocking your target down: 15% for Unarmed or one-handed melee, 30% for two-handed melee.

**Terrifying Presence** *(Speech 70)*
Can intimidate foes through dialogue; closing dialogue results in the foe fleeing for 5 seconds.

### Level 10

**And Stay Back** *(Guns 70)*
Shotguns have a 10% chance, per pellet, of knocking an enemy back in a way similar to the Super Slam! perk.

**Here and Now**
You instantly level up again.

**Animal Friend** *(Determination 6, Survival 45, ranks: 2)*
With the first rank, hostile animals become neutral. With the second rank, they assist in combat, but not against other animals.

**Fight the Power!**
+2 Damage Threshold and +5% Critical Chance against anyone wearing NCR, Legion, or Brotherhood of Steel armor.

**Finesse**
+5% Critical Chance.

**Math Wrath** *(Science 70)*
Reduces all AP costs by 10%.

**Miss Fortune** *(Luck 6)*
10% chance that Miss Fortune will incapacitate a target in V.A.T.S.

**Mister Sandman** *(Sneak 60)*
Can instantly kill a sleeping non-player character and earn bonus XP when doing so.

**Mysterious Stranger** *(Luck 6)*
+50% damage with fire-based weapons.

**Robotics Expert** *(Science 50)*
+25% damage to robots; can shut down robots by sneaking up on them and deactivating.

**Nerd Rage!** *(Brains 5, Science 50)*
+15 DT and Might increased to 10 whenever health is 20% or lower.

**Night Person**
+2 Brains and +2 Perception between 6:00 p.m. and 6:00 a.m.

**Plasma Spaz** *(Energy Weapons 70)*
AP costs for all plasma weapons are reduced by 20%.

### Level 12

**Alertness** *(Perception 6-9)*
+2 Perception when crouched and still.

**Fast Metabolism**
+20% Hit Points restored with stimpaks.

**Ghastly Scavenger** *(requires "Cannibal" perk)*
When you're in Sneak mode, you gain the option to eat a super mutant or feral ghoul corpse to regain hit points, but lose Karma.

**Heavyweight** *(Might)*
Weapons with a weight of more than 10 are cut in half. Does not affect weapons modded to under 10 wg.

**Hobbler** *(Perception 7)*
Your chance to hit an opponent's legs in V.A.T.S. is increased by 25%.

**Hit the Deck** *(Explosives 70)*
+25 DT against explosives.

**Life Giver** *(Endurance 6)*
+30 HP.

**Long Haul** *(Endurance 6, Barter 70)*
Being over-encumbered no longer prevents you from using fast travel.

**Piercing Strike** *(Unarmed 70)*
All your unarmed and melee attacks negate 15 points of DT.

**Pyromaniac** *(Explosives 60)*
+50% damage with fire-based weapons.

**Silent Running** *(Agility 6, Sneak 50)*
Running no longer factors into a successful sneak attempt.

**Sniper** *(Perception 6, Agility 6)*
25% more likely to hit the target's head in V.A.T.S.

**Splash Damage** *(Explosives 70)*
Explosives have a 25% larger area of effect.

**Unstoppable Force** *(Might 7, Melee Weapons 90)*
x4 normal damage through enemy Blocks with melee and unarmed attacks.

### Level 14

**Eye for Eye**
For each crippled limb you have, you do an additional 10% damage.

**Adamantium Skeleton**
Damage taken by limbs reduced by 50%.

**Center of Mass** *(Guns 70)*
In V.A.T.S., you do an additional 15% damage when targeting the torso.

**Chemist** *(Medicine 60)*
Chems and (in Hardcore) stimpaks last twice as long.

**Jury Rigging** *(Repair 90)*
Repair any item using a roughly similar item.

**Light Step** *(Perception 6, Agility 6)*
Floor traps or mines will not be set off.

**Purifier**
You do 50% extra damage with melee and Unarmed weapons against centaurs, night stalkers, spore plants, spore carriers, deathclaws, and super mutants.

### Level 16

**Action Girl** *(Agility 6, ranks: 2)*
+15 AP per rank.

**Better Criticals** *(Perception 6, Luck 6)*
+50% damage with critical hits.

**Chem Resistant** *(Medicine 60)*
Half as likely to get addicted.

**Meltdown** *(Energy Weapons 90)*
Foes killed by your Energy Weapons emit a corona of harmful energy.

**Tag!**
Grants a fourth "tag" skill: +15 points to that skill.

**Weapon Handling** *(Might < 10)*
Weapon Might requirements are now 2 points lower than normal for you.

### Level 18

**Computer Whiz** *(Brains 7, Science 70)*
Can make one extra attempt to hack a locked-down terminal.

**Concentrated Fire** *(Energy Weapons 60, Guns 60)*
+5% accuracy in V.A.T.S. with every subsequent attack on a given body part queued.

**Infiltrator** *(Perception 7, Lockpick 70)*
Can make one more attempt to pick a broken lock.

**Paralyzing Palm** *(Unarmed 70)*
Can paralyze an enemy for 30 seconds with a V.A.T.S. unarmed attack.

**Walker Instinct** *(Survival 50)*
+1 Perception and Agility when outside.

### Level 20

**Atomic!** *(Endurance 6)*
In irradiated areas, +25% move and attack speed, +2 DT, +2 Might. With excess rad level, AP regen scales from 1.1x to 1.5x normal.

**Explorer**
All locations are marked on your map.

**Grim Reaper's Sprint**
A kill in V.A.T.S. restores 20 AP immediately.

**Mile in Their Shoes** *(Survival 25)*
You have come to understand night stalkers. Consuming night stalker squeezin's now grants bonuses to Perception (+1 Perception), Poison Resistance (+5), and Stealth (+5 Sneak) in addition to the normal benefits.

**Ninja** *(Melee Weapons 80, Sneak 80)*
Multiplies Critical Chance by x1.15 with melee and unarmed weapons (despite the in-game description stating a flat +15% bonus), and grants +25% damage with melee/unarmed sneak attack criticals.

**Solar Powered** *(Endurance 7)*
+2 Might and +1 HP per second while outside, from 6:00 a.m. to 6:00 p.m.

**Them's Good Eatin'** *(Survival 55)*
Any living creature you kill has a 50% chance to have the potent healing items thin red paste or blood sausage when looted.

### Level 22

**Irradiated Beauty** *(Endurance 8)*
Sleep removes all Rads (Hardcore: only -100 Rads).

**Laser Commander** *(Energy Weapons 90)*
You do an extra 15% damage and have a 10% extra chance to critically hit with any laser weapon.

**Voracious Reader** *(Brains 7)*
Damaged books become blank magazines; can copy existing magazines into blank magazines.

### Level 24

**Slayer** *(Agility 7, Unarmed 90)*
The speed of all your melee and unarmed attacks is increased by 30%.

### Level 26

**Nerves of Steel** *(Agility 7)*
20% faster AP regeneration.

**Tunnel Runner** *(Agility 8)*
+25% sneaking speed when wearing light or no armor.

### Level 28

**Rad Absorption** *(Endurance 7)*
-1 Rad every 20 seconds.

**Roughin' It** *(Survival 100)*
Sleeping outside gives Well Rested benefit.

### Level 30

**Implant GRX** *(Endurance 8, ranks: 2)*
You gain a non-addictive subdermal turbo (chem) injector. The second rank increases the effect from 2 to 3 seconds and the uses per day from 5 to 10 (activated via the Slip-Toy).

**Burden to Bear** *(Might 6, Endurance 6)*
+50 Carry Weight.

### Level 36

**Broad Daylight**
No Sneak penalty for using the Slip-Toy's light.

### Level 40

**Certified Tech**
+25% critical hit chance against robots, 85% chance of finding an extra crafting component on destroyed robots.

### Level 50

Requirement branches on current Karma.

**Ain't Like That Now** *(Karma < -250)*
Karma reset to 0, +25% AP regeneration rate, +20% attack speed, immunity to critical hits.

**Just Lucky I'm Alive** *(-250 < Karma < 250)*
+4 Luck for 3 minutes upon finishing a battle with less than 25% health; immunity to critical hits, +50% critical damage.

**Thought You Died** *(Karma > 250)*
+10 Health per 100 Karma; Karma reset to 0, +10% damage, immunity to critical hits.

---

## Additional Perks (Adapted from Inner Tepenia)

Requirement thresholds below are simplified from Inner Tepenia's dual-MACHINE-stat gates down to a single MAPLE-BUD stat + skill gate, and should be treated as placeholders pending Toronto Fell Out's own balancing pass — the content that matters here is each perk's effect and identity, not the exact numbers yet.

### Discovery

**Derelict's Eye**
*(No stat/skill gate — earned by discovery)* Unlocked by finding and successfully restoring a genuinely derelict, pre-collapse structure: archaeological reclamation of something dormant since the war, not routine repair of already-functioning infrastructure, with no quest marker pointing to it. Grants permanent at-a-glance recognition of what any ruined pre-war structure originally was and what it'd take to restore it.

### Social / Dialogue

**Silver Tongue** *(Determination 8, Speech 40, ranks: 2)*
+20% bonus to non-combat persuasion checks. Rank 2: after a failed persuasion check, one retry attempt per interaction becomes available.

**Lie Detector** *(Perception 9, Insight 50)*
Always know when an NPC is lying. Choose whether to reveal this knowledge in the moment or hold it for leverage.

**Fly on the Wall** *(Determination 8, Speech 80 or Sneak 100)*
If you witness an event without intervening, NPCs involved can be made to forget you were present. Powerful for intelligence gathering without commitment.

**Diplomat** *(Determination 8, Speech 90)*
Full diplomatic authority in formal negotiations; summits, treaty talks, and faction leadership meetings treat you as a legitimate party rather than a mere messenger or petitioner.

### Combat / Survival

**Last Stand** *(Determination 8, Endurance 7)* ⚠
Once per combat, when your health would reach zero, survive instead at 1 HP with a brief window of near-immunity to act. *(Originally: "immediately gain double AP for an emergency action... immune to all attacks until it's the player's turn" — turn-based framing. Real-time equivalent needs designing: likely a brief invulnerability/bullet-time window rather than an AP grant.)*

**Ferocious Loyalty**, **Field Repair Protocols** — see below (Technical/Utility) and Foundation section above.

### Technical / Utility

**Thermal Engineer** *(Brains 7, ranks: 2)*
Improved heat and power allocation in managed systems; reduces collateral damage during blackouts/power failures. Rank 2: temporarily stabilize a failing grid section, buying time for a proper solution.

**Power Grid Manager** *(Endurance 6, Brains 6, ranks: 2)*
Route emergency power through improvised pathways, unlocking unique solutions in power/utility-grid-related quests. Rank 2: improvised bypasses persist after you leave the area — a lasting infrastructure change.

**Precision Maintenance** *(Brains 9 or Repair 100, ranks: 3)*
Repaired items degrade more slowly and occasionally exceed their base specifications after repair. Rank 1: items degrade 10% slower. Rank 2: 20% slower. Rank 3: 30% slower.

**Field Repair Protocols** *(Endurance 6, Repair 50, ranks: 2)*
Perform emergency self-repair mid-combat using components in inventory — no workbench needed. Rank 2: can also patch up companions mid-combat.

### Robot/Automated-Defense Combat

Written for fighting non-sentient robots/automated defenses — relevant given Toronto Fell Out's Securitron-/Sentry-Bot-style enemies.

**Electronic Disruptor** *(Brains 7, Science 60, ranks: 2)* ⚠
EMP and electronic attacks have higher success rates and longer effect durations. Rank 2: a successful electronic attack can chain disruption to one adjacent electronic target at no additional cost.

**Electronic Warfare** *(Brains 8, Perception 7)* ⚠
Direct, reliable disruption of enemy electronics and robotic systems in the field, beyond what a single Electronic Disruptor-style trick can manage alone.

**Chain Protocol** *(Determination 8, Brains 7)* ⚠
Critical hits on robot enemies have a significantly higher chance to trigger cascade failures. A cascade can spread from the struck component to one adjacent system.
