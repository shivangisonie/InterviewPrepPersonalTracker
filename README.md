# Senior SWE Interview Prep — 4 Week Plan

A four-week coding-round plan for an experienced engineer who is **rusty rather than new**, budgeting **~12–13 hours per week** (1–1.5 hrs on weekdays, 3–4 hrs on weekend days).

Covers three round formats:

- **Classic DSA** — 1–2 algorithm problems in 45 minutes
- **Practical / API building** — build a working feature over 60–90 minutes with iterative requirements
- **Low-level / object-oriented design** — model a system in code

System design (distributed / architecture) is explicitly **out of scope** and handled separately.

> [!NOTE]
> Problem links go to LeetCode. Target is ~55 unique problems + ~20 deliberate redos over the month — that is the realistic ceiling at this time budget, and it is enough.

## Contents

- [Ground rules](#ground-rules)
- [Week 1 — Pattern re-acquisition](#week-1--pattern-re-acquisition)
- [Week 2 — Trees, graphs, heaps](#week-2--trees-graphs-heaps)
- [Week 3 — DP, backtracking, first practical build](#week-3--dp-backtracking-first-practical-build)
- [Week 4 — Consolidation and simulation](#week-4--consolidation-and-simulation)
- [Redo queue](#redo-queue)
- [If you fall behind](#if-you-fall-behind)
- [Known coverage gaps](#known-coverage-gaps)

---

## Ground rules

These matter more than the problem list.

### 1. Pick one language today and never switch

Python costs the fewest keystrokes under time pressure; C# or TypeScript are fine if that is where you are fluent. Whatever you pick, memorize its heap, sorted-container, and default-dict equivalents cold.

- [ ] Language chosen: `__________`
- [ ] Wrote a scratch file exercising heap / sort-with-comparator / dict-of-lists from memory

### 2. Turn off autocomplete and AI assist while practicing

This is the single biggest trap for a working engineer. You write code all day with a copilot; the interview will not have one. Practice in a plain editor or in the real tool (CoderPad, HackerRank, CodeSignal).

- [ ] Practice environment set up with assist disabled

### 3. Run a redo queue

Any problem that took **>35 min** or needed a hint goes on the [redo queue](#redo-queue) with a date. Redo it from scratch at **+3 days** and **+10 days**. Re-solving beats new volume for retention — expect ~30% of your problem slots to be redos by week 3.

### 4. Timebox hard

```
25 min  attempt
10 min  read the editorial
 5 min  write a two-line "pattern trigger" note
```

Example trigger note: *"sorted array + pair sum → two pointers."* Do not grind a single problem for 90 minutes; that is how rusty people burn a week on three problems.

### 5. Narrate out loud from week 2 onward

Senior candidates get dinged for silent solving far more often than for a suboptimal complexity.

---

## Week 1 — Pattern re-acquisition

Arrays through stacks. Two problems per weekday. **Untimed** Mon–Tue, **timed** from Wed onward.

### Mon — Hashing
- [ ] [Two Sum](https://leetcode.com/problems/two-sum/)
- [ ] [Group Anagrams](https://leetcode.com/problems/group-anagrams/)
- [ ] [Longest Consecutive Sequence](https://leetcode.com/problems/longest-consecutive-sequence/)

### Tue — Two pointers
- [ ] [Container With Most Water](https://leetcode.com/problems/container-with-most-water/)
- [ ] [3Sum](https://leetcode.com/problems/3sum/)

### Wed — Sliding window
- [ ] [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/)
- [ ] [Minimum Window Substring](https://leetcode.com/problems/minimum-window-substring/)

### Thu — Binary search
- [ ] [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/)
- [ ] [Koko Eating Bananas](https://leetcode.com/problems/koko-eating-bananas/)

### Fri — Stacks / monotonic stack
- [ ] [Valid Parentheses](https://leetcode.com/problems/valid-parentheses/)
- [ ] [Daily Temperatures](https://leetcode.com/problems/daily-temperatures/)

### Sat (3–4h) — LLD foundations
Learn the format before doing a problem:

```
clarify requirements  →  list entities  →  sketch classes + interfaces
                      →  implement one class fully  →  answer an extension question
```

- [ ] Read/absorb the five-step format above
- [ ] **Design a Parking Lot** — end to end, in real code, not just boxes

### Sun (3h) — Consolidation
- [ ] Four timed problems mixed from the week
- [ ] Populate the redo queue
- [ ] Write down which patterns you failed to **recognize** vs. failed to **implement** — that distinction drives week 4

---

## Week 2 — Trees, graphs, heaps

Start narrating out loud this week, even when practicing alone.

### Mon — Tree recursion
- [ ] [Invert Binary Tree](https://leetcode.com/problems/invert-binary-tree/)
- [ ] [Diameter of Binary Tree](https://leetcode.com/problems/diameter-of-binary-tree/)
- [ ] [Lowest Common Ancestor of a BST](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree/)

### Tue — BST and harder trees
- [ ] [Validate Binary Search Tree](https://leetcode.com/problems/validate-binary-search-tree/)
- [ ] [Kth Smallest Element in a BST](https://leetcode.com/problems/kth-smallest-element-in-a-bst/)
- [ ] [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/)

### Wed — Graph BFS / DFS
- [ ] [Number of Islands](https://leetcode.com/problems/number-of-islands/)
- [ ] [Clone Graph](https://leetcode.com/problems/clone-graph/)
- [ ] [Rotting Oranges](https://leetcode.com/problems/rotting-oranges/)

### Thu — Topological sort and union-find
- [ ] [Course Schedule](https://leetcode.com/problems/course-schedule/)
- [ ] [Course Schedule II](https://leetcode.com/problems/course-schedule-ii/)
- [ ] [Redundant Connection](https://leetcode.com/problems/redundant-connection/) — union-find

### Fri — Heaps and intervals
- [ ] [Merge Intervals](https://leetcode.com/problems/merge-intervals/)
- [ ] [Task Scheduler](https://leetcode.com/problems/task-scheduler/)
- [ ] [Merge k Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/)

### Sat (3–4h) — LLD block two
- [ ] [LRU Cache](https://leetcode.com/problems/lru-cache/) — implement properly with hashmap + doubly linked list; this is LLD and DSA at once
- [ ] **Design a Rate Limiter** with two strategies (token bucket, sliding window) behind one interface

Extensibility through interfaces is the thing actually being graded.

### Sun (3h) — First mock
- [ ] 45-minute mock: two problems, out loud, **recorded**
- [ ] Watch the recording back — painful, high yield
- [ ] Redo queue

Use [interviewing.io](https://interviewing.io) or [Pramp](https://www.pramp.com) for a real human if you can.

---

## Week 3 — DP, backtracking, first practical build

### Mon — Backtracking
- [ ] [Subsets](https://leetcode.com/problems/subsets/)
- [ ] [Combination Sum](https://leetcode.com/problems/combination-sum/)
- [ ] [Word Search](https://leetcode.com/problems/word-search/)

### Tue — 1-D DP
- [ ] [House Robber](https://leetcode.com/problems/house-robber/)
- [ ] [House Robber II](https://leetcode.com/problems/house-robber-ii/)
- [ ] [Coin Change](https://leetcode.com/problems/coin-change/)
- [ ] [Longest Increasing Subsequence](https://leetcode.com/problems/longest-increasing-subsequence/)

### Wed — 2-D DP
- [ ] [Unique Paths](https://leetcode.com/problems/unique-paths/)
- [ ] [Longest Common Subsequence](https://leetcode.com/problems/longest-common-subsequence/)
- [ ] [Word Break](https://leetcode.com/problems/word-break/)

### Thu — Tries
- [ ] [Implement Trie (Prefix Tree)](https://leetcode.com/problems/implement-trie-prefix-tree/)
- [ ] [Design Add and Search Words Data Structure](https://leetcode.com/problems/design-add-and-search-words-data-structure/)

### Fri — Linked lists and bits (cheap points)
- [ ] [Reverse Linked List](https://leetcode.com/problems/reverse-linked-list/)
- [ ] [Reorder List](https://leetcode.com/problems/reorder-list/)
- [ ] [Single Number](https://leetcode.com/problems/single-number/)

### Sat (4h) — Practical round simulation

Build an **in-memory key-value store with TTL expiry** from scratch, with tests, in 90 minutes.

- [ ] Block 1 (90 min): `get` / `set` / `delete`, TTL expiry, unit tests
- [ ] Block 2 (45 min): add two requirements you did **not** plan for — an LRU eviction cap, and a `compareAndSwap` operation

The iterative-requirements shape is exactly what Stripe-style rounds do. The skill being graded is whether your first design absorbs change gracefully.

> [!TIP]
> A transactional ledger with idempotency keys is an equally good practice target, and plays to a billing/payments background.

### Sun (3h) — Second mock
- [ ] 45-minute mock, out loud
- [ ] Redo queue

---

## Week 4 — Consolidation and simulation

**No new topics.** This week is about recall under pressure.

### Weekdays (1–1.5h each)
One timed 45-minute round per day: two problems **drawn at random** across all topics, narrated, no hints. Then 20 minutes on the redo queue.

- [ ] Mon — timed round + redos
- [ ] Tue — timed round + redos
- [ ] Wed — timed round + redos, plus a 30-min **verbal** LLD walkthrough, no code (Vending Machine or Elevator System)
- [ ] Thu — timed round + redos
- [ ] Fri — timed round + redos

Random draw is the whole point: in weeks 1–3 you always knew the topic in advance, and **pattern recognition** is what actually fails in a real interview.

### Sat (4h)
- [ ] Extend the week-3 project with a feature you have not thought about (persistence, or pub/sub on key changes)
- [ ] LLD #4 — **Splitwise** or **Notification Service**

### Sun — Full loop simulation
- [ ] 45-min DSA round
- [ ] 45-min DSA round
- [ ] 60-min LLD round

Back to back, with real breaks. This tells you what your fatigue curve looks like, which is genuinely useful information.

- [ ] Taper: light redos only for the following few days

---

## Redo queue

Anything that took >35 min or needed a hint. Redo from scratch at +3 and +10 days.

| Problem | First attempt | Why it went on the list | Redo +3 | Redo +10 |
|---|---|---|:---:|:---:|
| | | | ☐ | ☐ |
| | | | ☐ | ☐ |
| | | | ☐ | ☐ |
| | | | ☐ | ☐ |
| | | | ☐ | ☐ |

---

## If you fall behind

Cut in this order:

1. 2-D DP (Wed, week 3)
2. Tries (Thu, week 3)
3. Bit manipulation (part of Fri, week 3)

> [!IMPORTANT]
> Never cut graphs, the mocks, or the redo queue. Two mocks with real feedback beat twenty extra solved problems.

---

## Known coverage gaps

Deliberately skipped, because at senior level they are rare enough that the time is better spent elsewhere:

- Segment trees / Fenwick trees
- Advanced string algorithms (KMP, suffix arrays, Z-algorithm)
- Math-heavy and number-theory problems
- Concurrency-flavored coding rounds

Add them back only if you are targeting a company known to ask for them.
