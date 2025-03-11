---
author: ["Mariatta"]
title: "| or 'or' in Sphinx documentation"
date: "2025-03-11"
tags: ["changelog"]
categories: ["changelog"]
series: ["Changelog"]
ShowToc: false
TocOpen: false
---

Additional recommendations in the Style Guide https://github.com/python/devguide/pull/1377/

## Summary

[Discourse](https://discuss.python.org/t/how-should-we-mark-up-multiple-types-in-a-type-field/48196) topic: How
should we mark up multiple types in a type field?

Currently, the Python docs use `|` (pipe) character, similar to how you'd annotate a union of types:

```rst
:param p:
   A parameter that takes an int or a float argument.
:type p: int | float
```

However, the [Sphinx docs](https://www.sphinx-doc.org/en/master/usage/domains/python.html#send_message) says to use the word `or`:

```rst
:param p:
   A parameter that takes an int or a float argument.
:type p: int or float
```

The editorial board's decision was requested on this matter via [issue #7](https://github.com/python/editorial-board/issues/7).

The editorial board discussed this over several meetings, our decision is to use the `|` symbol. We met with Adam Turner
to discuss how this would be implemented in Sphinx. This is supported in the latest version of Sphinx and the CPython
docs have been built using the latest Sphinx.

