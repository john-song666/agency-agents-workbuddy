# agency-agents-workbuddy

The [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) role library, **converted into WorkBuddy skill format** and **merged into 17 domain skills**.

Each `agency-<domain>/` folder is one WorkBuddy skill: `SKILL.md` is a router/index, and `references/*.md` holds each agent's original persona brief (loaded on demand).

## Features

- **239 expert personas** across 17 domains, ready to use as WorkBuddy skills
- **On-demand loading** — only the persona you need is read into context
- **Routing built-in** — describe a task and the skill points you to the right expert
- **Faithful conversion** — original role content preserved, credited to the author

## Domains (17)

| Domain | Skill id | Agents |
| --- | --- | --- |
| Academic | `agency-academic` | 6 |
| Design | `agency-design` | 9 |
| Engineering | `agency-engineering` | 49 |
| Finance | `agency-finance` | 5 |
| Game Development | `agency-game-development` | 5 |
| GIS | `agency-gis` | 13 |
| Healthcare | `agency-healthcare` | 3 |
| Marketing | `agency-marketing` | 36 |
| Paid Media | `agency-paid-media` | 7 |
| Product | `agency-product` | 5 |
| Project Management | `agency-project-management` | 7 |
| Sales | `agency-sales` | 9 |
| Security | `agency-security` | 10 |
| Spatial Computing | `agency-spatial-computing` | 6 |
| Specialized | `agency-specialized` | 54 |
| Support | `agency-support` | 6 |
| Testing | `agency-testing` | 9 |

## Install

Copy the `agency-*` folders into your WorkBuddy skills directory:

```text
# Windows
C:\Users\<you>\.workbuddy\skills

# macOS / Linux
~/.workbuddy/skills/
```

Or clone this repo and copy the 17 `agency-*` folders:

```bash
git clone https://github.com/john-song666/agency-agents-workbuddy.git
cp -r agency-agents-workbuddy/agency-* ~/.workbuddy/skills/
```

## Use

In WorkBuddy, say e.g. *"use a frontend expert"* or invoke the skill by id (`agency-engineering`); the router will point you to the right persona file. Open any `references/*.md` to adopt that role.

## Structure

```text
agency-agents-workbuddy/
├── README.md                  # this file
├── agency-academic/
│   ├── README.md           # domain overview (6 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 6 persona briefs (*.md)
├── agency-design/
│   ├── README.md           # domain overview (9 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 9 persona briefs (*.md)
├── agency-engineering/
│   ├── README.md           # domain overview (49 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 49 persona briefs (*.md)
├── agency-finance/
│   ├── README.md           # domain overview (5 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 5 persona briefs (*.md)
├── agency-game-development/
│   ├── README.md           # domain overview (5 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 5 persona briefs (*.md)
├── agency-gis/
│   ├── README.md           # domain overview (13 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 13 persona briefs (*.md)
├── agency-healthcare/
│   ├── README.md           # domain overview (3 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 3 persona briefs (*.md)
├── agency-marketing/
│   ├── README.md           # domain overview (36 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 36 persona briefs (*.md)
├── agency-paid-media/
│   ├── README.md           # domain overview (7 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 7 persona briefs (*.md)
├── agency-product/
│   ├── README.md           # domain overview (5 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 5 persona briefs (*.md)
├── agency-project-management/
│   ├── README.md           # domain overview (7 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 7 persona briefs (*.md)
├── agency-sales/
│   ├── README.md           # domain overview (9 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 9 persona briefs (*.md)
├── agency-security/
│   ├── README.md           # domain overview (10 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 10 persona briefs (*.md)
├── agency-spatial-computing/
│   ├── README.md           # domain overview (6 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 6 persona briefs (*.md)
├── agency-specialized/
│   ├── README.md           # domain overview (54 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 54 persona briefs (*.md)
├── agency-support/
│   ├── README.md           # domain overview (6 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 6 persona briefs (*.md)
├── agency-testing/
│   ├── README.md           # domain overview (9 agents)
│   ├── SKILL.md            # router / index
│   └── references/         # 9 persona briefs (*.md)
└── LICENSE
```

## Credit / 致谢

This skill-pack is a conversion of [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents) by **Michael Sitarzewski**.

> 感谢原作者 **Michael Sitarzewski** 的分享与开源。 🙏
> Converted & merged by domain into WorkBuddy skill format. All role content remains attributed to the original author.
