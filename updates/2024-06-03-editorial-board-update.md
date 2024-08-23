# Meeting Notes: Python Docs Editorial Board

## June 3, 2024

## Attendees

Mariatta, Ned, Carol, Joanna, Guido


## Old Action Items

Where are we with the action items from April 8?

1. Bring up in the next community call: Are there clear possibilities that you can share with the editorial board, so we can make a decision?
    - Ned has been attending, but can’t tomorrow. They have not been coming up with things they want us to do.
    - Give them immediate feedback: we will decide if you create an issue.
    - Sometimes the problem isn't framed appropriately
    - Carol will attend tomorrow. 
    - Todo: be clear to the docs wg that we will decide if you open up a ticket

2. Eric Matthes said: wants to see us have more guiding principles before getting involved,

3. Todo: create a dir in the GitHub repo and move there?
   - Google Drive? 
   - Todo: move or link the docs to the GitHub repo
   
4. NEW Action item: communicate the above to the next Docs Community meeting.

Where are we with the action items from March 11?
1. Look at front page of docs.p.o and decide which ones should be more prominent
2. Come up with a short: (3 page) tutorial. Carol will start an outline. 
3. Document our philosophy, explain the different target users and where they can find the docs they need.


## Agenda

1. What action items are we taking from the discussion at the docs dinner?
   * Notes on contributing to docs:
     - Melanie’s notes: [Python Docs Contributing Adventure](https://docs.google.com/document/d/11zxisx5XfYOsrDOn4qd-XUSpDltIOi35qiOO9fDLfnI/edit#heading=h.1hkck4lqac8)
     - Shauna’s notes: [Python Docs Onboarding Notes](https://docs.google.com/document/d/1icjPpmEUH0BRPDwl7oXLkpasvwZoS5io2LyTEhblku0/edit)
     - Notes after discussion with Eric Matthes: [Guiding Principles for Documentation Editorial Board.md](https://drive.google.com/file/d/1elKNdRPTIoNe6EZ4TbS9aquM-RaNDgmc/view?usp=drive_link)
     - Sprint ideas from Carol's discussion: [Doc ideas.md](https://drive.google.com/file/d/17uGzCmFnUDBYGwsR9xmzEOGi4fOOSnOj/view?usp=drive_link)

   * Other notes from dinner: 
     - Should you learn Python
     - Cheatsheet for rST markup
     - Ned says: "Write how-tos for Trey"
     - Trey = priorities
     - Docs are shared resource
     - Add "Did you find this helpful"
     - Update "How to contribute to docs" in dev guide and perhaps in a more user friendly way
     - What to expect after a docs PR
     - Codespell run once by core devs then add to CI after
     - Message on PR template for docs that sets expectations for PR review
   
   * Action item: no clear path for contributing to CPython Docs. Devguide section is lacking, mostly for CPython code changes. 
   * New action item: the PDEB should write tickets for the action items on this meeting
   * Decision:
     - We are sticking with Rst for CPython docs.
     - Myst Parser: https://myst-parser.readthedocs.io/en/latest/
     - Mariatta has a talk: [Introduction to Sphinx Docs and reStructuredText](https://www.youtube.com/watch?v=v4eoYpCON_c) - Pyninsula #28
   * Action item:
     - Ned will write up an outline for “How to contribute to CPython Docs”

2. What action items are we taking from the docs summit?
   none

3. Do we have action items from the Docs Community?
   

4. Is it time for us to focus on filling out these two docs so we can set a direction? Is there something else we should do first because it is either a higher priority or a prerequisite? Are there people in the Python community who have more formal experience with user research and might want to help?
   * Discovery doc about learners (Carol, would you like to capture your thoughts in this doc since you seem to have considered the issue deeply?) The Guiding Principles for Documentation Editorial Board.md captures the 3 user personas.
   * Discovery doc about contributors (Ned, would you like to capture your observations about the community in this doc since you seem to be the most involved with them?)
   * Action item: finish up the 🔒 [Guiding Principles](https://docs.google.com/document/d/1ILusuBaAoxUzm1NDOuiS3sZYePDVB5YcY7RoLkXyfI0/edit?usp=sharing) doc, and officially adopt it. To become the first page of the Docs Guide. To answer the “Discover Doc about Learners” Discovery Doc: Who is Our Learner

5. Todo: form a WG to address packaging users docs

6. Discussing the [Guiding Principles](https://drive.google.com/file/d/1elKNdRPTIoNe6EZ4TbS9aquM-RaNDgmc/view?usp=sharing)
   * How to ensure the novices are properly supported? 
   * Action item: Develop a user-journey. Tutorials, to be added outside of the actual Tutorials section. Eg including examples in references.
   * Who are our contributors?
     - Core devs. Code changes -> doc changes
     - Long-term docs contributors
     - Drive-by contributors
     - Translations
   * People writing dev docs professionally don’t wanna contribute to Open source docs?
   * Educators may have feedback too
   * As PDEb we can create a system to unblock contributors. Which type of contributors we want to focus on? #2: long-term docs contributors.
   * Action item: the doc outline. Share tools/cheatsheet of learning Sphinx/rst, etc
     - Note:  the logistics of splitting up docs sections will be a big project
   * Action item:
     - Pull out docs-related from devguide as a (git) subtree
   * There are a lot of undocumented Docs tooling. Should write it up?

7. Next meeting: vacations, EuroPython.
   * Cancel July, and meet August 12.
