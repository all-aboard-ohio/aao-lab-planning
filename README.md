# AAO Data Lab — Project Planning

This repository is the org-level project tracker for the [All Aboard Ohio Data Lab](https://lab.allaboardohio.org).

Use it to **propose new tools, analyses, and research projects**. Once a project is approved and a contributor is ready to build, it gets its own repository bootstrapped from a template.

---

## The Two-Tier System

AAO Data Lab uses a two-tier issue structure tracked on one [org-level GitHub Projects board](https://github.com/orgs/all-aboard-ohio/projects):

| Tier | Where | What lives here |
|---|---|---|
| **Proposals** | This repo (`aao-lab-planning`) | New tool and analysis ideas |
| **Implementation tasks** | Individual project repos | Features, bugs, data work for active projects |

Both tiers feed the same board so the whole org's work is visible in one place.

---

## GitHub Projects Board

> **[View the board →](https://github.com/orgs/all-aboard-ohio/projects)**

The board is the canonical view of everything in-flight. It auto-pulls all issues from this repo and issues labeled `task` from individual project repos.

### Status workflow

| Status | Meaning |
|---|---|
| **Proposed** | Issue opened here, awaiting maintainer review |
| **Scoping** | Maintainer reviewing — clarifying scope, disciplines needed |
| **Approved** | Scope accepted; waiting for a contributor to pick it up |
| **In Progress** | Repo created or issue claimed; active work underway |
| **Review** | PR open, awaiting review |
| **Shipped** | Tool deployed or analysis published; homepage updated |

---

## Proposing a New Project

1. Check open issues and the board to avoid duplicates
2. Mention your idea in [`#projects`](https://join.slack.com/t/lab-allaboardohio/shared_invite/zt-3x7cyvl53-0IQMjvljmA64iNCZvhaP1w) on Slack first
3. Open an issue using the appropriate template:
   - **New Tool or App** — deployable web tools (maps, calculators, dashboards, PWAs)
   - **New Analysis or Research** — data models, notebooks, cleaned datasets, reports
4. The issue auto-appears on the board as **Proposed**
5. A maintainer will move it to **Scoping** and collaborate with you to sharpen the scope

---

## Starting a New Repository

Once a project reaches **Approved**:

1. Create a new repo from the right template:
   - [aao-lab-template-tool](https://github.com/all-aboard-ohio/aao-lab-template-tool) — React + Vite + Tailwind, AAO components pre-wired, GitHub Pages deploy included
   - [aao-lab-template-analysis](https://github.com/all-aboard-ohio/aao-lab-template-analysis) — Python + Jupyter, standard folder structure
2. Comment the new repo URL on the planning issue and link back from the repo README
3. Open implementation task issues in the new repo labeled `task` — they’ll auto-populate the board

---

## Shipping

When a tool is deployed or analysis is published:

1. Close all implementation issues in the project repo
2. Comment the live URL on the planning issue here, then close it
3. Move the board item to **Shipped**
4. If it’s a deployed web tool: update [`aao-lab-homepage/src/data/projects.js`](https://github.com/all-aboard-ohio/aao-lab-homepage/blob/main/src/data/projects.js) to show it as Live

---

## Labels

| Label | Description |
|---|---|
| `new-tool` | Web tool or app proposal |
| `research` | Data model, notebook, or analysis proposal |
| `in-scoping` | Under maintainer review |
| `approved` | Scoped and ready for a contributor |
| `good first issue` | Well-scoped, suitable for a new contributor |
| `needs-discipline` | Blocked on finding a specific skill |

---

## Resources

| Resource | Link |
|---|---|
| Project board | [GitHub Projects](https://github.com/orgs/all-aboard-ohio/projects) |
| Contributor docs | [aao-lab-docs](https://github.com/all-aboard-ohio/aao-lab-docs) |
| Project management guide | [project-management.md](https://github.com/all-aboard-ohio/aao-lab-docs/blob/main/project-management.md) |
| Architecture & deployment | [architecture.md](https://github.com/all-aboard-ohio/aao-lab-docs/blob/main/architecture.md) |
| Live site | [lab.allaboardohio.org](https://lab.allaboardohio.org) |
| Slack | [#projects](https://join.slack.com/t/lab-allaboardohio/shared_invite/zt-3x7cyvl53-0IQMjvljmA64iNCZvhaP1w) |

---

Part of [All Aboard Ohio](https://allaboardohio.org) · [lab.allaboardohio.org](https://lab.allaboardohio.org)
