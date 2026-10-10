# Combinatorial Taste

An English guide to `combinatorial-taste-skill`, version **0.1.1**.

This Skill is for people who recognize good website design but need help turning their references into a page of their own. It extracts design relationships, checks which methods work together, establishes a coherent visual language, and builds around the user's real business and content.

## What it covers

- Brand homepages.
- Product landing pages.
- Personal portfolio homepages.

It supports design proposals, redesigns, and runnable implementations. Complex dashboards, complete ecommerce systems, and full multipage products are outside the primary scope. Simple website identification, research organization, and business-logic fixes do not trigger the complete design workflow.

One readable reference is enough. With multiple references, every readable reference is analyzed, but only suitable methods are retained. A finished page does not need to contain an element from every reference.

## How to invoke it

Install the personal Skill at `~/.agents/skills/combinatorial-taste-skill/` on Codex versions that support this directory, or use your platform's supported personal Skill directory. The folder's `SKILL.md` is the discovery entry point; the English documents do not create a second Skill.

Use `$combinatorial-taste-skill` in your request. Matching natural-language requests can also activate it automatically; implicit invocation remains enabled.

Attach or link your references and provide:

- The website's purpose, audience, and primary action.
- Screenshots, accessible website URLs, or screen recordings you like.
- Available brand assets and content, plus any preferences or constraints.
- An existing project and its stack, if there is one.
- Whether you want a design proposal or an implementation, and any device or delivery limits.

Example:

```text
$combinatorial-taste-skill
Use the attached screenshots as references to create an English homepage
for my consulting studio. The audience is small-team leaders and the main
goal is booking an introductory conversation. Write draft copy and create
appropriate original artwork. There is no existing project. Deliver a page
that runs locally, for desktop only.
```

The Skill uses information already provided. It asks at most three questions in one batch only when missing information would change the design direction. Other details use reasonable, briefly stated defaults. The user's explicit scope and constraints take precedence over default checks.

## What happens

1. **Inspect the references.** View the actual rendered pages, images, or readable recording segments. Number sources and distinguish observed facts from design inferences. Unseen regions, animations, and responsive behavior remain unknown.
2. **Compare and compose.** Start with the business goal, identify compatible methods, consider two or three distinct directions internally, and choose the best fit without adding an approval step unless requested.
3. **Unify and implement.** Define concrete design tokens, rebuild the content order and visual focus, and use real content. Existing projects retain suitable design-system and stack conventions.
4. **Check and deliver.** Inspect the actual rendered output and necessary interactions when tools permit, repair observed problems, and report the verified scope and remaining limits.

For a design-only request, the output is an executable page plan with structure, content, visual values, states, and responsive rules. For an implementation request, the output also includes a runnable page and its usage instructions. Publishing or deployment is not implied by a design request.

## English workflow and rules

- [Workflow](references/en/workflow.md): input handling, composition, implementation, review, and delivery.
- [Reference analysis template](references/en/analysis-template.md): evidence, layout relationships, and cross-reference observations.
- [Composition rules](references/en/composition-rules.md): compatibility, competing directions, conflict resolution, and original expression.
- [Design tokens](references/en/design-tokens.md): concrete visual values and calibration against real content.
- [Review rubric](references/en/review-rubric.md): serious defects, quality checks, verification evidence, and bounded self-correction.

The Chinese entry point is [SKILL.md](SKILL.md), with the original Chinese rules in `references/`. The English documents describe the same behavior. Read one language path as needed rather than loading duplicate translations during every invocation. Input and output language follow the user's request.

## Important limits

An accessible reference must actually be viewed. Reading a website's text alone does not verify its appearance. If some sources are unreadable, work continues with the readable sources and explains the limitation; if all are unreadable, readable material is requested.

The Skill transfers methods such as alignment, grouping, crop logic, and visual hierarchy. It does not copy reference logos, proprietary images, copywriting, or a distinctive complete composition. It does not invent clients, metrics, testimonials, or successful submissions to make a page convincing. A simulated booking or form must be clearly identified as a demo.

Code checks do not establish visual acceptance. Unrendered views or untested behavior are marked unverified. Basic accessibility checks are not a complete compliance audit. Synthetic checks and development examples are not formal real-reference evaluations; the separate evaluation plan is a proposed practice threshold, not official certification or a promise of future zero-error performance.

Evaluation records, test cases, and development history stay outside this Skill's runtime resources. No executable helper is included because this workflow currently has no repeated deterministic operation that needs one.
