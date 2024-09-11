---
author: ["Mariatta"]
title: "Meeting Minutes: September 09, 2024"
date: "2024-09-09"
description: "Meeting Minutes from Python Docs Editorial Board: September 09, 2024."
summary: "Meeting Minutes from Python Docs Editorial Board: September 09, 2024."
tags: ["minutes"]
categories: ["minutes"]
series: ["Meeting Minutes"]
ShowToc: false
TocOpen: false
---

### Attendees

* Guido
* Mariatta
* Carol
* Ned


## Notes

* Discuss past action items.
* Catch up about last month:
    * Outline about the DevGuide 
    * DevGuide GitHub project (who will create?)
    * Write the issues (who will write?)
    * Do we publish changes as they are ready, or do we wait until entire reorg is finished?
        * What about existing URLs? (urls from other existing pages)
        * Since we are on readthedocs, it can be mapped from there -> redirect to new pages
        * You can mark pages as orphaned on Sphinx(?) Cam/Hugo might know
        * Do we need to convince others about this approach?
* Publicize the fact that we are actively reorganizing the DevGuide into Contribution Guide (~~TODO: Ned will start a Discourse thread, and will send a link~~)
  * Done https://discuss.python.org/t/refactoring-the-devguide-into-a-contribution-guide/63409
* Some things that document what’s changed between Python versions are better off in the same VCS as the code. Things in the current DevGuide are like that.
  * So we need to define what belongs in Contrib Guide vs CPython docs.
  * Example: Irit’s project is better documented within CPython’s doc. Tracked in https://github.com/python/cpython/issues/119786
* We should go into detail: what our workflow is, and explain where to go for different docs, where are things documented.
* We like the idea of publishing in progress. Unsure about url remapping right away.
* Are we still using the “devguide” sub url? -> should it be “contributing” subdomain.
  * “Devguide” is well known terminology among existing contributors.
  * “Contributors” vs “contributing” . python org url -> can cause confusion when typing out the url
  * We like “contrib” contrib.python.org is chosen as the new url.
  * Ticket created at https://github.com/python/devguide/issues/1393
* Adding a big banner on top saying this doc is being actively re-org.
* We might not want to render pages that are not really ready to be published. (by adding to conf.py ignores)? But also why not render those? When will we render those?
* Another idea: add new pages to main branch, add to “do not render” list, have 2 different rtd sites built using the same repo, different config.
* Sphinx has “if” conditional 
* Who’s available and can do this work during the Sprint? 
    * Mariatta, Ned (remotely)?
* There will be a period of when both versions exist, and we want to keep this period short.
* Tools available to make both versions work. 
