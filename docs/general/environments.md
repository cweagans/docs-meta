---
title: Environments
weight: 30
---

There are two separate environments for this documentation site. Production can be found at https://docs.cweagans.net. Staging can be found at https://docs-staging.cweagans.net.

Each environment is deployed on a different cadence. Production is deployed once per week (every Monday at 9am Mountain Time) and staging is deployed whenever there is a change to the `main` branch of one of the upstream docs repositories.
If you need the deployment frequency of either environment turned up temporarily, please let me know. There's currently not enough activity to justify more frequent deployments, but I'm happy to help if you're working on documentation.

While the documented projects are typically on a tagged release model, all documentation on this site is on a rolling release: anything that's in the `main` branch of the project repository will get deployed to this site. That can be changed temporarily to accommodate specific work in any project repository: open an issue and let me know what you need.

Functionally, there is no difference between the two environments. They are hosted on the same server with the same configuration. Eventually, I may add some stuff to staging to discourage search engines from indexing the pages, but that's not a huge priority right now.
