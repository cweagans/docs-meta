---
title: Assumptions
---

Because this site automates a number of things related to documentation, there are some assumptions that are made about the projects that it interacts with. 

* Projects must be available via Git.
* The `main` branch of each project should be the most up-to-date version of the project.
* If the project is in a GitHub repository (preferred), there should be an issue template called `docs.yml` for leaving documentation feedback. This template should include a field with an `id` of `file` so that the path to the source file can be pre-populated.
* Content is organized into sections and optionally ordered by `weight` values in the front matter of each section/page.
