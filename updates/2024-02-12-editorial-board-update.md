# Meeting Notes: Python Docs Editorial Board

## February 12, 2024

## Attendees

Mariatta, Ned, Joanna, Guido


## Agenda

1. What project do we want to deliver first? Here are some ideas to start the discussion:

   a. Define scope and outline for new intro tutorial
   b. Define scope and outline for new landing page
   c. Inventory/audit a section of the docs
   d. Personas (see #3 below)


2. What does the docs community need from us most right now? Here are some ideas to start the discussion:

   - How-to discussion
   - First-person discussion 
   - A more thorough and more skimmable style guide

3. [meta] Do we have a way to collect the largish topics they’ve discussed that we could provide guidance for? -> see editorial-board GH repo

   - Function parameters: bulleted or not
   - Examples: how to integrate into the docs
   - Type hints 

4. Do we have an idea of what type of learner/user we need to optimize the docs for?

   - Wait until Carol is back 

5. Do we have an idea of what type of contributor we want to prioritize removing obstacles for and creating systems for?

6. Will the editorial board give an update at the language summit or PyCon?

7. The language summit isn’t even announced yet. We’ll think about it next time

## Notes

1. Let’s begin with a relatively small project. 1b from above. It is concrete, and we can propose implementation and refine it quickly.

2. 2a is a bigger issue, but is important. (will affect 2b)

3. Recommendation: don’t use first-person for new docs.

4. Howto doc: we might preserve some historical content. Some docs may be marked as “historical doc”, keep them, but might get changed. Add a disclaimer at the top.

5. Add reminder to future contributors not to use those as a template.

6. PR churn. Docs changes don’t need to follow the same guidelines.

7. Style guide:
   - In devguide now, update it
   - https://devguide.python.org/documentation/style-guide/
   - Some things should be in the style guide
   - First person, terminologies like master/slave, should be there
   - Big O notation should be in the Howto part of the style guide
   - The EB will own this (and create issues and PRs)
   - Should still be on devguide

8. Discovery: 🔒 [Docs Style Guide](https://docs.google.com/document/d/1rSkUIGFuI5zDMYturyJCo9agYPQ-d53Z3MntSV0rB3E/edit#heading=h.hflx14peuyef)

9. Mariatta to create a Gdrive folder to be shared with PDEB
   
10. Need an “ad-campaign” about https://github.com/python/editorial-board, this exists, the readme tells how to be involved and ask for help.
   On Discourse
   - In the readme of docs-community GitHub repo
   - DevGuide
   - And PEP 732 

11. Docs Discord server: we shouldn’t need to be the owner.
   
12. Discuss: what type of learner we need to optimize the docs for?
    - We wait until Carol is back
    - We’ll start an async collaboration in a GDoc in a new 
    - There is a way to get notification of changes in GDoc. Need to be set up per-doc
    - Click the “comment” button on GDoc
    - Click the bell to set notifications: you can get notified of all content changes

13. Do we have an idea of what type of contributor we want to prioritize removing obstacles for and creating systems for?
    - What are the types of contributors?
    - Core devs, triagers -> already know the way
    - For non core devs: First time OS contributor, vs experienced OS contributor
    - Non developers
    - Not-primarily english-speaking contributors

14. Guido’s request: Not having links that are hidden unless you hover

15. A tutorial on how to successfully contribute to the CPython docs.

16. CPython docs links to GitHub source code if clicked on the “Show Source” link. Is this good?
    - Some pages get rendered (pprint.rst), some show as raw rst (functions.rst)

17. What type of contributors who can make the biggest impact, that we are currently overlooking?
    - Tech writers
    - Challenge: who to listen to. PR reviews can be noisy. 
    - Member vs Contributor 
    - But what if even core devs conflict with each other. 

18. Can we have volunteers/helpers to help people with pull requests?
    - Could be similar to the Djangonauts: have someone who will help new contributors with PRs. Captains, navigators, etc
    - Or less structured.
    - Avoiding using the word “mentor” because it seems to be establishing a formal relationship


## Action items

* Style Guide:
  Update the style guide with some new recommendations: first-person, terminologies
* Ad campaign:

More detail on #10 of the above notes:
* Start the async exploration of who our learners are 
* Start the async explorations of what kind of contributors we want to help
* Specify that Python wiki is out of scope in PEP 732: https://github.com/python/peps/pull/3663	

