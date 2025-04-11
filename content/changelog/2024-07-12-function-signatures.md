---
author: ["Ned Batchelder"]
title: "Function signatures include slash and star"
date: "2024-07-12"
tags: ["changelog"]
categories: ["changelog"]
series: ["Changelog"]
ShowToc: false
TocOpen: false
---

Function signatures should include slash and star: https://github.com/python/devguide/pull/1344

## Summary

If a function accepts positional-only or keyword-only arguments, include the
slash and the star in the signature as appropriate.

```rst
.. function:: some_function(pos1, pos2, /, pos_or_kwd, *, kwd1, kwd2):
```

Although the syntax is terse, it is precise about the allowable ways to call
the function and is taken from Python itself.

The CPython Devguide has been updated to reflect [this recommendation](https://devguide.python.org/documentation/style-guide/#function-signatures).
