# Java Mastery Roadmap

A single-file, offline Java learning roadmap and problem bank. Open `index.html` in any
browser — no build step, no dependencies, no internet required.

## What is inside

**Roadmap — 12 levels, 152 topics.** Every topic card opens a detail view with:

- a plain-language explanation of the concept
- a short, runnable code example
- a practice problem
- the full solution

Progress is tracked per topic and saved in your browser's `localStorage`.

| # | Level | # | Level |
|---|---|---|---|
| 1 | Java Fundamentals | 7 | Multithreading |
| 2 | Object-Oriented Programming | 8 | JVM |
| 3 | Exception Handling | 9 | JDBC & SQL |
| 4 | Collections Framework | 10 | DSA with Java |
| 5 | Advanced Core Java | 11 | Spring & Spring Boot |
| 6 | Functional Programming | 12 | Backend Development |

**Problems — 164 LeetCode-style problems, grouped by topic.** 23 topic sections
(Arrays, Two Pointers, Hashing, String, Linked List, Stack, Queue, Heap, Tree, BST,
Graph, Trie, Union-Find, Backtracking, Greedy, DP, and more). Difficulty mix is
44 Easy / 84 Medium / 36 Hard.

Each problem shows the statement, a Java solution in LeetCode submission style, and a
link to search the problem on LeetCode. Search, difficulty filter, topic filter, and a
"Solved at top" toggle are all available. Solved problems are saved separately from
roadmap progress, so the two never interfere.

## Using it

Just open `index.html`. To serve it locally instead:

```bash
python -m http.server 8000
# then visit http://127.0.0.1:8000/
```

## Features

- Dark and light theme, remembered for the session
- Search and difficulty filters on both views
- "Continue" jumps to your first incomplete topic
- Per-level and per-topic collapse
- Progress bars at the roadmap level, the topic level, and per problem section
- Responsive layout, works on a phone
- Respects `prefers-reduced-motion`

## Notes

The file is fully self-contained: no external stylesheets, fonts, or scripts, and nothing
is fetched at runtime. Your progress lives only in your own browser and is never sent
anywhere.

Solutions are written to be readable teaching examples. They have not been compiled or
run against LeetCode's test harness, so treat them as a reference rather than a
guaranteed-correct submission.