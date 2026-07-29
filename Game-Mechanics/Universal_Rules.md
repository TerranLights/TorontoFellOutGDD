# Universal Rules

Game-wide rules that apply across all systems, content, and design decisions regardless of context. These are binding. When a specific system document conflicts with a rule listed here, this document takes precedence unless a specific named exception is documented below.

Cross-reference: some of these rules are also documented within their originating system docs. This file exists as the single consolidated reference.

---

## Inventory

**Quest items are weightless.**
All items classified as quest items carry zero inventory weight, regardless of their physical nature or size. This is unconditional — there are no heavy quest items. Applies to main-quest critical items, companion-given objects, post-romance mini-questline rewards, and any other item that receives quest item classification.

**Quest items cannot be sold, dropped, lost, pickpocketed, or broken down.**
Quest item classification confers full protection. The player cannot remove a quest item from their inventory by any means, intentional or accidental. This protection is permanent for the duration of the playthrough.

**Quest items are examinable in the inventory UI.**
Every quest item has a written description accessible from the inventory screen. The description conveys what the item is, its significance, and where relevant, what it means that the player has it.

---

## Companion System

**All recruitable companions are romanceable. No exceptions.**
Any character who can be recruited as a player companion is romanceable, subject to their individual gate conditions. This rule admits no exceptions. If a character is recruitable, they are romanceable.

**Party composition: one human companion + one non-human companion, simultaneously.**
Toronto Fell Out uses Fallout: New Vegas's dual-slot model, not a single-slot model. The non-human slot's signature character is Muttchow. Both slots are independent — recruiting a new companion in either slot requires dismissing the current occupant of that slot. See `Core-Mechanics/Companion-System.md`.

**Romance gates use the visible MAPLE-BUD stat check UI.**
Romance gates are displayed using the same visible stat-check format as all other MAPLE-BUD stat checks. Both the passing and failing dialogue options are shown simultaneously. Failed thresholds display as [current/required]. See `Core-Mechanics/Companion-System.md` for full documentation and format examples.

**Perks are excluded from romance gates.**
Romance gates check MAPLE-BUD stats and traits only — never perks. Stats and traits define who the player character fundamentally is. Perks represent what they have learned and done. A player cannot perk their way into a romance they were not built for.

**Romance gates check permanent base stats only — not temporary boosts.**
Temporary stat increases from food, chems, equipment, or any other time-limited effect do not count toward romance gate thresholds. The gate is checking who the player character fundamentally is, not their momentary enhanced state. Permanent stat raises — whether set at character creation or raised through gameplay means such as the Intense Training perk — count in full. Temporary boosts do not count at all, and there is no "angry later" consequence for attempting to use them; they are simply not read by the gate check.

**A companion's player home is accessible only while the romance is active.**
Home access is granted when the romance is established and revoked if the romance ends (via the monogamy rule). The home belongs to the companion; the player's access is contingent on the relationship.

---

## World Canon

**Sexuality by character type.** Human female characters (companions and sexually-available NPCs) are bisexual by default. Human male characters are heterosexual, fixed-gender attraction. Applies universally to companions, romanceable NPCs, and the sexually-available character pool. No exceptions established. **Mechanical consequence:** romanceable human male companions gate on an additional gender check (the player must be presenting as the gender he's attracted to) on top of the standard MAPLE-BUD stat check — see `Core-Mechanics/Companion-System.md`. Human female companions gate on the stat check alone.

*(Toronto Fell Out has no sentient robots/androids, so no robot-specific sexuality rule applies here.)*

---

## Design Law

**Fallout Precedence Law: New Vegas wins by default, with rare named exceptions.**
Where Fallout: New Vegas and Fallout 1/2/3/4 establish conflicting design precedents, New Vegas takes precedence unless a specific exception is documented below. Exceptions must be named explicitly here, not assumed case-by-case. See `General-Overview-Notes/Design-Philosophy.md`.

**Named exception — camera system: Fallout 4, not Fallout: New Vegas.**
Toronto Fell Out uses Fallout 4's free third-person camera, which allows swiveling around to view the character from the front. Fallout: New Vegas's third-person camera does not permit this. This is a deliberate, confirmed exception to the New-Vegas-wins default.
