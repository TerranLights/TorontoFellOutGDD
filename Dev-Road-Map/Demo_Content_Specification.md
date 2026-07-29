# Demo Content Specification

**What this is:** a working spec for what actually ships in the free Demo build, distinct from the Early
Access content-split plan in `Early_Access_vs_Launch_Content_Split.md` and the conceptual distinction drawn
in `Demo_vs_Early_Access.md`. Several items below are genuinely undecided and flagged as such — this is a
first pass, not a locked spec. Toronto Fell Out has far less confirmed main-quest structure than a fully
beat-mapped game would, so this file is deliberately more provisional than a comparable spec for a project
further along in main-story design.

---

## 1. Where the Demo starts and ends

Grounded in the one piece of main-quest structure that's actually locked in — `Reference/Main-Storyline-
Candidates.md`'s established hook:

- **The confirmed through-line:** the player's initial short-term goal is climbing the CN Tower and
  reactivating its radio transmitter. This is played straight as the game's apparent main objective — a
  satisfying, iconic setpiece that primes the player to believe they've won — and it's a **false victory**:
  completing it doesn't end the game, it reveals that the real objective is something else entirely. Which
  of the four candidate reveal-directions in that file ends up true (or the combined structure proposed
  there) is not yet decided, but the shape of the beat — climb, reactivate, false victory — is locked.
- **Recommended endpoint: the false-victory reveal itself.** The moment the tower's reactivation lands and
  then curdles — "we're not alone" turning into whatever the actual complication is — is a complete
  emotional unit in its own right, the same way a good demo slice ends on a real beat rather than a
  cliffhanger mid-scene.
- **Open, and more open than it would be in a project with a locked beat structure:** what happens *between*
  the player's actual game-start and reaching the tower. Toronto Fell Out doesn't yet have a confirmed
  opening location, starting scenario, or early-game structure the way it has a confirmed CN Tower hook —
  that content simply doesn't exist yet. This file can't specify it without inventing it, so it's left as an
  open item rather than a placeholder district or beat.

## 2. Companions

- **No full recruitable companion in the Demo.** Toronto Fell Out's companion system (`Game-Mechanics/Core-
  Mechanics/Companion-System.md`) confirms a dual-slot model (one human + the non-human slot, whose
  signature character is **Muttchow**), but no actual companion roster exists yet to draw from. Even once
  one does, the same logic that applies to Early Access content generally (`Early_Access_vs_Launch_Content_
  Split.md`) applies one step further down for a Demo: if companion romance is confirmed as one of the
  game's headline draws, a free, unpaid, pre-wishlist-conversion slice shouldn't spend it. The Demo's job is
  proving the game's tone, systems, and writing quality, not pre-spending its own biggest draw.
- **Open:** whether it's worth teasing Muttchow specifically (visible, clearly important, not yet
  functionally a full companion in the slice) purely as a hook — no decision made here, and contingent on
  how early in development Muttchow's own content is ready to show.

## 3. Systems that need to be represented

A Demo's job is proving the core gameplay loop works and reads well, so it should include a working (if
shallow) taste of each pillar system already established for Toronto Fell Out, not just narrative:

- **Real-time 1st-/3rd-person combat** — at least one real encounter, enough to show the core loop. Uses
  Fallout: New Vegas/Fallout 4's real-time aim/hit resolution per `Design-Philosophy.md`'s Flat Thresholds
  note, not a turn-based system.
- **MAPLE-BUD stat system** — either a pre-generated starting character with visible stats, or (if character
  creation itself is meant to be a selling point) a trimmed character-creation pass. **Open** which.
- **Dialogue/skill-check system** — flat, binary thresholds per `Design-Philosophy.md` (no dice rolls on any
  skill/stat check). Whatever early content exists between game-start and the tower should exercise this at
  least once.
- **The confirmed-but-unnamed V.A.T.S.-equivalent targeting system** — distinctive enough to be worth
  surfacing even in a short slice, once it's named and its mechanics are locked down (see `Reference/Open-
  Worldbuilding-Decisions.md`).
- **The Slip-Toy** — the wrist device is a natural, low-cost thing to introduce early and reinforce in a
  short slice, the way a Pip-Boy equivalent typically is in this genre's own openings.

**Deliberately excluded, too soon or too large for this scope:** the full perk/leveling arc; whichever hidden
Karma-replacement system (`Reference/Hidden-System-Candidates.md`) is eventually chosen, since that kind of
system only becomes legible across many hours of accumulated choices; any DLC content, since none is planned
yet. There is currently no combat sub-system document under `Game-Mechanics/Combat/` (the directory is
empty) — this spec deliberately does not reference a system that doesn't exist yet.

## 4. Technical/structural constraints

Per `Demo_vs_Early_Access.md`:

- **Free**, no purchase gate.
- **Frozen build** — the Demo isn't expected to be rebuilt in response to player feedback the way Early
  Access is; budget for a stability/polish pass before release, then leave it largely static except for bug
  fixes.
- **No save carryover** into Early Access/Launch — a separate Steam depot tied to the main store page, not a
  truncated version of the same save-compatible build.
- **Runtime target:** a single, complete sitting — commonly 20-60 minutes for CRPG demos of this kind.
  **Open:** no specific target chosen yet; worth timing against the actual opening content once it's built
  out in-engine.

## 5. What the Demo needs to prove, as a checklist

- **The tone and writing quality** — the game's central creative pitch (dark, specifically Canadian gallows
  humor sitting next to a genuinely bleak setting, per `README.md` and `General-Overview-Notes/Design-
  Philosophy.md`) — comes through even without a companion romance arc present. This checklist maps directly
  onto the Steam wishlist-conversion goal in `Steam_Launch_Strategy_and_AI_Disclosure.md` Section 2 — a Demo
  that fails any of these items is unlikely to convert into a wishlist.
- Combat feels good in a single real encounter.
- The MAPLE-BUD stat system's basic shape is legible even from a short slice.
- The false-victory structure of the CN Tower beat — climb, reactivate, apparent triumph, the turn — reads
  clearly and lands emotionally, since it's the one piece of main-quest shape the whole Demo is actually
  built around.

---

## 6. The New Vegas Lesson: build this content last, not first

Added per a design principle the developer specifically drew from interviews/documentaries about *Fallout:
New Vegas*'s own production. Goodsprings, New Vegas's opening area, was deliberately designed and finalized
**late** in development, not early — precisely because its job is to function as a representative summary of
every major thing the player will definitely experience over the full game, which means it can't actually be
locked down until the rest of the game's systems, tone, and content are known well enough to summarize. Per
the Fallout Precedence Law in `Game-Mechanics/Universal_Rules.md`, New Vegas is this project's own standing
precedent source for design questions like this one — and the parallel here is unusually direct, since
Toronto Fell Out's own opening (climb the tower, reactivate the radio, hit the false-victory beat) already
occupies the exact same structural role Goodsprings occupied for New Vegas: the first thing every player
sees, built to look simple, secretly carrying the job of representing the whole game.

**Two direct implications for Toronto Fell Out's Demo, since the Demo's content *is* the game's own opening
sequence:**

1. **Production order, not just content scope.** The Demo shouldn't be treated as "the easy early content,"
   buildable first because it's chronologically first in the story. It should be one of the **last** major
   content pieces locked down — built and iterated on only once combat, the MAPLE-BUD stat system,
   dialogue/skill checks, and the targeting system are all far enough along elsewhere in the game to actually
   be represented accurately. Building it early risks the Demo shipping a version of these systems that gets
   meaningfully revised later, making the Demo an inaccurate preview of the real game by the time Early
   Access or Launch arrives.
2. **Design mandate, not just checklist.** Section 5's "what the Demo needs to prove" checklist isn't just a
   QA pass to run once the opening content exists — it's the actual brief the opening content should be
   *designed against* from the start. Whatever fills the gap between game-start and the tower, and the tower
   sequence itself, should be deliberately engineered as a compressed, representative sample of the full
   game's major systems and tone (per the Goodsprings precedent), not merely "whatever the first story beat
   happens to contain that also incidentally teaches the player something."

**The genuine tension this creates, left open rather than resolved here:** Section 2 of
`Steam_Launch_Strategy_and_AI_Disclosure.md` recommends launching a Demo well *before* Early Access to build
wishlist velocity and land a Steam Next Fest slot — which pushes toward building the Demo *early*. The New
Vegas lesson above pushes the opposite direction — toward finalizing it *late*. One resolution precedent worth
naming: Goodsprings itself still existed in a rough, playable form throughout most of New Vegas's own
production — it was iterated on repeatedly, not built from a blank slate at the very end. The likely shape for
Toronto Fell Out is the same: **rough out the Demo's content early enough to hit a Next Fest window, but
treat it as a living draft that gets revised alongside the rest of the game, with a final polish/finalization
pass deliberately scheduled late** rather than a single early build and then no more.

---

## Still Open

- What actually happens between the player's real game-start and reaching the CN Tower — no opening
  location, scenario, or early structure is designed yet; this is the single biggest gap in this spec
  compared to a project with a locked beat structure.
- Which of the four candidate false-victory directions (or the combined structure) in `Reference/Main-
  Storyline-Candidates.md` is chosen — the Demo's ending beat depends on this only insofar as it needs the
  reveal to land, not on which specific direction it turns out to be.
- Whether Muttchow gets a glimpse/tease without being a functional companion in the slice.
- Pre-generated character vs. trimmed character creation.
- Target runtime.
- Timing relative to Early Access launch and any specific Steam Next Fest window.
- The exact rough-draft-then-finalize schedule described in Section 6 — no specific milestones chosen yet for
  when the Demo's content gets its first playable pass vs. its final polish pass.

See `Tutorial_Section_Specification.md` for the fuller, standalone brief on what the tutorial/opening sequence
itself needs to contain — since that content and the Demo's content are the same sequence, that file expands
on Sections 3, 5, and 6 above in more detail.
