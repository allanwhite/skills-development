# Demo Plan Template

*Load this when generating a demo plan from discovery notes. Produce each
section below, adjusting depth based on the prospect's use case tier.*

---

## Demo Narrative Arc

The story to tell during the demo, in order. Not every demo needs all seven
steps — skip what isn't relevant to the prospect.

1. **Acknowledge their world.** Mirror their current state and pain back to them.
   Use their language from discovery. ("You told us [pain]. Here's how we
   think about solving that.")

2. **Content model.** Show structured content that matches their use case.
   Explain why this matters for their specific pain — content reuse, editorial
   autonomy, multi-channel delivery, or whatever surfaced in discovery.
   *Connects to: Model your business.*

3. **Studio experience.** Show editing workflows tailored to their editor
   personas. Focus on what unblocks editors from needing developers — custom
   document views, page builder patterns, visual editing.
   *Connects to: Model your business.*

4. **Delivery and APIs.** Show GROQ, CDN, and Live Content API if relevant to
   their channel needs. Connect to their tech stack (Next.js, Nuxt, etc.)
   and show how content reaches their surfaces.
   *Connects to: Power anything.*

5. **Automation and AI.** Show Content Releases, Functions, or Content Agent
   if relevant to their operational pain. Only include this if they have a
   clear automation or AI trigger from discovery.
   *Connects to: Automate everything.*

6. **Enterprise features.** Show only what maps to their enterprise triggers.
   Load `triggers.md` for the full mapping.

7. **Comparable customer story.** Match by use case and industry where possible.
   If no close match exists, match on pain pattern instead.

---

## Demo Plan Document Structure

When producing a demo plan, include these sections:

### 1. Prospect context
2-3 sentences. Summarize their current state, primary pain, and what they're
trying to achieve. Use their language from discovery, not Sanity marketing
language.

### 2. Demo narrative
Walk through the arc above, noting specifically what to say and show at each
step. Be concrete — name the schema types, the Studio views, the API calls.

### 3. What to show
A list of features and capabilities to demonstrate. For each:

- **Feature:** What to show
- **Why:** How it connects to their stated pain
- **How:** What to prepare or build (e.g., "create a sample product schema
  with variant references," "configure a custom desk structure for their
  editorial team")

### 4. What to build or prepare
The SE's prep checklist before the demo:

- Schema or content model to create
- Studio customizations to configure
- Sample content to populate
- Integrations or API examples to prepare (GROQ queries, webhook examples,
  framework integration)
- Slides or visuals needed

For **High tier** prospects: build a custom Studio instance that mirrors their
use case. Populate with realistic sample content using their domain language.

For **Standard tier**: adapt an existing demo environment with relevant schema
and content examples.

For **Light tier**: use the standard demo with verbal mapping to their use case.

### 5. Competitive positioning notes
Include only if a competitor is in the evaluation. 2-3 key differentiators
to emphasize during the demo. Frame as "what we do" not "what they can't do."

For detail beyond the quick-reference in SKILL.md, load
`/mnt/skills/user/sanity-messaging/references/competitive-positioning.md`.

### 6. Risks and objections
Likely objections based on the prospect's persona and context. For each:

- **Objection:** What they might push back on
- **Response:** How to address it, grounded in their specific situation

Common patterns:

| Persona | Typical objection | Response angle |
|---------|------------------|----------------|
| CTO / VP Eng | "Is this just another CMS?" | Position as Content Operating System — model, automate, power |
| CTO / VP Eng | "Will we hit its limits?" | Schema-as-code, App SDK, Functions — you build on it, not around it |
| Product Manager | "Is this too technical for our editors?" | Show Studio customization — editors get a tailored UI, not a developer tool |
| Product Manager | "Will this slow down delivery?" | Show developer velocity — schema-as-code, AI-assisted dev, modern stack |
| Lead Developer | "Is this better than building it ourselves?" | Content Lake, real-time APIs, Functions — platform primitives, not a black box |
| Lead Developer | "Can it integrate with our stack?" | Show API-first architecture, framework compatibility, webhook/function patterns |

For persona-specific messaging depth, load
`/mnt/skills/user/sanity-messaging/references/personas.md`.
