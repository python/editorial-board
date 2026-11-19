---
title: "{{ replace .File.ContentBaseName "-" " " | title }}"
# The date the project was added to the list. Used to order the RSS feed.
date: "{{ .Date }}"
# proposed | active | blocked | done
status: "proposed"
# Editorial Board member sponsoring the project. Leave empty if none yet.
sponsor: ""
# Set to false if the project does not need an Editorial Board sponsor.
needs_sponsor: true
# Person actively leading the work. Leave empty if none yet.
# An active project must have a lead.
lead: ""
# One or two sentences on what this project delivers.
summary: ""
# Link to the project issue: the issue that fully describes the project.
project_issue: ""
# Rough priority within its status group: lower numbers are listed first.
weight: 100
# Other relevant issues, PRs, discussions, or docs. GitHub issue and PR links
# get a live status badge, and their title is filled in from GitHub if left empty.
links: []
#  - title: ""
#    url: ""
---

## Description

What the work is, broken down into tasks if possible.

## Benefits

Who benefits and why this is worth doing now.

## Decisions

Smaller decisions that are still open. Major decisions should be made before the
project is listed.

## Challenges and risks

The hard parts and possible pitfalls.

## How to help

Concrete ways a contributor can get involved.
