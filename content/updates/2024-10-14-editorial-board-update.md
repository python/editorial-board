---
author: [""]
title: "Meeting Minutes: Oct 14, 2024"
date: "2024-10-14"
description: "Meeting Minutes from Python Docs Editorial Board: October 14, 2024"
summary: "Meeting Minutes from Python Docs Editorial Board: October 14, 2024"
tags: ["minutes"]
categories: ["minutes"]
series: ["Meeting Minutes"]
ShowToc: false
TocOpen: false
members: ["Carol Willing", "Guido van Rossum", "Mariatta", "Ned Batchelder"]
---

### Agenda

* Contribution Guide progress
* Modernizing Python Docs

### Notes


* Contribution Guide progress
    * PR created, approved.
        * PR build: [https://cpython-devguide--1426.org.readthedocs.build/](https://cpython-devguide--1426.org.readthedocs.build/) 
        * PR: [https://github.com/python/devguide/pull/1426](https://github.com/python/devguide/pull/1426)	
    * Status:
        * There is a new section within the current Devguide: “(draft)” item on the left menu.
    * How do we feel about it landing on main right now?
        * Worried about people ending up in the draft accidentally and thought it’s the real one.
        * There is an info box at the top of each contrib guide saying it’s a WIP. 
        * Example: [https://cpython-devguide--1426.org.readthedocs.build/contrib/intro/](https://cpython-devguide--1426.org.readthedocs.build/contrib/intro/)	there is a box at the top.
        * [Ned TODO] Add the plan of this new contrib guide under “Introduction”
        * [Ned TODO] embolden the section head in side bar also.
    * How can people discover this?
        * [devguide.python.org/contrib](devguide.python.org/contrib)
        * Or look for the menu item
    * Concerns with merging
        * Linking concerns?
        * Plan: flesh out the pages that don’t exist first. Then move things around later?
        * We use Sphinx include directives.
    * Make sure existing devguide maintainers and docs wg community take one last look
        * Hugo, Jelle, Ezio, Petr
    * DevGuide landing page, has a Quick Reference. It goes straight to code contribution. Feedback from people: it’s not relevant to doc contribution. Need a better pathway.
    * Move the Quick reference to the code contribution. 
    * On the landing page there is the table for contribution paths, we can move that up.
        * Instead of table with many rows, it could be a table with two rows and bullet lists.
        * We could use tabs too?
    * What’s the next steps after merging?
        * Ned will write up the plan
        * Talk to people mentioned above
        * Merge the PR
        * More todo items from above
        * Get feedback from people interested in writing sections and see it grow
    * Do people want to be “codeowners” on the new contrib guide?
        * Maybe eventually

* Modernizing Python Docs (Mariatta)
    * Inspiration [https://docs.astro.build](https://docs.astro.build)
    * tutorials.python.org built with new content and new tech
    * What is the vision?
    * Guido would like to see a smaller project using this new/other technology.
    * We can frame it as “PDEB wants to try things out and will solicit feedback from the community.”
    * Maybe take existing tutorials/how to and see how it works on this new tech.
    * See also [https://mystmd.org/](https://mystmd.org/)
      * Alternative tech that has JS interactivity
    * Start with a small prototype of a tutorial
        * Slice tutorial?


