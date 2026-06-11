---
title: "Projects"
url: "/projects"
summary: "Documentation projects the Editorial Board is leading or shepherding."
hideMeta: true
ShowToc: true
TocOpen: true
---

> **Status: Draft.** This page is a work in progress, started following the
> [June 2026 meeting](/updates/2026-06-09/).

This is the Editorial Board's list of significant documentation projects we are
actively leading or shepherding. It reflects our
[proactive stance](/expectations/#how-we-work-proactive-not-just-reactive):
rather than only reacting to requests, we identify important work and find
people to carry it out.

## How this list works

- **Every project has a committed lead.** This is not a wish list. A project is
  added only when someone has agreed to lead it. If a project loses its lead, it
  moves to [Parking lot](#parking-lot) until a new lead steps up.
- **Each project names its challenges**, not just the goal. Describing the
  hard parts up front helps contributors know what they are taking on.
- **We keep the list short and prioritized** rather than long and
  aspirational, so we can give each project real oversight.

Want to help with a project, or propose a new one? Open an
[issue on this repo](https://github.com/python/editorial-board/issues/new/choose)
or reach out in the [Python Docs Discord](https://discord.gg/nXkJ2JYvCu).

## Project template

Once a project is approved by the Editorial Board, copy this block to add a new project.

```markdown
### <Project name>

- **Lead:** <name — required; no lead, no listing>
- **Status:** Proposed | Active | Blocked | Done
- **Summary:** One or two sentences on what this project delivers.
- **Why it matters:** Who benefits and why this is worth doing now.
- **Challenges / risks:** The hard parts — technical blockers, dependencies,
  unknowns, things that could derail it.
- **How to help:** Concrete ways a contributor can get involved.
- **Links:** Relevant issues, PRs, discussions, or docs.
```

## Active projects

_None listed yet. Add projects here using the template above._

<!--
Example seeded from recent meetings — fill in a committed lead before promoting
to "Active":

### Split up the datetime documentation

- **Lead:** _TBD — needs a committed lead_
- **Status:** Proposed
- **Summary:** Break the large `datetime` reference page into more focused
  pages, and move the strftime/strptime format codes to their own page.
- **Why it matters:** `datetime.rst` is among the ten largest files in the docs;
  it mixes reference and tutorial-style content. More focused pages improve
  navigation, SEO, and discoverability (including by LLMs).
- **Challenges / risks:** Existing external links will break — depends on the
  redirect mechanism being worked on in the Docs WG (Petr). Some readers value
  a single page they can Ctrl-F (per feedback from Paul Ganssle). Needs
  coordination with in-flight PRs (#125009, #132524) and with Stan.
- **How to help:** Help define the page split, draft an overall tutorial,
  separate reference from tutorial content.
- **Links:**
  - https://docs.python.org/3/library/datetime.html
  - https://github.com/python/cpython/pull/125009
  - https://github.com/python/cpython/pull/132524
-->

## Parking lot

Ideas worth doing that do **not** yet have a committed lead. These are not
active projects until someone steps up to lead them.

_Empty for now._