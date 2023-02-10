---
title: Meta
description: Information about how to write documentation here.
github: https://github.com/cweagans/docs-meta
layout: projecthome
---

{{< lead text="This documentation site aggregates documentation from all of my public projects" >}}

Stuff I want to write about here:

* Environments
  * Live is at docs.cweagans.net and has the latest _tag_ for each project deployed.
  * Staging is at docs-staging.cweagans.net and has the tip of `main` for each project deployed.
  * Deployment schedules/mechanisms (probably done through my on-prem Drone CI and deployed to Dreamhost)
* Writing
  * Formatting (kitchen sink example?)
  * Style guide
    * Friendly, approachable
    * Don't use warning unless it's something actually dangerous somehow
  * Shortcodes
    * Lead
    * Quicklinks
    * Callout
    * Warning
* Features
  * Automatic section/menu structure
  * Table of contents when heading waterfall is correct
  * Github link to project
  * Feedback link for each page
* Assumptions made about aggregated project docs
  * Docs live in `docs/` in the root of the repo
  * There is a issue template for docs feedback (add specifics from Composer Patches repo) that has a key for pointing at the specific file.
  * Content is set up in sections like hugo wants
* Roadmap
  * Redirects from .htaccess via a per-project configuration file (redirects.yaml or something along those lines, which generates .htaccess entries)
  * PR environments??
  * Doc search per-section
  * Scroll spy for table of contents
  * Manual menu setup?
  * Redirect section pages to their first page (we don't use the section pages for anything other than the menu headings)
  * Get rid of the Hugo-generated RSS feeds
  * Re-enable sitemap
  * Use prism styles from upstream template for code highlighting (or pick a different syntax theme that looks better)
  * Import project update feed for each project home page?
  * Maybe versioned documentation
  * Maybe a project picker in the header
