---
title: "Improve syntax documentation"
date: "2026-11-10"
status: "active"
sponsor: ""
lead: "Petr Viktorin"
summary: "Reword the syntax chapters of the Python Language Reference to match current Python: an overview and common uses first, then increasingly complex details, ending with the formal grammar."
project_issue: "https://github.com/python/editorial-board/issues/48"
weight: 10
links:
  - url: "https://github.com/python/cpython/issues/135676"
  - url: "https://github.com/python/cpython/issues/141984"
  - title: "Python Language Reference"
    url: "https://docs.python.org/3/reference/index.html"
---

## Description

1. Reword each section of the syntax chapters of the
   [Python Language Reference](https://docs.python.org/3/reference/index.html):
    - [x] Lexical analysis
    - [ ] Expressions
    - [ ] Simple statements
    - [ ] Compound statements
    - [ ] Top-level components
2. Synchronize the documented formal grammar with Python's actual grammar.
   (Both will need changing.)
3. Automatically generate as much of the formal grammar snippets as possible.
4. Add railroad diagrams to the docs.
5. Move the non-syntax chapters (Data model, Execution model, The import
   system) out of the Language Reference, and possibly rename it to
   *Python Syntax Reference*.

## Benefits

Better syntax docs that match current Python.

## Decisions

- Is this a good direction?
- Is the style good? See the mostly finished
  [Lexical analysis](https://docs.python.org/3/reference/lexical_analysis.html)
  chapter and the [current work](https://github.com/python/cpython/issues/141984)
  on Expressions.

## Challenges and risks

- There is an abrupt change in style between the rewritten chapters and the
  rest that is still untouched.
- The work is moving slowly, and depends on one person.

## How to help

The lead is not looking for people to take this on, since reviewing would be
as hard as writing. Feedback on the direction and style is welcome. The work
happens on weekly livestreams: see the
[Python Docs Discord](https://discord.gg/nXkJ2JYvCu).
