---
author: ["Ned Batchelder"]
title: "Timezone vs time zone"
date: "2024-07-18"
tags: ["changelog"]
categories: ["changelog"]
series: ["Changelog"]
ShowToc: false
TocOpen: false
---

Clarify `timezone` vs "time zone": https://github.com/python/devguide/pull/1352

## Summary

The CPython PR [#118449](https://github.com/python/cpython/pull/118449) updates the spelling of "timezone" to "time zone".
There was a discussion
on the PR that the "timezone" spelling is also acceptable and have been used within the CPython docs
consistently. However, both Wikipedia and The Free Dictionary redirect "timezone" to "time zone".

Using the two-word form "time zone" would help separate the concept from the "timezone" class in Python.

The [Style Guide](https://devguide.python.org/documentation/style-guide/#style-guide) section on CPython Devguide has
now been updated with the recommendation of using the
two word `time zone` when referring to the real-world time concept, and to use the one word `timezone` with
appropriate code markup when referring to a Python term.

