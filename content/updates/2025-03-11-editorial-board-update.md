---
author: ["Mariatta"]
title: "Meeting Minutes: Mar 11, 2025"
date: "2025-03-11T14:11:49-07:00"
description: "Meeting Minutes from Python Docs Editorial Board: Mar 11, 2025"
summary: "Meeting Minutes from Python Docs Editorial Board: Mar 11, 2025"
tags: ["minutes"]
categories: ["minutes"]
series: ["Meeting Minutes"]
ShowToc: false
TocOpen: false
members: ["Carol Willing", "Guido van Rossum", "Joanna Jablonski", "Mariatta", "Ned Batchelder"]
---

### Agenda

* [Docs audit with Savanna](https://docs.google.com/document/d/10MSDlxmgPex3ZGVr-4OggI2lqSAlv_0OTDchGlrLIkk/edit?usp=sharing) is on hold while she deals with other commitments
* [https://github.com/python/editorial-board/issues/25](https://github.com/python/editorial-board/issues/25) (translation management) (issue is closed)

### Notes

* Wiki:
    * Carol went to Docs WG meeting last week. Discussion about the wiki. It is outside of EB’s focus. But we should not link to the wiki from Python docs.
    * It would be great to have an Educational Landing page -> for a Python user, it would be better to have it instead of the wiki.python.
    * Wiki is not a PSF-owned infrastructure? 
    * We have many links (~20) to the wiki from cpython repo. Most were old what’s new docs.
    * We will update and unlink (?)
    * Maybe write in Devguide about the status about wiki.p.o. It is a community-run resource, it has implied authority beyond its actual authority.
* Translations is doing well, now there is a translations dashboard https://python-docs-translations.github.io/dashboard/
* Issue 25 is now closed, opened a Discourse instead [https://discuss.python.org/t/pep-545-update-pep/83534/](https://discuss.python.org/t/pep-545-update-pep/83534/)
* There is now typing.python.org 
    * Why is it separate from docs.python.org?
    * It’s maintained by typing council.
    * A set of standards for type checkers (which are not maintained by Python core)
    * Should we explain all the different (something).python.org -> specifically wiki and typing
    * Add writeup in devguide about which ones are Core Python docs, and there are things like packaging.
    * Should we add typing.python.org as “not in scope” in our charter doc?
    * The typing.p.o docs aren't tied to CPython version
* Carol received comment from a Linux conference attendee, last few Python releases have been easy to install.
* Ned is still going on with Devguide reorg (Initially we set a due date to get it done by PyCon US - PyCon US is in 2 months)
*  “Or” vs “|” in the docs. 
    * Feb 11 notes: prefer | instead of “or”. We should write it to our changelog [https://github.com/python/editorial-board/blob/main/CHANGELOG.md](https://github.com/python/editorial-board/blob/main/CHANGELOG.md)
    * [https://github.com/python/editorial-board/issues/7](https://github.com/python/editorial-board/issues/7) 
    * It depends on the Sphinx’ capability. It is supported in latest Sphinx and docs are now built using latest Sphinx.
* Need to go back in our notes and backfill the Changelog.md file
* The Docs WG are to ask the PSF to pay for the translation tools.

