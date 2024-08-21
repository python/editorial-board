---
author: ["Carol Willing"]
title: "Meeting Minutes: January 8, 2024"
date: "2024-01-08"
description: "Meeting Minutes from Python Docs Editorial Board: January 8, 2024."
summary: "Meeting Minutes from Python Docs Editorial Board: January 8, 2024."
tags: ["minutes"]
categories: ["minutes"]
series: ["Meeting Minutes"]
ShowToc: false
TocOpen: false
---



### Attendees

Carol, Guido, Joanna, Mariatta, Ned

### Agenda

We discussed these questions and worked to answer them.

#### How often will we meet?

We will meet monthly on second Monday each month from 1:30-2:30pm Pacific.

We will work asynchronously most of the time.

Next meeting: February 12, 2024

#### What are our deliverables about process and decisions?

We will produce:

1. Meeting Minutes: Working meeting notes will be summarized and published in repo after each meeting.
2. Process and priorities
    * Decisions will be published in "Recommendation" documents. These would be short documents focused on one topic. They would be published in the repo.
    * Identify what the needs are for the specific section of docs. So that greater community can know the goals when they do sprints etc.
    * We can identify blocking factors and remove them.
    * We write outlines, and the community can write the content. It’s good because it encourages writing new docs instead of modifying existing ones. There have been a lot of big overhaul projects that got swamped by discussions.
3. Agenda gathering for next meeting: Use an issue on the GitHub repo.
4. Focus on content needs and improvements; tone and style guides (not restructuredText style but writing)
5. From the docs landing page, do an annual assessment of each part and identify need/frequency of changes (could be the foundation of a high-level editorial calendar of needs - one section each month)
6. *Idea:* incorporate algolia search to sphinx
7. Python.org vs docs.python.org
    * We should limit ourselves to docs.python.org
    * Share recommendations to python.org for changes about making sure on python.org docs will go to docs.python.org. Reduce multiple paths to wiki and doc landing pages other than docs.python.org when refering to "docs"

#### Will we start implementing the five-year plan partly outlined in the [Language Summit 2020 presentation](https://pyfound.blogspot.com/2020/04/cpython-documentation-next-5-years.html), or do we need to reassess and set a different direction?

The goals mentioned in the first and second years sound great, but I think we should review and see what we want to tackle first.  It could be those goals, or other ones, or a mix.

##### *Year 1 goals (from old presentation)*

* Governance and Workgroup: In progress; TODO: define how we work
* Tutorials: Discussion started about existing tutorial. TODO: Do we have one "official" tutorial? Pathways for getting started (relates to landing page)
* Language Translations: Seems to be going well; TODO: Identify any PyCon sprint focus areas
* Landing Page: Work in progress [Documentation Experience presentation](https://docs.google.com/presentation/d/1ujDv8wViPvAMFAtYCRxSKh-CMUlbjcfVYitsqEI2Ios/edit#slide=id.p) TODO: Work with PSF to remove links to old wiki. This is for many the first stop in finding Python docs.

##### *Year 2 and beyond goals (from old presentation)*

* Evaluate effectiveness
* Documentation sprints
* Annual editorial review

##### Selected priorities for the Editorial Board

* How we can make it easier for people to contribute to docs
* How to make the docs even more accessible
* Modernizing the docs: content, UX, or the mechanics?
  * Editorial board should lead the content priorities
  * Color change, theme, community can do it. (They probably should have a PEP tp the SC for major changes.)
* Better SEO
* Process for the community to ask and bring proposals to EB
  * Let's model this after the SC process
* Encourage more positive and constructive discussions in the Python docs community. Work to reduce lengthy arguments, which are sometimes hostile and dismissive.
* When disagreements are at an impasse, make decisions to reduce those blockages.

**Decisions about documentation can be undone more easily than with code.**

#### How will we stay in touch with the docs community?

Some people have already asked how they can be involved.

Generally, people want to help with writing documentation, so they should be involved with the docs community and not editorial board.

* Published meeting minutes. Clear "how to contact" us.
* We will create the Repo and issue templates.
* Individuals can create an issue to request the topic be added to the agenda. We will discuss at the next scheduled meeting time or asynchronously.

* Can people attend these Editorial Board meetings?

  No. We will use a similar process as the SC.

We discussed the following process considerations:

* Repo is public, but not meant for public discussions.
* Avoid situation where there are many open issues.
* Prefer discussion on Discourse with Documentation tag, instead of on the Editorial Board repo.
* Issue on the Editorial board will lead to discussions on that issue. Is that ok?

  We will follow the existing SC process:
  * Have discussion on Discourse first then link the to an issue on the Editorial Board repo.
  * Any further discussions to continue on the Discourse, or privately by the Editorial Board.
  * There is no further discussions/comments on the repo's issue.

#### What are the things that require the Editorial Board to act on?

* Conflicts on content
* Conflicts on tone and style best practices
* Review of existing documentation and outline editorial needs
* Identify needs for new content
* Identify needs for rewrites
* Provide guidance and guidelines for changes
  See for example, the recent pull request: [https://github.com/python/cpython/pull/107449/files](https://github.com/python/cpython/pull/107449/files) which touches on global style issues.

### Action items

* Contact PSF infra/PSF board about python.org.
* Create a REPO similar to steering-council: python/editorial-board
  * Readme should point to the PEP for Editorial board to create. @Carol to add content.
* Meeting notes: don’t need to include too much details. It doesn’t need review, comments.
* Let’s create a new repo: python/editorial-board. Done. @editorial-board team was also created.
* Need an issue template: on GitHub
  * Need to submit their request into one of two big priorities:
    * 1. Proposing a new idea
    * 2. We need a decision of existing issue.

### Resources

These links give context on the editorial board:

* [PEP 732](https://peps.python.org/pep-0732/)
* [PEP 732 Discourse discussion](https://discuss.python.org/t/pep-732-the-python-documentation-editorial-board/36710)
* [Language Summit 2021 presentation](https://pyfound.blogspot.com/2021/05/the-2021-python-language-summit-python.html)
* [Language Summit 2020 presentation](https://pyfound.blogspot.com/2020/04/cpython-documentation-next-5-years.html)

These links give context on existing landing pages:

* [CPython Documentation Landing page (docs.python.org)](https://docs.python.org/3/)
* [PSF (python.org) website landing page](https://python.org)
* [Documentation Experience presentation](https://docs.google.com/presentation/d/1ujDv8wViPvAMFAtYCRxSKh-CMUlbjcfVYitsqEI2Ios/edit#slide=id.p) _[Work in Progress: Review of PSF landing page for docs]_
