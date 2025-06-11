---
author: ["Mariatta"]
title: "Meeting Minutes: June 10, 2025"
date: "2025-06-10"
description: "Meeting Minutes from Python Docs Editorial Board: June 10, 2025"
summary: "Meeting Minutes from Python Docs Editorial Board: June 10, 2025"
tags: ["minutes"]
categories: ["minutes"]
series: ["Meeting Minutes"]
ShowToc: false
TocOpen: false
members: ["Carol Willing", "Joanna Jablonski", "Mariatta", "Ned Batchelder"]
---

### Agenda:



* [Docs audit with Savanna](https://docs.google.com/document/d/10MSDlxmgPex3ZGVr-4OggI2lqSAlv_0OTDchGlrLIkk/edit?usp=sharing) is on hold
* Education & Outreach working group
* Docs WG read-out
* [https://github.com/python/cpython/pull/135160](https://github.com/python/cpython/pull/135160) 
* Side note from the PR: Translation churn
* Monitoring discuss.python.org

### Notes

* Education & Outreach
    * Mariatta was at their open space at PyCon
    * Kattni, Keith the ee, Nicholas Tollervey, Jeff Jacobson, Sheena were there
        * Photo of the open space:
            https://photos.google.com/share/AF1QipPYYQgHzj32bYsJZk7IHs5acgR-O8cEzJCv67STV6SXxj33PQACa4O5Awn4FZUXeg?pli=1&key=enBoWmo4VFZiMENUM083akFWODNHUXFIY3lpZnZB

    * Tutorial: no one had a clear answer for where newbs should go
    * TODO: find out where they are coordinating online
    * There will be overlap with us
    * Carol: wishes [python.org](python.org) had a definition education landing page
        * “If you are new to programming…”
    * Our Group is chartered with decision about CPython docs
    * Edu group is chartered with outreach 
    * We should have tutorial, it should be in [python.org](python.org)
    * There is a governance overlap. We have interest in seeing a Python tutorial, but should it be in our scope?
    * A tutorial that is targeting beginners, should be more of the focus of the Edu group, not ours
* Docs WG Monthly meeting
    * Carol ran the meeting well. Discussed translations effort. Good progress. There is a doc and process about translations.
    * Process change should be documented on devguide. And also figure out what needs to be changed in the PEPs.
    * Beginner tutorials were discussed during the meeting. Kattni says she will continue organizing the work.
    * Having interactive tutorials will be a minimum for beginner tutorials.
* PR [https://github.com/python/cpython/pull/135160/files](https://github.com/python/cpython/pull/135160/files)
    * “Argument” vs “Parameter”
    * The terms are used informally, so do we need to be precise?
    * Is the effort worth it, since precision users know what the imprecise people mean?
        * If the precision users can’t agree on the term, then leave it alone.
    * Arguing about the right terminology. If we’re not going to agree what difference would it make.
    * See where the community goes? 
    * What’s the downside if the change is not made?
    * Start with smaller surface area to change? Perhaps the c-api folder. Focus there first?
    * But for consistency..
    * It shouldn't update what’s new in older Python versions? Misc.news / (historical artifacts)
    * .py changes should be done separately than .rst changes, same as .c files.
        * To avoid code churn, and to allow doc changes to backport
    * Prefer to keep it as is due to the size of the PR, but would be more open to change if it’s a smaller PR, eg just for a one module.
    * Typing folks might be interested.
    * Consensus: it’s not worth the change compared to the effort discussing it. 
    * TODO: Follow up. Joanna will post a response on the PR.
    * Will include in our Decision log. The above could be general guidance when making doc changes. Sometimes you do need to change code and docs at the same time, but this change was meant to be docs changes and shouldn’t have affected other artifacts. 
* Translations churn
    * It’s ok for docs to move faster and change faster compared to code changes,
    * … except for translations. Any small changes to the docs, reverted the translated content back to english because they weren’t translated yet.
        * TODO: find out from the translators what happens when the source docs change
    * What would the translations group prefer to be notified? 
        * How can we notify them, when would they like to be notified?
        * Can a GitHub action post an issue to the translation repos?
        * AI could help fix tiny translations changes, maybe?
        * Every language translation is a separate group with diverging processes and desires
        * “Best practices in docs translation” discussion: \
[https://discuss.python.org/t/best-practices-in-docs-translation/94427](https://discuss.python.org/t/best-practices-in-docs-translation/94427) 
        * We need to learn more about translations and how each groups work.
        * Lysandros plans to host a Greek translations at PyCon Greece. Said it would be great to have best practises