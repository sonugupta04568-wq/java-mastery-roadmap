# Programming Roadmaps and Problem Bank

A single-file, offline learning page: roadmaps for Java, C++ and Python, a
topic-grouped problem bank, and a syntax reference for seven languages. Open
`index.html` in any browser — no build step, no dependencies, no internet required.

## What is inside

The page has three tabs.

### Roadmap — Java, C++ and Python

Switch language with the selector at the top of the tab. Each roadmap is 12 levels
and every topic card opens a detail view with:

- a plain-language explanation of the concept
- a short, runnable code example
- a practice problem
- the full solution

**Java — 152 topics**

| # | Level | # | Level |
|---|---|---|---|
| 1 | Java Fundamentals | 7 | Multithreading |
| 2 | Object-Oriented Programming | 8 | JVM |
| 3 | Exception Handling | 9 | JDBC & SQL |
| 4 | Collections Framework | 10 | DSA with Java |
| 5 | Advanced Core Java | 11 | Spring & Spring Boot |
| 6 | Functional Programming | 12 | Backend Development |

**C++ — 113 topics:** Foundations, Functions and Scope, Classes and Objects,
Inheritance and Polymorphism, Pointers and Memory, STL Containers, STL Algorithms and
Iterators, Strings/Streams/Files, Exceptions, Templates and Generic Code, Concurrency,
Modern C++.

**Python — 113 topics:** Foundations, Built-in Data Structures, Functions, Modules and
Packages, OOP, Errors and Exceptions, Files/Paths/Data, Standard Library Tour,
Functional Techniques, Data Structures from Scratch, Algorithms and Complexity,
Concurrency and Async.

Progress is tracked per topic, saved separately per language in `localStorage`
(`jmr-progress`, `jmr-progress-cpp`, `jmr-progress-py`), so the three roadmaps never
interfere.

**Problems — 164 LeetCode-style problems, grouped by topic.** 23 topic sections
(Arrays, Two Pointers, Hashing, String, Linked List, Stack, Queue, Heap, Tree, BST,
Graph, Trie, Union-Find, Backtracking, Greedy, DP, and more). Difficulty mix is
44 Easy / 84 Medium / 36 Hard.

Each problem shows the statement, a Java solution in LeetCode submission style, and a
link to search the problem on LeetCode. Search, difficulty filter, topic filter, and a
"Solved at top" toggle are all available. Solved problems are saved separately from
roadmap progress, so the two never interfere.

### Languages — 101 syntax topics across 7 languages

A syntax reference you can scan and copy from, covering **C (13 topics), C++ (16),
Python (16), JavaScript (17), SQL (15), Java (11) and Bash (13)**. Each topic shows a
one-line explanation and a runnable example.

Two cross-language cheat sheets sit at the top of the tab:

- **Same task in C, C++, Python and JavaScript** — hello world, declaring a variable,
  conditionals, loops, functions, dynamic arrays, maps, custom types, freeing memory,
  and how to build and run.
- **Includes and imports across languages** — how each of the six languages pulls in a
  standard library, one of your own files, a whole namespace, a single renamed item,
  and where on disk it searches for them.

Each language also has its own imports topic (`#include` for C and C++, `import` for
Python, JavaScript and Java, `source` for Bash).

The C, C++, Python, JavaScript and Bash examples were compiled and executed while being
written; the SQL examples follow one consistent `employees` / `departments` schema.

## Using it

Just open `index.html`. To serve it locally instead:

```bash
python -m http.server 8000
# then visit http://127.0.0.1:8000/
```

## Features

- Three tabs: Roadmap, Problems and Languages, switched with `1`, `2` and `3`
- Three roadmaps in the first tab: Java, C++ and Python, each with independent progress
- On a wide screen the Roadmap tab grows a sticky level sidebar with live progress,
  and the page widens from 1000px to 1240px
- `Ctrl`+`K` opens a command palette that searches all 378 roadmap topics, 164
  problems and 101 syntax topics at once, and jumps straight to them
- `j` / `k` move between cards, `x` ticks the focused card
- Problem grid has a compact / comfortable density toggle
- Dark and light theme, remembered for the session
- Search and difficulty filters on every tab
- "Continue" jumps to your first incomplete topic; "Next unsolved" does the same
  for the problem bank
- copy-to-clipboard on every code block and on both comparison tables
- toast notifications for every completion
- back-to-top floating button once you scroll past the hero
- progress bars at the roadmap level, the topic level, per problem section and per
  language
- per-level, per-topic and per-language collapse
- progress, filters, active tab and active roadmap persist across reloads
- responsive layout: bottom-sheet dialogs and scrollable tab strips on a phone
- respects `prefers-reduced-motion`

## Notes

The file is fully self-contained: no external stylesheets, fonts, or scripts, and nothing
is fetched at runtime. Your progress lives only in your own browser and is never sent
anywhere.

Solutions are written to be readable teaching examples. They have not been compiled or
run against LeetCode's test harness, so treat them as a reference rather than a
guaranteed-correct submission.