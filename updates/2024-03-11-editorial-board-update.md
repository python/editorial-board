# Meeting Notes: Python Docs Editorial Board

## March 11, 2024

## Attendees

Mariatta, Ned, Joanna, Guido


## Agenda

1. What project do we want to deliver first? Here are some ideas to start the discussion:

a. Define scope and outline for new intro tutorial
b. Define scope and outline for new landing page
c. Inventory/audit a section of the docs
d. Define learner personas


2. What does the docs community need from us most right now? Here are some ideas to start the discussion:

- How-to discussion
- First-person discussion 
- A more thorough and more skimmable style guide

3. [meta] Do we have a way to collect the largish topics they’ve discussed that we could provide guidance for? -> see editorial-board GH repo

- Function parameters: bulleted or not
- Examples: how to integrate into the docs
- Type hints 

4. Do we have an idea of what type of learner/user we need to optimize the docs for?
   - 🔒 [Discovery doc about learners](https://docs.google.com/document/d/1ILusuBaAoxUzm1NDOuiS3sZYePDVB5YcY7RoLkXyfI0/edit?usp=sharing)
   - [Thoughts about growth in users and approach](https://discord.com/channels/1100135599077331024/1100135599077331028/1216838941723070534)

5. Do we have an idea of what type of contributor we want to prioritize removing obstacles for and creating systems for?

6. How do we decide on issues for our agenda?
   Is e.g. https://github.com/python/cpython/pull/116595 suitable to discuss here?



## Notes

Guido: We didn't actually go through that agenda at all.
We discuss what our priorities are.
We also didn't review last month's action items.


1. Python growth for the next decade will be driven by non CS folks, new users, non technical. 
2. Existing tutorial is the "what" 
3. Python has a rich ecosystem, you can get a lot of things done without needing the full scope of the stdlib. We should have more docs for it.
   Example docs:
   - https://github.com/sandiegopython/intro-to-python/ 
   - Jessica McKellar’s intro: https://www.youtube.com/watch?v=rkx5_MRAV3A 
4. We need an introduction to Python docs. Current official Tutorial isn’t targeting new non-technical learners. They don’t know where to start. Other resources exist elsewhere. But it would be useful to have a beginner’s guide within docs.p.o
   - Do we need to cover everything? Lots of people write guides to Python
   - Official docs could have a curated list of useful docs. 

5. Options:
   - Better landing page?
     * It needs to be better for newcomers, but also for people who are already experienced and already know their way around the docs.
     * Come up with a refresh of the docs.python.org landing page, more user friendly and welcoming/inviting.
     * Tooltips/ Guided tours -> need cookies.
       Just provide a link instead of interactive.
   - Action item:
     * Look at front page of docs.p.o and decide which ones should be more prominent
     * Come up with a short: (3 page) tutorial. Carol will start an outline. 
     * Document our philosophy, explain the different target users and where they can find the docs they need.
   - Glossary
   - Define other user personas first?
6. Docs community meeting. Anything we should know?
   - What to do with Changelog.
   - Directives changes in the rst. Need to improve the devguide for it.
   - Typographic markups. Still under discussion on Discourse. 
   - Think about the outcome first and toolings next.
   - Accessibility checking. UI/UX. Italics or not.
7. Ned is talking to a university professor who is building their own IDE/notebook. 
   - They see this as a hurdle for teaching Python to students
