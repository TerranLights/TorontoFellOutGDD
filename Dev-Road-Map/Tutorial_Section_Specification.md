# Tutorial Section Specification

**What this is:** a standalone spec for the opening/tutorial sequence itself — split out into its own file so
it can be referenced independently of the Demo and Early Access planning it overlaps with. The tutorial
sequence — whatever precedes it plus the CN Tower climb and radio reactivation, per `Reference/Main-
Storyline-Candidates.md` — *is* the Demo's actual content (see `Demo_Content_Specification.md`), but this
file exists because the tutorial has its own design mandate independent of Demo/wishlist concerns — it's the
one piece of content every single player of the finished game will experience, regardless of whether they
ever touched a Demo.

**Governing principle:** per `Demo_Content_Specification.md` Section 6 (the "New Vegas Lesson," drawn from how
Obsidian built Goodsprings), the tutorial's job is to function as a **compressed, representative summary of
every significantly major thing the player will definitely experience across the full game** — which is why
it should be finalized late in development even though it's chronologically the first thing a player sees.
This file is the content brief that principle produces. Toronto Fell Out has considerably less confirmed
main-quest structure than a project with a locked beat-by-beat outline would have, so several sections below
are framed as requirements to design against rather than content that already exists.

---

## 1. Systems every CRPG tutorial has to cover, in Toronto Fell Out's own specific form

- **MAPLE-BUD stats mattering immediately.** At least one moment early on where a stat check visibly changes
  an outcome — not just a flavor line — so character-creation choices land right away. See `Game-Mechanics/
  Character-Creation/Skills.md` for the full MAPLE-BUD attribute and skill list.
- **A real skill-check payoff.** Something in the opening content that's meaningfully easier, or newly
  possible, because of a specific invested skill, so it reads as a real build decision rather than a number
  on a sheet. **Open:** whether Toronto Fell Out uses a Fallout: New Vegas-style Tagged-skill mechanic at all
  — nothing in the existing skill/perk documentation confirms this one way or the other yet, so it isn't
  assumed here.
- **One real combat encounter** — enough to establish the real-time 1st-/3rd-person aim/hit-resolution loop
  (per `Design-Philosophy.md`'s Flat Thresholds note, this is Fallout: New Vegas/Fallout 4 real-time combat,
  not a turn-based system), without needing the full perk/leveling arc behind it yet.
- **A first level-up**, timed to land during or right after the opening content, so the leveling model is
  *felt* early, not just explained in a menu. **Open:** whether Toronto Fell Out uses a lump-sum XP model or
  another leveling shape — not established yet.

## 2. What makes this specifically a Toronto Fell Out tutorial, not a generic one

- **The Fame/Infamy reputation system's first registration.** `Game-Mechanics/Core-Mechanics/Reputation-
  System.md`'s two-axis system (carried over near-verbatim from Fallout: New Vegas) needs its first real move
  to happen here — whatever early content precedes the tower is a natural place for a player's early choice
  to visibly shift a reputation tier, previewing that the whole game tracks this.
- **The confirmed-but-unnamed V.A.T.S.-equivalent targeting system.** Distinctive enough to deserve a
  deliberate small introduction once it's named and its mechanics are locked (`Reference/Open-Worldbuilding-
  Decisions.md`), not left to be discovered by accident.
- **The Slip-Toy.** Toronto Fell Out's wrist device is a natural, low-cost thing to introduce clearly and
  mechanically in the opening sequence, the same way a Pip-Boy equivalent typically is in this genre's own
  openings — there's no "Bridge Unit"/jack-in identity-creation scene to build around instead, since Toronto
  Fell Out has no sentient robots and no equivalent premise; the player character is simply a person, and
  whatever establishes who they are at game-start is a separate, currently undesigned opening scenario (see
  Still Open, below).
- **At least one unmarked discovery.** Something in the opening content should be findable without a quest
  marker — teaching the player from minute one that this game rewards actually looking, not just following
  waypoints. No specific instance of this is designed yet.
- **The "you can say no" moment.** Whatever the game's opening request/hook turns out to be, giving the
  player a real, legible option to decline it and wander off instead previews the game's own non-linear
  philosophy from the first scene. Not yet tied to specific content, since the opening scenario itself isn't
  designed.

## 3. Tone-setting, not mechanical

- **Toronto Fell Out's specific tonal register** — dark, specifically Canadian gallows humor sitting next to
  a genuinely bleak, irradiated setting, per `README.md` and `General-Overview-Notes/Design-Philosophy.md` —
  should be legible through at least one ambient interaction in the opening content, ideally before the
  player even reaches the tower.
- **A planted-not-resolved hook.** The tutorial should teach players early that not everything pays off
  immediately, since that's the game's long-arc storytelling shape throughout — this can be layered onto the
  false-victory beat itself (the CN Tower reveal is, structurally, exactly this kind of planted hook at a
  larger scale) or onto something smaller in the run-up to it.

## 4. Deliberately out of scope for the tutorial

Systems that should NOT be introduced in the opening sequence, because they're either too much apparatus for
an opening or illegible until much later content has accumulated:

- Full companion recruitment and romance (see `Demo_Content_Specification.md` Section 2 for the reasoning —
  no recruitable companion in this sequence).
- Whichever hidden Karma-replacement system (`Reference/Hidden-System-Candidates.md`) is eventually chosen —
  this kind of system only becomes legible once many hours of accumulated choices exist behind it.
- Any DLC content — none is planned yet.

**Not applicable at all, rather than merely out of scope:** a re-specialization/identity-fragmentation
mechanic (Toronto Fell Out has no re-speccing system of any kind, so there's nothing here to defer) and a
robot-human relations baseline (Toronto Fell Out has no sentient robots, so this consideration simply doesn't
exist for this game).

---

## Still Open

- **The opening scenario itself.** Toronto Fell Out has a confirmed main-quest hook (climb the tower,
  reactivate the radio, false victory) but no confirmed starting location, starting scenario, or content
  between game-start and reaching the tower. This is the largest open item in this file, and everything in
  Sections 1-3 that references "the opening content" is written against a placeholder until that scenario
  exists.
- Which specific stat/skill check carries the "MAPLE-BUD stats matter immediately" moment, and whether a
  Tagged-skill-style mechanic exists at all — not chosen yet.
- Whether the unmarked discovery and the "say no" branch are the same moment or two separate ones.
- Exact scheduling of the "rough draft early, finalize late" production plan described in
  `Demo_Content_Specification.md` Section 6 — no milestones chosen yet.
