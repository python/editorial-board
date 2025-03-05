---
author: ["Mariatta"]
title: "Meeting Minutes: Feb 11, 2025"
date: "2025-02-11"
description: "Meeting Minutes from Python Docs Editorial Board: February 11, 2025"
summary: "Meeting Minutes from Python Docs Editorial Board: February 11, 2025"
tags: ["minutes"]
categories: ["minutes"]
series: ["Meeting Minutes"]
ShowToc: false
TocOpen: false
members: ["Guido van Rossum", "Joanna Jablonski", "Mariatta", "Ned Batchelder"]
guests: ["Adam Turner"]
---

### Agenda


* Doc audit
* [https://github.com/sphinx-doc/sphinx/pull/13242](https://github.com/sphinx-doc/sphinx/pull/13242) -- technicalities about 'or' vs. '|' in Sphinx ':type:' constructs. There appears to be growing support for sticking with '|'
* Star/Slash in function signatures

### Notes



* Docs audit for argparse: see the “Docs Audit: argparse” doc in resources
    * Looks like a good start
    * Joanna and Savannah will be collaborating on this in the doc at first
        * With some updates in the EB Discord
    * They don’t currently need anything from the Board at the moment
        * They will pull us in if needed
* Pipes vs “or” in Sphinx type descriptions?
    * [https://discuss.python.org/t/how-should-we-mark-up-multiple-types-in-a-type-field/48196/30](https://discuss.python.org/t/how-should-we-mark-up-multiple-types-in-a-type-field/48196/30)
    * Adam Turner joins to help
    * Adam’s view: we should adopt type annotation syntax
        * When that doesn’t work (no type, or “file-like”, etc) we should leave the annotation blank, but still write out the English
        * There are three places type information can appear:
            * The function signature, which should look like Python code
                * If an argument is “file like”, it should be omitted here.
            * The argument bullet list
                * This is the awkward place: types are parsed here with AST.
                    * Sphinx possibilities:
                        * Allow quoted strings, omit the quotes when rendering, and cross-link if the term is in the glossary.
                        * Try to parse with AST, if it fails, parse with tokenize
            * English prose in paragraph form
                * If an argument is “file like”, it should be fully described here.
    * Plan:
        * For non-formal types, use glossary cross-references
        * Use pipes instead of prose where possible
        * Implementation
            * Allow quoted strings as the type annotation
            * Unify parsing of field-list style and annotation-style
            * Start with custom code for CPython to not have to wait for Sphinx release
            * But goal is to upstream it to Sphinx
        * Update the discuss.python.org thread with the decision.
* Star/Slash in function signatures
    * We want signatures to be precise: if arguments are positional, use a slash, even if there is only one argument.
    * We will experiment with Sphinx tooling to provide a link on the slash and star.
    * We looked at underline for slash, it was distracting and drew attention to the slash, when most people argue that the slash is already too distracting
    * Hover text is a good fallback if a link isn’t an option.

