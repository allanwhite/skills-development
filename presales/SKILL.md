---
name: sanity-presales
version: 0.2
date: 2026-03-30
description: >
  Sanity presales toolkit for Solution Engineers. Use this skill for prospect
  research and context synthesis, discovery guidance, demo planning, and
  stakeholder enrichment. Triggers on: "demo prep," "discovery call," "S2,"
  "S3," "demo plan," "what should I show," "presales," "prospect meeting,"
  "deal prep," "technical demo," "prospect context," "prospect research,"
  or any request to prepare for or plan a customer-facing presales meeting.
  Also triggers when someone pastes discovery notes and asks what to demo,
  provides raw materials to synthesize into a prospect profile, or when
  preparing for a specific account.
---

# Sanity Presales Demo Planning

Help Solution Engineers (SEs) prepare for and run discovery and demo meetings with enterprise prospects.

Three modes:
1. **Discovery guide** — walk through a live discovery conversation, surface the right questions, and capture structured findings.
2. **Demo plan generator** — take discovery notes as input and produce a concrete plan: what to show, what to explain, and what to build.
3. **Prospect context synthesis** — take raw materials (call transcripts, briefers, stakeholder lists, public content) and produce a structured prospect profile.

---

## Mode routing

**Discovery mode.** The SE says something like "I have a discovery call with [company]" or "help me run discovery." Walk them through the discovery framework below, asking one question cluster at a time. Capture findings in the prospect context template at the end.

**Demo plan mode.** The SE pastes discovery notes or describes what they learned. Load `references/demo-plan.md` and produce a demo plan following that template. Also load `references/triggers.md` to map enterprise triggers to features.

**Prospect context mode.** The SE provides raw materials — Gong briefers, call transcripts, stakeholder lists, podcast transcripts, or other source files. Load `references/prospect-context-template.md` and synthesize all inputs into a structured prospect profile. Ask clarifying questions before starting. Mark unknowns as explicit discovery gaps. Run the enrichment checklist (below) to fill gaps from public sources.

In all modes, connect findings to Sanity's messaging pillars (Model your business / Automate everything / Power anything) where natural, but don't force every point through the framework. The goal is a practical plan, not a messaging exercise.

**When you need more context:**

| Need | Load |
|------|------|
| Prospect context template | `references/prospect-context-template.md` |
| Demo plan template and narrative arc | `references/demo-plan.md` |
| Enterprise trigger → feature mapping | `references/triggers.md` |
| Atlas account data (future) | `references/atlas.md` |
| Full competitive positioning | `/mnt/skills/user/sanity-messaging/references/competitive-positioning.md` |
| Persona-specific framing | `/mnt/skills/user/sanity-messaging/references/personas.md` |
| Full messaging framework | `/mnt/skills/user/sanity-messaging/SKILL.md` |

---

## Use Case Tiers

Use these to gauge engagement depth. Tier determines how much SE time and customization to invest.

| Tier | Use cases | SE engagement |
|------|-----------|---------------|
| **High** | E-commerce, editorial product, marketing website (content ops), LMS, line-of-business app, whitelabel platform, PIM | Full demo customization, POC support, custom Studio build |
| **Standard** | Marketing website (basic), mobile app, live event content, digital signage, marketing comms, configuration app | Tailored demo with relevant examples, lighter POC |
| **Light** | Blog, support portal, documentation, corporate site, careers site, internal tools | Standard demo flow, minimal customization |

When a prospect has multiple use cases, tier by the highest-value one, but note the full picture for expansion potential.

---

## Discovery Framework

Use these question clusters during a discovery call. You don't need every question — pick what's relevant and skip what you already know.

### Current state
- What CMS or content system are you replacing or augmenting?
- Who creates and publishes content today? What's the developer-to-editor ratio?
- What's the tech stack? (Framework, hosting, current CMS, key integrations)

