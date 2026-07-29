# Reputation System

**Source:** Fallout: New Vegas's two-axis Fame/Infamy reputation system, carried over near-verbatim (per the "Fallout Precedence" rule in `Design-Philosophy.md`: where territory overlaps with an existing Fallout: New Vegas system, treat FNV's implementation as the default reference). This isn't a reskin — it's the same system, same tier names, same structure.

---

## The Two-Axis Model

Reputation is **not a single scale**. Two independent tracks are maintained simultaneously per faction/district:

- **Positive Reputation ("Fame")** — Range 0 through Range 3
- **Negative Reputation ("Infamy")** — Range 0 through Range 3

The tier a player actually holds is the *combination* of both axes, not an average or a single blended number. A player can be simultaneously high on both axes at once (see Wild Child, bottom-right cell) — this is a real, distinct state, not a contradiction the system averages away.

## The Full Grid

**Legend:** 🟢 green = favorable reputation overall · 🔴 red = unfavorable reputation overall · ⚪ white/black = genuinely ambiguous, not read as clearly good or bad even by the people holding the opinion.

| Infamy ↓ / Fame → | **Range 0** | **Range 1** | **Range 2** | **Range 3** |
|---|---|---|---|---|
| **Range 0** | ⚪ **Neutral** — People don't know enough about you to form an opinion. | 🟢 **Accepted** — Folks have come to accept you for your helpful nature. | 🟢 **Liked** — Enough news of your good works has been passed around that people like you. | 🟢 **Idolized** — Renowned for your extensive support and goodwill, you are idolized by the community. |
| **Range 1** | 🔴 **Shunned** — You've left a poor impression on the community and may be shunned as a result. | ⚪ **Mixed** — A little bit good mixed with a little bit bad, people haven't figured you out yet. | 🟢 **Smiling Troublemaker** — People know you're good at heart even though you're occasionally a troublemaker. | 🟢 **Good-Natured Rascal** — Your reputation as a good-natured friend of the community manages to outshine your dark side. |
| **Range 2** | 🔴 **Hated** — Now that folks know you're bad, most people outright hate you. | 🔴 **Sneering Punk** — Even though you've done some good for the community, people still think you're a punk. | ⚪ **Unpredictable** — No one's sure what to make of your unpredictable nature, but you've left a strong impression. | ⚪ **Dark Hero** — Folks still think you're some kind of hero, but you sure can be nasty sometimes. |
| **Range 3** | 🔴 **Vilified** — For your overwhelmingly monstrous behavior, you have become vilified by the community. | 🔴 **Merciful Thug** — Despite your reputation as a thug, you are known to occasionally show a charitable side. | ⚪ **Soft-Hearted Devil** — Most people say you're the devil himself, but most admit you've also done a world of good. | ⚪ **Wild Child** — Your wild, seemingly capricious behavior leaves people scratching their heads in confusion and avoiding close contact. |

16 total named combinations. Row = Infamy tier, column = Fame tier; read the cell where they intersect.

## Named Tiers, Grouped

**🟢 Favorable overall:** Accepted, Liked, Idolized (pure Fame axis) · Smiling Troublemaker, Good-Natured Rascal (mixed but still read as good)
**🔴 Unfavorable overall:** Shunned, Hated, Vilified (pure Infamy axis) · Sneering Punk, Merciful Thug (mixed but still read as bad)
**⚪ Genuinely ambiguous, not clearly good or bad even to the people holding the opinion:** Neutral, Mixed, Unpredictable, Dark Hero, Soft-Hearted Devil, Wild Child
**The extreme case — both axes maxed simultaneously: Wild Child** (Fame Range 3 + Infamy Range 3). A real, distinct, permanent state a player can actually hold, not a contradiction the system resolves — a strong candidate for dedicated late-game content (unique dialogue, a rare companion-questline route — see `Companion-System.md`'s Personal Questline Design Rule) if Toronto Fell Out wants to build toward it, the way Inner Tepenia built dedicated Wild Child endings around this exact tier.

## Reputation-Based Merchant Discounts

**Any 🟢 favorable reputation tier with a district grants the player a purchase discount at every merchant in that district** — not scoped to any one vendor or service type.

**Discount scales with how favorable the tier is, paired by overall favorability level rather than by raw Fame magnitude alone:**

| Tier(s) | Discount |
|---|---|
| **Accepted** or **Smiling Troublemaker** | −5% |
| **Liked** or **Good-Natured Rascal** | −10% |
| **Idolized** | −20% |

**Idolized has no mixed-tier counterpart at this top level** — at Infamy Range 2 or 3 with max Fame, the grid reads as ambiguous (Dark Hero, Wild Child) rather than favorable, so there's no "mixed" equivalent to pair with Idolized the way Accepted/Smiling Troublemaker and Liked/Good-Natured Rascal are paired.

**⚪ ambiguous tiers (Neutral, Mixed, Unpredictable, Dark Hero, Soft-Hearted Devil, Wild Child) and 🔴 unfavorable tiers grant no discount** — only the five named 🟢 favorable tiers above do.

---

## Open Design Questions

- **Scope:** whether this tracks per-district, per-faction, or both, once Toronto Fell Out's own factions/districts are designed (see `TODO.md`).
- **Mechanical thresholds:** exact point values or actions required to move between Range 0-3 on each axis are not yet designed.
- **Full system design** (how reputation is earned/lost, UI presentation, whether it's visible to the player as raw numbers or only through tier names and NPC reactions) is not yet started — this file only formalizes the tier grid itself.
