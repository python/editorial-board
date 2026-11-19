---
title: "Adding a project"
url: "/projects/how-to-add/"
summary: "How to propose a documentation project and add it to the Editorial Board's project list."
hideMeta: true
ShowToc: true
TocOpen: false
ShowPostNavLinks: false
---

This page explains how a project gets onto the [project list]({{< relref "projects" >}}),
and how to write its page. For the kind of support a project can expect,
see [What to expect from a sponsor]({{< relref "projects#what-to-expect" >}}).

## From idea to project page

1. **Open an issue.** Use the
   [Suggest a project](https://github.com/python/editorial-board/issues/new?template=project.md)
   template. Describe the work, its benefits, the decisions needed, and the challenges and risks.
   The issue is where the proposal is discussed.
2. **Open a pull request with the project page.** Alongside the issue, open a pull request that
   adds one Markdown file for the project under
   [`content/projects/`](https://github.com/python/editorial-board/tree/main/content/projects),
   filled in as described below. Set `project_issue` to the issue from step 1, and mention the
   issue in the pull request description. You don't need Hugo installed: a preview of the site
   is built for every pull request, so you can see how the page will look.
3. **Get it approved.** The Editorial Board reviews the issue and the project page together,
   usually at a monthly meeting. The board may ask for changes to the page, for example to
   the scope, the challenges, or the status. Merging the pull request adds the project to the list.

## Creating the file

Copy the template in
[`archetypes/projects.md`](https://github.com/python/editorial-board/blob/main/archetypes/projects.md),
or, if you have Hugo installed, run:

```
hugo new content content/projects/short-project-name.md
```

The file name becomes the project page's URL, so keep it short and descriptive.

## Frontmatter

| Field | Required | Description |
|-------|----------|-------------|
| `title` | yes | The project's name. |
| `date` | yes | The date the project was added to the list, for example `2026-11-10`. Used to order the projects RSS feed. |
| `status` | yes | One of `proposed`, `active`, `blocked`, or `done`. Any other value fails the build. See [Statuses](#statuses). |
| `lead` | for `active` | The person actively leading the work. Leave empty if there is no lead yet; the page shows "Needs a committed lead". |
| `sponsor` | no | The Editorial Board member sponsoring the project. Leave empty if none yet. |
| `summary` | yes | One or two sentences on what the project delivers. Shown in the project list. |
| `project_issue` | no | Link to the project issue: the issue that fully describes the project, usually the one opened with the "Suggest a project" template. |
| `weight` | no | Rough priority. The list shows active projects first, then proposed, blocked, and done; within each status, lower numbers are listed first. |
| `links` | no | Related issues, PRs, discussions, or docs, as a list of `url` entries with an optional `title`. See [Links](#links). |

See the [example](#example) below for a complete project file.

## Page body

Below the frontmatter, describe the project with these sections, matching the issue template:

- **Description**: what the work is, broken down into tasks if possible.
- **Benefits**: who benefits and why it is worth doing now.
- **Decisions**: smaller decisions that are still open. Major decisions should be made
  before a project is listed, so the work is ready to start.
- **Challenges and risks**: the hard parts. Every project should name these.
- **How to help**: concrete ways a contributor can get involved.

## Example

A complete project file, `content/projects/off-by-one-pizza.md`:

```markdown
---
title: "End the off-by-one pizza incidents"
date: "2026-04-01"
status: "active"
sponsor: ""
lead: "Spam Eggington"
summary: "Explain range() so clearly that nobody orders 9 pizzas for a party of 10 ever again."
project_issue: "https://github.com/example/office-party/issues/42"
weight: 10
links:
  - title: "range(10) stopping at 9 is not intuitive"
    url: "https://github.com/example/office-party/issues/43"
  - url: "https://github.com/example/office-party/pull/44"
  - title: "Pizza slicing reference"
    url: "https://docs.example.com/pizza/slicing.html"
---

## Description

Every office party, someone writes `for slice in range(1, 10)` and one guest goes hungry.
This project rewrites the guide to counting things so the end of a range is never a surprise.

1. Explain why `range(10)` gives ten numbers but never the number 10.
2. Add a worked example: splitting 8 slices between 3 people with `divmod()`,
   and what to do with the leftover slices.
3. Add a "counting from zero" sidebar for readers who still count on their fingers.

## Benefits

- Fewer hungry guests, and fewer bug reports titled "range is broken".
- Readers new to Python learn half-open ranges once, instead of once per party.

## Decisions

- Should the examples use pizza, or something less controversial, like cake?
- Does the leftover-slices example belong in this guide or in the `divmod()` reference?

## Challenges and risks

- Pineapple: any pizza example will start an argument that has nothing to do with Python.
- Readers who are used to inclusive ranges in other languages may need more than one example.
- The lead is easily distracted by actual pizza.

## How to help

- Review the draft and tell us where you first got confused.
- Suggest a better example than pizza, if one exists.
- Bring snacks to the review meeting.
```

## Links

The entries in `links` are shown after the page body, in two tables:

- **Issues and pull requests**: any GitHub issue or pull request URL. Each one is shown as
  `owner/repo#number` with a status badge: Open, Draft, Merged, Closed, or Not planned.
  The status is fetched from GitHub in the reader's browser, so it stays current without
  rebuilding the site. If `title` is left out, the title from GitHub is shown instead.
  Don't put the status in the title, since the badge already shows it.
- **Links**: everything else, such as pages in the docs, shown with the site they're on.
  Give these a `title`, otherwise the URL itself is shown.

The `project_issue` link is shown at the top of the page, with the same status badge.

If GitHub can't be reached, for example because of its limit on anonymous requests,
the links still work but are shown without a status badge.

## Statuses

- **Proposed**: approved as worth doing, but not yet started, or still missing a lead.
- **Active**: work is underway with a committed lead.
- **Blocked**: work can't continue, for example because the project lost its lead.
- **Done**: finished. Keep the page so the list shows what was accomplished.

The project list can be searched and filtered by status. Filters are kept in the URL, so a
filtered view can be shared, for example
[`/projects/?status=active`]({{< relref "projects" >}}?status=active).
