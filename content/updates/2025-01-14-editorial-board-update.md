---
author: ["Mariatta"]
title: "Meeting Minutes: Jan 14, 2025"
date: "2025-01-14"
description: "Meeting Minutes from Python Docs Editorial Board: January 14, 2025"
summary: "Meeting Minutes from Python Docs Editorial Board: January 14, 2025"
tags: ["minutes"]
categories: ["minutes"]
series: ["Meeting Minutes"]
ShowToc: false
TocOpen: false
members: ["Guido van Rossum", "Joanna Jablonski", "Ned Batchelder"]
---

### Agenda


* [https://discuss.python.org/t/getopt-and-optparse-vs-argparse/69618/123](https://discuss.python.org/t/getopt-and-optparse-vs-argparse/69618/123)

### Notes


* Revisiting the “how to mark up types” discussion: [https://discuss.python.org/t/how-should-we-mark-up-multiple-types-in-a-type-field/48196/30](https://discuss.python.org/t/how-should-we-mark-up-multiple-types-in-a-type-field/48196/30)
    * Erlend said “int or float” (our slight preference) would cause a syntax error for attributes in Sphinx.
    * Ned’s quick experiment didn’t cause a syntax error
    * Ned has pinged Erlend in Discord for a clarifying conversation.
    * If it is a tooling issue, we will rule in favor of “int | float”
        * Otherwise, we can rule for “int or float”
* [https://discuss.python.org/t/getopt-and-optparse-vs-argparse/69618/123](https://discuss.python.org/t/getopt-and-optparse-vs-argparse/69618/123)
    * Savannah mentioned an audit
    * Joanna will respond on Discourse, inviting Savannah to participate in a docs audit of the argparse pages.
    * Starting point:
        * Two potential user journeys:
          * Making something more basic. Have flags, take in files
            * Making something with subcommands, like git. How do you structure that?
            * Make them part 1 and part 2 of a how-to?

        * Main docs link to how-to(s) with user journeys + reference docs
    * We’ve long aspired to doing docs audits, this could be a good baby step
        * It is small enough to be approachable
        * It can be a way to educate people about what docs audits are and how to do them
        * It can be a way for us to reach agreement on how we will do docs audits
    * User personas
        * How much of this is needed before starting an audit?
