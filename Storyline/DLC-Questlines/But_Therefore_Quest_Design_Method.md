# The "But / Therefore" Method — Quest & Plot Design Rules

**Source:** Trey Parker and Matt Stone (South Park), via [perell.com's summary](https://perell.com/note/but-therefore-rule/) and a
[r/Screenwriting discussion thread](https://www.reddit.com/r/Screenwriting/comments/7266rn/). Adapted for
Toronto Fell Out from Inner Tepenia's own `But_Therefore_Quest_Design_Method.md` — the method itself is
generic screenwriting craft, not tied to either game's specific lore, so it carries over almost unchanged.
Only the worked example in Section 4 and the cross-references in Section 6 are TFO-specific.

**Status:** a reusable method, not itself a quest or a piece of lore. Nothing in Section 4's worked example
is canon — it's a small, illustrative, throwaway scenario built to teach the technique, explicitly not a
real Toronto Fell Out quest.

---

## 1. The core rule

Parker and Stone tested this on their writers' room whiteboard: **whenever you can connect two beats
in your outline with "and then," the story is inert. Whenever you connect them with "but" or
"therefore," the story has momentum.**

- **Weak (And Then):** *Jimmy went to the mall, and then he got tired, and then he got a coffee, and
  then he walked back to the lot, and then he drove home.* Every beat is true, in order, and nobody
  cares.
- **Strong (But / Therefore):** *Jimmy went to the mall, but he realized he was tired. Therefore he
  got a coffee. But he'd parked in an illegal spot because he was tired. Therefore, when he got back,
  his car had been towed.*

Nothing in the second version is a bigger event than the first. The only thing that changed is that
every beat is now a *consequence* of the beat before it, and half of those consequences are
*unwelcome*. That's the whole rule.

---

## 2. "But" and "Therefore" are not interchangeable — they do two different jobs

This is the sharpest, most useful distinction to come out of the discussion thread (credit: u/120_pages),
and it's worth holding onto as two separate tools rather than one combined mantra:

- **"Therefore" = consequence.** Something happens *because* of what just happened. This is what
  stops a plot from being episodic — events stop being random and start being caused.
  *Bob proposed to Jill. Therefore, Jill broke up with Dan.*
- **"But" = reversal.** Something happens that **subverts the expectation the last beat just set up.**
  This is what keeps a plot from being predictable, even once it's causally connected.
  *Bob proposed to Jill. But Jill took out a life insurance policy and started plotting with Dan to
  kill him.*

A quest built entirely out of "Therefore" chains is causally sound but can still be flat — one damn
thing correctly causing the next damn thing, with no surprise anywhere. A quest needs **both**: the
"Therefore" beats give it a spine, and the "But" beats keep bending that spine somewhere the player
didn't expect.

---

## 3. The failure mode: "But / Therefore" wearing an "And Then" costume

Flagged directly in the discussion thread, and worth taking seriously: **the words "but" and
"therefore" don't do the work by themselves.** You can write a chain that's technically all
Buts-and-Therefores and is still just a disguised And-Then list, if none of the "buts" are genuine
reversals:

> Our secret agent found the villain's lair — **and then** ran into three henchmen — **and then**
> used the gadget from page ten — **and then** made a lucky escape — **and then** reached a dead end
> — **and then** the henchmen caught up — **and then** her partner appeared in a vent — **and then**
> the villain flooded the vents with gas.

Every one of those beats *could* be phrased with "but"/"therefore," and it would still read as flat,
because each event was already the expected next step. **The test isn't "did I use the word 'but,'"
it's "did this beat actually make the player's situation worse, or force a choice they didn't see
coming, relative to what the last beat implied was about to happen."** If a beat doesn't pass that
test, it's an And Then no matter which conjunction is sitting in front of it.

---

## 4. Worked example — illustrative only, not canon

**This scenario is invented purely to teach the method.** It is not a real Toronto Fell Out quest, it
doesn't imply any confirmed NPC, faction, or location, and nothing in it should be treated as
established lore. It uses only generic, already-safe setting texture (PATH tunnels, radioactive winter,
the general existence of non-sentient automated defenses) rather than anything specific to Toronto Fell
Out's still-undesigned districts or factions.

> The player needs to reach a supply cache marked on an old transit map, on the other side of a flooded
> PATH tunnel. **But** the tunnel's one working access hatch has been welded shut from the inside by a
> survivor who's using the space as a wind-break shelter and doesn't want to be found. **Therefore**
> the player has to talk their way past, sneak around, or force their way through this survivor to
> reach the cache. **But** forcing the issue — cutting the weld, breaking in loudly — is exactly the
> kind of noise that wakes a dormant automated defense unit that's been sitting powered-down in that
> tunnel since before the Fell Out; it isn't reacting to the player's presence, only to the racket.
> **Therefore** the player now has an active threat to deal with that wasn't part of the original plan,
> with the welded-in survivor's safety hanging on how it's handled. **But** once the defense unit is
> down (or avoided), it turns out the survivor didn't weld themselves in against the cold at all — the
> cache the player's after is sitting next to a grave they dug themselves, and they've been guarding it,
> not hiding from weather. **Therefore** the "simple" fetch-the-cache quest has quietly become a real
> choice: take the cache and leave someone standing over a grave, split it with them, or walk away
> and let them keep all of it.

Notice what this does *not* require: no new lore was invented beyond what's already safe (non-sentient
automated defenses, PATH tunnels, Toronto's radioactive winter). The method's job here isn't to generate
content — it's to find the causal spine and the reversal points, and sequence them so the player feels
each one land instead of just being told about it.

---

## 5. Plot schematics

### 5a. The Linear Escalation Chain (single-thread side quest)

For a quest with one throughline and no branching companion/faction stakes attached:

```
SETUP           — establish what the player wants, and why it looks achievable
   │
   ▼ BUT
COMPLICATION 1  — the obvious path is blocked or costs more than expected
   │
   ▼ THEREFORE
ACTION 1        — player does the thing this complication demands
   │
   ▼ BUT
COMPLICATION 2  — that action created a new, bigger problem (not just "more of the same")
   │
   ▼ THEREFORE
ACTION 2        — player commits further, usually with less room to back out
   │
   ▼ BUT
REVERSAL        — the goalposts move; what the player thought they were solving turns out
                  to be a smaller piece of something else (per Section 4's tunnel example)
   │
   ▼ THEREFORE
RESOLUTION      — player's choice at the climax is shaped by everything above, not just
                  the original setup
```

**Design check:** if you can delete Complication 1 or Complication 2 without changing what the player
does at Resolution, that complication isn't load-bearing — it's an And Then. Every But needs to
change the shape of what comes after it, not just delay it.

### 5b. The Branching Consequence Tree (companion quests, major faction quests)

Toronto Fell Out already has binding design laws for this tier of content — see
`General-Overview-Notes/Design-Philosophy.md`'s **No Good Endings** and **Dual-Outcome Companion Perks +
Companion-Mediated Access** rules. The But/Therefore method is the mechanism that *produces* those
outcomes rather than bolting them on at the end:

```
SETUP
   │
   ▼ BUT
FORK POINT      — a genuine reversal that splits into 2+ paths, not a menu of flavor options.
                  Each path must cost something different, per "No Good Endings."
   │
   ├──▼ THEREFORE (Path A)          ├──▼ THEREFORE (Path B)
   │  ACTION A1                     │  ACTION B1
   │     │                          │     │
   │     ▼ BUT                      │     ▼ BUT
   │  COMPLICATION A2                │  COMPLICATION B2
   │  (different in kind from        │  (different in kind from
   │   B2, not just relabeled)       │   A2, not just relabeled)
   │     │                          │     │
   │     ▼ THEREFORE                │     ▼ THEREFORE
   │  PERK/ACCESS A                  │  PERK/ACCESS B
   │  (per Companion-Mediated        │  (per Companion-Mediated
   │   Access: a new place or        │   Access: a different new
   │   faction opens up)             │   place or faction opens up)
```

**Design check:** if Path A's complication and Path B's complication are the same event with the
names swapped, the fork isn't real — it's cosmetic. The whole point of forking on a "but" is that the
two branches genuinely don't converge back to the same beats. This is also where `Design-Philosophy.md`'s
**Branch count policy** applies (2 branches is the floor, 3 the default target, 4 permitted when earned,
5 a hard cap) — don't fork further than the material actually supports.

### 5c. The Quest Beat Worksheet

A blank, fill-in-the-blank version of 5a, meant to be copy-pasted and actually typed into during
drafting — the point is to force every transition to be explicitly labeled, so a chain of accidental
And-Thens can't hide:

```
Quest: ___________________________     Context/Storyline thread: ___________________________

SETUP:            ______________________________________________
   BUT             ______________________________________________
COMPLICATION 1:    ______________________________________________
   THEREFORE       ______________________________________________
ACTION 1:          ______________________________________________
   BUT             ______________________________________________
COMPLICATION 2:    ______________________________________________
   THEREFORE       ______________________________________________
ACTION 2:          ______________________________________________
   BUT             ______________________________________________
REVERSAL:          ______________________________________________
   THEREFORE       ______________________________________________
RESOLUTION:        ______________________________________________

Self-check: could any BUT line above be deleted without changing what the player
does two lines later? If yes, that BUT is an AND THEN in disguise — rewrite it.
```

---

## 6. How this interacts with Toronto Fell Out's own standing design laws

This method is a generator, not a replacement for the project's existing narrative rules. When
drafting a quest chain, route the "But" reversal points through whichever of these already applies —
all documented in `General-Overview-Notes/Design-Philosophy.md`, Toronto Fell Out's own canonical design
laws (not Inner Tepenia's memory-tagged equivalents):

- **No Good Endings** — a companion-branch "But" should cost something real, not just look
  dramatic. If a reversal doesn't force a genuine trade-off, it's decoration.
- **Dual-Outcome Companion Perks + Companion-Mediated Access** — a Fork Point (5b) is usually where a
  companion questline's mutually exclusive perks actually originate. Design the fork first; the perks
  should fall out of what each branch's "Therefore" naturally grants, not get bolted on afterward. Each
  branch's final "Therefore" is also a natural place to grant the new location/faction access this law
  separately requires.
- **Minimum Five Solutions** — non-story-gated quests and skill checks should offer at least five
  distinct ways to pass. A Fork Point in 5b can be a natural home for several of those five, since each
  branch's Action beats are themselves alternate approaches.
- **Branch count policy** — see 5b above.

**Not carried over from Inner Tepenia's version of this document:** references to a "Cross-DLC Bypass
Design Law" and an "XP Lump-Sum Model" — both tied to Inner Tepenia's own DLC-item-gifting and XP-payout
systems, neither of which Toronto Fell Out has an equivalent of yet. If Toronto Fell Out designs its own
version of either system later, this section is the place to add the cross-reference.

---

## 7. Before calling a quest draft done

Read the chain top to bottom using only the conjunctions (skip the content). If it reads
**But-Therefore-But-Therefore** all the way down with no run of two or more Therefores (or two or more
Buts) in a row, and no beat that could be deleted without consequence, the quest has the shape the
method is looking for. If it reads like a list with "but"/"therefore" stapled on, go back to Section 3.
