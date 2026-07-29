# QA Bug Report Template

A standard template for logging bugs found during testing of Toronto Fell Out. Copy the **Bug Report Fields**
section below for each new bug and fill it in. The **Field Definitions** section explains what belongs in
each field and how to choose severity/priority/status consistently across the team. The **Example** section
at the bottom shows a filled-out report.

---

## Bug Report Fields

```
Bug ID:
Summary:
Reporter:
Date Found:
Build Version / Commit Hash:
Platform:
Related System/Area:
Severity:
Priority:
Frequency:
Status:

Steps to Reproduce:
1.
2.
3.

Expected Behavior:

Actual Behavior:

Screenshots / Video:

Related Bugs / Duplicate Of:

Regression? (Y/N, and last known-good build if Y):

Workaround (if any):

Notes / Additional Context:
```

---

## Field Definitions

**Bug ID**
A unique identifier for the bug (e.g., an incrementing number, or whatever ID your tracker assigns
automatically). Used to reference this bug from other bugs, commits, or design docs.

**Summary**
A single-sentence description of the bug, specific enough to be understood at a glance in a list of a
hundred other bug summaries. Prefer "Companion HP bar doesn't update after healing item is used mid-combat"
over "healing bug."

**Reporter**
Who found and logged the bug.

**Date Found**
The date the bug was observed, not the date it was logged (usually the same day, but worth distinguishing if
there's a gap).

**Build Version / Commit Hash**
The exact build, version number, or commit the bug was observed in. Essential for reproducing the bug later
and for confirming a fix actually landed in a subsequent build. If the project doesn't yet have formal build
numbers, use the commit hash or a date-stamped build label.

**Platform**
Operating system, hardware, input method, and any other environment detail that could plausibly affect
reproduction (e.g., "Windows 11, NVIDIA RTX 3070, keyboard/mouse" or "Steam Deck, docked, controller").

**Related System/Area**
Which part of the game the bug touches — combat, dialogue, companion system, inventory, save/load, UI,
audio, a specific quest, etc. Useful for routing the bug to the right person and for spotting clusters of
bugs in the same system.

**Severity**
How badly the bug damages the game if it isn't fixed. This is about *impact*, independent of how often it
happens.
- **Critical** — Crashes, save corruption, data loss, or a bug that makes the game unplayable/unwinnable
  (e.g., a quest-blocking soft-lock with no workaround).
- **High** — Major functionality is broken or clearly wrong (a core system doesn't work as designed, a
  significant visual/audio glitch, a quest that can't be completed through its intended path even if an
  alternate route exists).
- **Medium** — Noticeable but doesn't block progress — a stat displaying incorrectly, a companion line
  playing at the wrong time, a minor visual artifact.
- **Low** — Cosmetic or trivial — a typo, a slightly misaligned UI element, a barely noticeable audio pop.

**Priority**
How soon this should actually be worked on, which is related to but distinct from Severity — a Low-severity
bug that's trivially easy to fix and highly visible (a typo on the main menu) might get fixed before a
Critical bug that only occurs in a rare edge case nobody has reproduced twice. Common scale: **P0** (drop
everything), **P1** (fix this build), **P2** (fix soon), **P3** (fix eventually/backlog).

**Frequency**
How reliably the bug reproduces.
- **Always** — Happens every time the steps are followed.
- **Often** — Happens most of the time, but not every time.
- **Sometimes** — Happens on a noticeable but minority fraction of attempts.
- **Rare** — Happened once or twice out of many attempts; hard to reproduce on demand.
- **Once** — Observed a single time; not yet reproduced at all.

**Status**
Where the bug currently stands in the pipeline.
- **New** — Just logged, not yet triaged.
- **Confirmed** — A second person (usually not the original reporter) has reproduced it.
- **Cannot Reproduce** — Reported, but reproduction attempts have failed; kept open for a set period in case
  it resurfaces, rather than closed immediately.
- **In Progress** — Actively being worked on.
- **Fixed** — A fix has been implemented and is awaiting verification in a build.
- **Verified** — QA has confirmed the fix actually works in a subsequent build.
- **Won't Fix** — Acknowledged, but deliberately not being addressed (with a reason noted in Notes — e.g.,
  extremely low impact, deprecated system, working as intended after review).
- **Duplicate** — Already logged under a different Bug ID; reference it in Related Bugs.

**Steps to Reproduce**
A numbered list specific enough that someone unfamiliar with the bug can follow it and see the same result.
Include starting conditions (save state, character build, location) if they matter.

**Expected Behavior**
What should happen, in plain language — what the design or common sense says the correct outcome is.

**Actual Behavior**
What actually happens instead. Be specific and literal; avoid interpreting *why* it happens here (that's for
whoever investigates the fix) — just describe what was observed.

**Screenshots / Video**
Visual evidence, especially for anything UI-, animation-, or rendering-related. A short clip is often far
more useful than a text description for timing-sensitive or visual bugs.

**Related Bugs / Duplicate Of**
Cross-reference other Bug IDs this one might be connected to, caused by, or a duplicate of.

**Regression?**
Whether this used to work correctly in an earlier build and has since broken. If yes, note the last build
where it was confirmed working — this narrows down which change caused it.

**Workaround**
Any known way for a player (or a tester continuing to play past the bug) to avoid or mitigate the issue.
Not every bug has one; leave blank if none is known.

**Notes / Additional Context**
Anything else relevant — suspected cause, related design intent, links to the relevant design doc section,
or context on why a bug was marked Won't Fix.

---

## Example

```
Bug ID: 0142
Summary: Companion HP bar in the interact wheel doesn't update after a healing item is used on them mid-combat
Reporter: J. Alvarez
Date Found: 2026-07-14
Build Version / Commit Hash: v0.3.2-dev (a91f3c2)
Platform: Windows 11, keyboard/mouse
Related System/Area: Companion System — combat healing interaction
Severity: Medium
Priority: P2
Frequency: Always
Status: Confirmed

Steps to Reproduce:
1. Enter combat with an active human companion.
2. Let the companion take damage until their HP bar (visible in the interact wheel) drops below 50%.
3. Open the interact wheel and select the healing-item option to heal them.
4. Observe the HP bar in the interact wheel after the heal is applied.

Expected Behavior:
The companion's HP bar should immediately update to reflect the restored HP value.

Actual Behavior:
The HP bar stays at its pre-heal value until the interact wheel is closed and reopened, even though the
companion's actual HP (confirmed via a debug readout) is correctly restored.

Screenshots / Video: bug_0142_hp_bar_desync.mp4 (attached)

Related Bugs / Duplicate Of: None known

Regression? Y — confirmed working correctly in build v0.3.0-dev; likely introduced with the interact-wheel
UI refactor between v0.3.0 and v0.3.2.

Workaround: Closing and reopening the interact wheel forces the bar to refresh with the correct value.

Notes / Additional Context: Underlying HP value is correct — this looks like a UI refresh/binding issue
specific to the interact wheel, not an actual healing-logic bug. See `Game-Mechanics/Core-Mechanics/
Companion-System.md`'s "Combat Interaction — Applying Healing Items to a Companion" section for the intended
behavior.
```
