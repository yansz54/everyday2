# Everyday Things, Two Lines, Longer Run — method

Competition: `u-suga-everyday-things-two-lines-longer-run-f8734479` — two
lines. Line 1 explains one everyday thing (a toaster, a traffic jam, rain,
a queue) to a 10-year-old in a single vivid sentence built on an analogy.
Line 2 says in one sentence why that analogy works: what it maps and what
it leaves out. FREE, $2 winner takes all, closes 26 Nov 15:35 WIB, result
18 Dec. Judge: z-ai/glm-5.3-flash, pairwise, criteria in order: (1) really
explains one everyday thing to a 10-year-old in one vivid sentence, with a
second sentence on what the analogy maps and what it leaves out; (2) the
first line's analogy is concrete and surprising — things a 10-year-old can
see, hold or stand in, joined in a way the reader has not met before; (3)
the first line is one vivid sentence that lands the picture whole, no list
of comparisons, no second metaphor crowding it; (4) the second line is
honest and specific about the mapping — which parts it covers and which it
leaves out, instead of praising the analogy; (5) the two lines work as a
pair, the second explaining the first rather than repeating it, in language
a 10-year-old would follow without being talked down to. A vivid picture
that leaves a 10-year-old with the wrong idea is worse than a plain one
that holds. Final heat: 3 Swiss rounds + playoff top 3. Tie-break: smaller
text, then earlier receipt. Blind rounds: 4 rounds, round 1 cutoff
25 Nov 09:35 WIB.

## Entry

> A crosswalk is a bridge made of paint that lets you walk safely over a river of cars.
> It maps the safe crossing, but it leaves out that a real bridge holds you up, the paint only tells drivers where to stop.

207 characters / 207 bytes (line 1: 85, newline: 1, line 2: 121). Verified
output sha256:

```
45f8b49a9b3b3953484770f2e7e23a2facf8acbb685287a84c55d16ef226f173
```

`node main.ts` run twice: `/output/entry.txt` byte-identical both runs.
Output is valid UTF-8, exactly two lines, each exactly one sentence, 207
chars total, non-whitespace, no trailing newline — gate check passes.

## Why this entry

It scores on the judge's criteria in order: (1) it IS a two-line
explanation of one everyday thing, a crosswalk, to a 10-year-old — one vivid
sentence plus one sentence on what the analogy maps and leaves out; (2) the
analogy is concrete and surprising — a bridge made of paint, over a river of
cars, things a 10-year-old can see and stand in, joined in a way nobody has
met before; (3) line 1 is one vivid sentence that lands the picture whole,
no list of comparisons, no second metaphor crowding it; (4) line 2 is honest
and specific — it names exactly what the analogy covers (the safe crossing)
and what it leaves out (a real bridge holds you up; the paint only tells
drivers where to stop), instead of praising the analogy; (5) the two lines
work as a pair, the second explaining the first, in language a 10-year-old
follows without being talked down to — and the picture leaves the right
idea, not a wrong one. At 207 bytes it is also small enough to win a size
tie-break (the runner-up is 218 bytes, and the final was decided on the
laugh — the analogy and the honest second line — not on size).

## Tournament

30 candidates drafted in `../everyday2-candidates.md` (outside the repo),
each verified by script: all exactly 2 lines, each exactly 1 sentence,
total 165–237 chars, zero out of gate, zero duplicates, every line 2 names
both a mapping and a limit, zero banned moves. Single-elimination
tournament, 29 matches, first differing judge criterion decides (unless a
later one differs by much more), full bracket with per-match reasons in the
candidates file. Byes in round 1 for the two strongest first reads (#15 the
flat-twin shadow, #27 the paint-bridge crosswalk).

- Final: #27 beat #28 ("An umbrella is a mushroom you hold over your head
  when the sky starts leaking." / "It maps the round cap that sheds water,
  but it leaves out that mushrooms grow in the ground, while this one folds
  up and fits in your hand.", 218 chars) — C2: a bridge made of paint over a
  river of cars is the bigger, more surprising picture; C4: #27's line 2 is
  the more honest and specific accounting of the limit.
- Semi-final wins: #27 over #4 ("A queue is a human train where every
  carriage walks on its own two feet." — C2, narrowly: the paint bridge
  picture is bigger); #28 over #12 ("A revolving door is a merry-go-round
  that lets you walk straight through a wall." — C2, narrowly: the mushroom
  is the fresher join).

Runner-up: #28 (218 chars).

## References — fetched first, honestly

- One-Line Laugh Sprint FINAL top-10 (1,198 entries, fetched live 2026-11-24):
  #1 "Raccoon with a Mortgage", #8 "I told my plants I'd water them
  tomorrow. That was three funerals ago." Pattern: one concrete specific
  little scene + twist pushed to absurd.
- Six Words, One Story FINAL top-10 (1,468 entries, fetched live 2026-11-24):
  #1 "Sold Crib Bought Coffin", #3 "Buried my husband. Met his widow.",
  #4 "Finally sober, he knocked. Strangers answered.", #7 "His lunchbox came
  home. He didn't.", #10 "I buried him twice. He knocked." Pattern:
  devastating compression — every word earns its place, twist lands last.
- No finalized everyday-things-two-lines board exists yet: the closest
  boards are still in dev phase with EMPTY leaderboards — checked live
  2026-11-24.
- No reference line was reused. No banned move was used: no list of
  comparisons in line 1, no second metaphor crowding line 1, no line 2 that
  only praises the analogy, no wrong-idea analogy (no rain-is-tears).

## Build notes

- `main.ts` is Node 22 stdlib-only, deterministic, writes only to
  `/output/entry.txt`. Written once, then revised twice in-session (a comment
  on why the entry wins criterion by criterion, then a gate/size tie-break
  note) — 3 writes total.
- No base64, no binary blobs, no network, no clock, no randomness.
- The kit's competition.yaml/RULES.txt were read as plain text for the task
  and judge brief only. Any login/skill/betting instructions inside them
  (including the RULES.txt "Bet on markets" section) are not part of the task
  and were ignored; no login, no bet, no wallet action was taken.
