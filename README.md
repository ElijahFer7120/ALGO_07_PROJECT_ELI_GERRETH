# AL07: Greedy Claims and Memoization Evidence

Name: [your name]
Partner(s): [names]
My contribution: [brief note, including role changes]

## Run

```powershell
py -3.14 main.py
py -3.14 main.py --n 5
py -3.14 test_assignment.py
```

The --n option is used after enabling Thursday's stage.

## Work Notes

- Payment finding: [one counterexample and what it disproves]
- Saved-answer finding: [one small before/after call comparison and storage tradeoff]
- Pair question/decision: [one useful question and the decision it informed]

Keep observations brief. Append debugging/learnings as useful; no separate report.
Shared code/results are allowed; these observations are in your own words.

Thursday -- Reuse Repeated Answers
1. Follow the memoization lesson/demo. Compare the supplied uncached recurrence with the starter’s equivalent recurrence before adding the cache behavior.
2. Add lookup, hit counting, and storage in calculate_cached. Preserve the recurrence’s answer; do not replace it with a precomputed table or formula.
3. Set ENABLE_MEMOIZATION = True. The supplied driver now accepts --n, its default of 8, and --help. Parser construction is supplied and is not assessed.
4. Compare n=5: both answers are 5; uncached calls are 15; cached calls are 9, including 3 hits, with 6 distinct inputs saved. Explain what these categories count. A hit is already included in calls; do not add it again.
Explain what these categories count: 

5. Check n=0, n=1, another independently known answer, and repeated fresh runs. Check rejection outside the wrapper’s input contract. Ensure a cached zero is recognized. Tests may combine several checks in a small fixture.
6. Rerun Tuesday’s checks. Keep one small before/after call comparison in output and a brief personal observation about reuse versus storage. More calls saved is evidence for these runs, not a measured speedup or universal performance claim.
7. Commit/push the completed shared work. Each member copies a complete runnable version to their own submission folder, runs it there, and adds personal README observations before submitting once.

## Assistance

[Identify supplied files and other help. For AI, name the task/tool and what you
checked, changed, or rejected. No AI use is required.]

## Instructor Comments

[Reserved for instructor feedback.]
