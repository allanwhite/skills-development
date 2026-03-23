---
name: presales-demo-planning
version: 0.1
date: 2026-03-22
description: >
  Plan and prepare Sanity presales demos for Solution Engineers. Use this skill
  whenever an SE needs to run discovery, prepare a tailored demo, or plan what
  to show, explain, and build for a prospect. Triggers on: "demo prep," "discovery
  call," "S2," "S3," "demo plan," "what should I show," "presales," "prospect
  meeting," "deal prep," "technical demo," or any request to prepare for or
  plan a customer-facing presales meeting. Also triggers when someone pastes
  discovery notes and asks what to demo, or when preparing for a specific account.
---

# Sanity Presales Demo Planning

Help Solution Engineers (SEs) prepare for and run discovery and demo meetings
with enterprise prospects. Two modes:

1. **Discovery guide** — walk through a live discovery conversation, surface
   the right questions, and capture structured findings.
2. **Demo plan generator** — take discovery notes as input and produce a
   concrete plan: what to show, what to explain, and what to build.

---

## Mode routing

**Discovery mode.** The SE says something like "I have a discovery call with
[company]" or "help me run discovery." Walk them through the discovery
framework below, asking one question cluster at a time. Capture findings in
the structured discovery output format at the end.

**Demo plan mode.** The SE pastes discovery notes or describes what they learned.
Load `references/demo-plan.md` and produce a demo plan following that template.
Also load `references/triggers.md` to map enterprise triggers to features.

In both modes, connect findings to Sanity's messaging pillars (Model your
business / Automate everything / Power anything) where natural, but don't
force every point through the framework. The goal is a practical plan, not a
messaging exercise.

**When you need more context:**

| Need | Load |
|------|------|
| Demo plan template and narrative arc | `references/demo-plan.md` |
| Enterprise trigger → feature mapping | `references/triggers.md` |
| Atlas account data (future) | `references/atlas.md` |
| Full competitive positioning | `/mnt/skills/user/sanity-messaging/references/competitive-positioning.md` |
| Persona-specific framing | `/mnt/skills/user/sanity-messaging/references/personas.md` |
| Full messaging framework | `/mnt/skills/user/sanity-messaging/SKILL.md` |

---

## Use Case Tiers

Use these to gauge engagement depth. Tier determines how much SE time and
customization to invest.

| Tier | Use cases | SE engagement |
|------|-----------|---------------|
| **High** | E-commerce, editorial product, marketing website (content ops), LMS, line-of-business app, whitelabel platform, PIM | Full demo customization, POC support, custom Studio build |
| **Standard** | Marketing website (basic), mobile app, live event content, digital signage, marketing comms, configuration app | Tailored demo with relevant examples, lighter POC |
| **Light** | Blog, support portal, documentation, corporate site, careers site, internal tools | Standard demo flow, minimal customization |

When a prospect has multiple use cases, tier by the highest-value one, but
note the full picture for expansion potential.

---

## Discovery Framework

Use these question clusters during a discovery call. You don't need every
question — pick what's relevant and skip what you already know.

### Current state
- What CMS or content system are you replacing or augmenting?
- Who creates and publishes content today? What's the developer-to-editor ratio?
- What's the tech stack? (Framework, hosting, current CMS, key integrations)

### Pain and motivation
- What's breaking or frustrating your team? (Common: editors blocked by devs,
  slow publishing, no structured content, can't reuse across channels)
- What channels does content need to reach? (Web, mobile, email, signage, APIs, agents)
- What's driving the timeline? (Migration deadline, product launch, contract renewal, replatforming)

### Enterprise context
- Is compliance a factor? (SSO/SAML, GDPR, data residency, security review)
- What enterprise capabilities matter? (Content Releases, Custom Roles,
  Live Content API, Media Library, App SDK)
- What's the expected scale? (API volume, asset count, number of editors, number of projects)

### Buying process
- Who is the economic buyer? Who is the technical champion?
- What's the decision timeline and process?
- Who else is being evaluated? (Contentful, Contentstack, Adobe, Sitecore, homegrown)

### Discovery output

After discovery, capture these fields. This becomes the input for demo planning.

```
Account:
Primary use case:
Use case tier: [High / Standard / Light]
Current CMS:
Tech stack: [framework, hosting, key integrations]
Pain points: [list the top 2-3]
Channels: [where content needs to go]
Enterprise triggers: [compliance / features / SLA / quota / other]
Competitors in eval:
Champion: [name, role]
Economic buyer: [name, role]
Timeline:
Key messaging pillar fit: [Model / Automate / Power — which resonates most]
```

---

## Competitive Quick Reference

For fast demo prep. For full competitive detail, load
`/mnt/skills/user/sanity-messaging/references/competitive-positioning.md`.

**vs. Contentful:** Sanity offers fully customizable Studio (not just UI
extensions), schema-as-code with version control, and AI workflows with
structured context. Frame: "We go beyond publishing into content operations."

**vs. Contentstack:** Sanity provides code-first schema and workflows vs.
UI-bound configuration. Frame: "Developer control without platform constraints."

**vs. Adobe AEM / Sitecore:** Sanity delivers DXP-level capability without the
cost, complexity, or vendor lock-in. Frame: "Modern and agile, not heavy
and expensive."

**vs. Homegrown:** Sanity gives you custom-build flexibility with a maintained
platform underneath. Frame: "Stop maintaining infrastructure, start building
features."

In all cases: lead with what Sanity does. Never call competitors broken.
Use the pattern "They do X. We do Y."

---

## Messaging Pillar Reference

Light reference for connecting demo points to Sanity's value story. Don't
force-fit; use where it naturally strengthens the narrative.

| Pillar | Core idea | Features that prove it |
|--------|-----------|----------------------|
| **Model your business** | Build a content system that matches how you operate | Content Lake, GROQ, Studio, App SDK, Visual Editing, Media Library |
| **Automate everything** | Let automation handle the repetitive work | Functions, Content Agent, Content Releases, Agent API |
| **Power anything** | Serve content to every channel from one source of truth | Libraries, Live CDN, MCP server, GROQ, Context for Agents |

For the full messaging framework, positioning hierarchy, and persona-specific
proof points, load `/mnt/skills/user/sanity-messaging/SKILL.md`.
