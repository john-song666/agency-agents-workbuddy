# Contributing

Thanks for your interest in improving this project!

## Acknowledgement

This repository is a **WorkBuddy-packaged version** of
[`msitarzewski/agency-agents`](https://github.com/msitarzewski/agency-agents)
by **Michael Sitarzewski**. All agent personas originate from that project —
thank you, Michael, for sharing and open-sourcing the work. 🙏

If you want to contribute *upstream* agent content (new roles, fixes to role
briefs), please open a PR against the original repo. This repo focuses on the
WorkBuddy packaging (skill format, routing, docs).

## What this repo is

`agency-agents-workbuddy` bundles the 239 agents from `msitarzewski/agency-agents`
into **17 domain skills** that WorkBuddy can load directly. Each domain skill:

- lives in `agency-<domain>/`
- has a `SKILL.md` that acts as a **router/index** (lists every agent in the
  domain and when to use each)
- has a `references/` folder with one `*.md` file per agent — the original
  persona brief, preserved verbatim

## Repository structure

```
agency-agents-workbuddy/
├── README.md                 # overview, domain table, install & usage
├── LICENSE                   # upstream license
├── CONTRIBUTING.md           # this file
└── agency-<domain>/          # 17 domains (academic … testing)
    ├── SKILL.md              # router/index for the domain
    ├── README.md             # per-domain usage + agent list
    └── references/
        └── <agent>.md        # one persona brief per file
```

## How skills load in WorkBuddy

1. Drop a domain folder into `~/.workbuddy/skills/` (e.g.
   `~/.workbuddy/skills/agency-engineering/`).
2. WorkBuddy picks the skill via its `description` / trigger keywords, or you
   invoke it explicitly by id: `agency-engineering`.
3. The skill tells WorkBuddy to *adopt* the requested persona; to follow a
   specific role closely, open the matching `references/<agent>.md` and follow
   that brief.

## Ways to contribute

### 1. Improve docs (no code)
- Fix typos, clarify the README, or improve a domain `README.md`.
- Open a PR with the change. Please keep the original-author credit block
  intact at the bottom of every README.

### 2. Add a new agent to an existing domain
1. Add the persona brief as `agency-<domain>/references/<agent-slug>.md`.
2. Add a one-line entry to `agency-<domain>/SKILL.md` (router list) and to
   `agency-<domain>/README.md` (agent list).
3. Open a PR.

### 3. Add a brand-new domain
1. Create `agency-<new-domain>/` with `SKILL.md`, `README.md`, and a
   `references/` folder.
2. Follow the structure of any existing domain (copy one as a template).
3. Add the new domain to the root `README.md` domain table.
4. Open a PR.

### 4. Sync with upstream
Upstream `msitarzewski/agency-agents` evolves. To refresh:
- Pull the latest `divisions/*.md` from upstream.
- Re-run the conversion/merge step (see `README.md` → "How it was built").
- Regenerate READMEs and re-upload. Keep the credit block.

## Style notes
- Persona briefs in `references/` are **verbatim from upstream** — don't
  rewrite them.
- Router/README prose is ours; keep it concise and in English (the credit
  block may stay bilingual).
- Keep `SKILL.md` frontmatter valid YAML (quote descriptions containing `:` or
  leading/trailing special chars).

## Questions?
Open an issue. For upstream agent content, go to the
[original repository](https://github.com/msitarzewski/agency-agents).