### Pain and motivation
- What's breaking or frustrating your team? (Common: editors blocked by devs, slow publishing, no structured content, can't reuse across channels)
- What channels does content need to reach? (Web, mobile, email, signage, APIs, agents)
- What's driving the timeline? (Migration deadline, product launch, contract renewal, replatforming)

### Enterprise context
- Is compliance a factor? (SSO/SAML, GDPR, data residency, security review)
- What enterprise capabilities matter? (Content Releases, Custom Roles, Live Content API, Media Library, App SDK)
- What's the expected scale? (API volume, asset count, number of editors, number of projects)

### Buying process
- Who is the economic buyer? Who is the technical champion?
- What's the decision timeline and process?
- Who else is being evaluated? (Contentful, Contentstack, Adobe, Sitecore, homegrown)

### Discovery output

After discovery, fill the prospect context template (`references/prospect-context-template.md`). The template captures all discovery findings in a structured format: company profile, deal metadata, pain points, use case fit, competitive context, stakeholders, Sanity angle, pillar alignment, and discovery gaps.

This replaces the need for a separate discovery output format — discovery findings and prospect context are the same document.

---

## Enrichment Checklist

After initial synthesis from provided materials, enrich the prospect context from public sources. Not every item applies to every deal — use judgment.

### Company research
- Company size, revenue, ownership structure, and funding history
- Brands, sub-brands, and product lines (especially if multi-brand is a use case)
- Site structure: main domains, microsites, subdomains
- Recent news: acquisitions, rebrand, leadership changes, product launches

### Stakeholder enrichment
- LinkedIn URLs for all known stakeholders
- Title verification — CRM data goes stale; confirm current titles via LinkedIn or company site
- Role hypothesis — if roles aren't provided, infer from title (e.g., SVP Product = technical evaluator/influencer)
- Add `last_verified` date when enriching

### Public content from key people
- CEO/exec podcast appearances, conference talks, blog posts, published books
- Cross-reference multiple sources for recurring themes (themes in 2+ sources are higher confidence)
- Extract quotes that intersect with content strategy, digital transformation, or AI adoption
- Summarize executive philosophy in a few sentences — this shapes demo framing

### Tech stack
- Current CMS confirmation via web research (BuiltWith, Wappalyzer, or manual inspection)
- Frontend framework, hosting, CDN
- Known integrations (forms, middleware, analytics, marketing automation)

---

## Competitive Quick Reference

For fast demo prep. For full competitive detail, load `/mnt/skills/user/sanity-messaging/references/competitive-positioning.md`.

**vs. Contentful:** Sanity offers fully customizable Studio (not just UI extensions), schema-as-code with version control, and AI workflows with structured context. Frame: "We go beyond publishing into content operations."

**vs. Contentstack:** Sanity provides code-first schema and workflows vs. UI-bound configuration. Frame: "Developer control without platform constraints."

**vs. Adobe AEM / Sitecore:** Sanity delivers DXP-level capability without the cost, complexity, or vendor lock-in. Frame: "Modern and agile, not heavy and expensive."

**vs. Homegrown:** Sanity gives you custom-build flexibility with a maintained platform underneath. Frame: "Stop maintaining infrastructure, start building features."

In all cases: lead with what Sanity does. Never call competitors broken. Use the pattern "They do X. We do Y."

---

## Messaging Pillar Reference

Light reference for connecting demo points to Sanity's value story. Don't force-fit; use where it naturally strengthens the narrative.

| Pillar | Core idea | Features that prove it |
|--------|-----------|----------------------|
| **Model your business** | Build a content system that matches how you operate | Content Lake, GROQ, Studio, App SDK, Visual Editing, Media Library |
| **Automate everything** | Let automation handle the repetitive work | Functions, Content Agent, Content Releases, Agent API |
| **Power anything** | Serve content to every channel from one source of truth | Libraries, Live CDN, MCP server, GROQ, Context for Agents |

For the full messaging framework, positioning hierarchy, and persona-specific proof points, load `/mnt/skills/user/sanity-messaging/SKILL.md`.