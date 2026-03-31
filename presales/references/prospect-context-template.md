---
version: ""           # e.g. "1.0"
author: ""            # e.g. "@presailor"
date: ""              # e.g. "2026-03-30T21:20:00+00:00 UTC"
generator: "miriad"
skills: []            # e.g. ["sanity-presales (NR2IXlzl)", "sanity-messaging (F911ULfT)"]
sources: []           # see example below
# sources:
#   - file: ""
#     purpose: ""
---

# Prospect Context

## Company

```yaml
company: ""
industry: ""           # e.g. Hospitality, Retail, Fintech, Healthcare
sub_vertical: ""       # e.g. Luxury Hotels, Sports Retail, B2B SaaS
size:
  employees: ""        # e.g. 50K+, ~200, Enterprise
  revenue: ""          # e.g. $5B, unknown
  footprint: ""        # e.g. Global, US-only, EMEA
```

---

## The deal

```yaml
deal:
  stage: ""            # S1–S6
  ae: ""               # Account Executive name
  se: ""               # Solution Engineer name
  meeting_type: ""     # e.g. discovery, demo, technical deep-dive, exec review
  meeting_date: ""     # e.g. 2026-04-15
```

---

## Known pain points

List what you know about their current situation. Free text is fine.
The more specific, the better the story ranking.

```yaml
pain_points:
  - ""    # e.g. "12 regional CMSes, no shared content"
  - ""    # e.g. "Marketing can't publish without engineering"
  - ""    # e.g. "Replacing AEM — too slow, too expensive"
```

---

## Primary use case fit

Which of these best describes what they're evaluating Sanity for?
Mark the primary one and any secondary ones.

```yaml
use_case_fit:
  portal:          false   # Internal portal, brand standards hub, dealer/partner portal
  content_hub:     false   # Single source of truth across channels/brands
  consolidation:   false   # Replacing or merging multiple CMSes
```

---

## Competitive context

```yaml
competition:
  incumbent: ""    # What they're replacing, e.g. AEM, Sitecore, Contentful, homegrown
  also_evaluating: # Other vendors in the process
    - ""
```

---

## Stakeholders

```yaml
stakeholders:
  - name: ""
    title: ""
    role: ""           # e.g. champion, economic buyer, technical evaluator, skeptic
    notes: ""          # e.g. "Cares about developer experience", "Budget holder"
    email: ""
    linkedin: ""
    last_verified: ""  # e.g. "2026-03-30"
```

---

## Key people context

Public statements, podcast appearances, published philosophy from executives
relevant to the deal — even if they're not directly in the buying process.
Include a summary statement and key quotes that intersect with content strategy.

```
[free text — summary, theme analysis, quotes]
```

---

## Sanity angle

What resonates with this prospect? Use their language, not ours.
Connect their situation to Sanity's strengths without pillar labels.

```
[free text]
```

---

## Sanity pillar alignment

Map each pillar to the prospect's specific situation.

| Pillar | Prospect alignment |
|--------|--------------------|
| **Model your business** | |
| **Automate everything** | |
| **Power anything** | |

---

## Discovery gaps

Open questions to clarify in the next interaction.

```yaml
discovery_gaps:
  - category: "buying_process"   # buying_process, technical, stakeholder, timeline, competitive
    question: ""
  - category: "technical"
    question: ""
```

---

## Notes

Anything else relevant — recent news about the company, sensitivities,
what went well or poorly in the last meeting, specific objections raised.

```
[free text]
```
