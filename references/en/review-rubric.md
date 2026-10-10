# Acceptance Review and Bounded Self-Correction

Use before delivery. Check serious defects first, then assess quality; an average score must not hide a failure. This rubric is for self-review within one task and does not constitute formal trial certification.

## Verification Evidence

For implementations, record startup/build commands and results, the actual location accessed, viewport widths, screenshot files, interaction checks, and issue status. When rendering is possible, actually inspect the page at 1440, 768, and 390 CSS px. For long pages, check the first screen and every major section below it; inspecting only the first screen or the DOM is insufficient. Screenshots demonstrate layout; interactions must be performed separately. If tools are missing or the project cannot run, list the specific unverified items.

A proposal can be checked for content structure, tokens, responsive rules, and state definitions. Do not claim verification of unimplemented pages, actual breakpoints, interactions, font loading, or visual results.

## Serious Defects: Any One Prevents a Passing Acceptance Result

- The page cannot open, or missing critical resources make its main content unusable.
- At 390px, horizontal overflow, overlap, or missing core content interferes with reading or use. Do not hide defects through global clipping.
- Main text is hard to read, has insufficient contrast, or is too small; core content is forcibly truncated.
- Core requirements are missing, primary actions are unreachable, or demo feedback is presented as a real submission. Clearly state delivery boundaries when a required service has not been connected.
- The design directly replicates a reference's distinctive overall composition, or uses reference assets in violation of their usage rules.

## Quality Checks

| Dimension | Observable evidence of passing |
| --- | --- |
| Consistency | The same roles share typography, color, spacing, and component rules; special treatments have a clear purpose |
| Information hierarchy | The first visual focal point supports the goal; real long copy retains a reading order, and the primary action is clear |
| Fit to requirements | All necessary content is present, images and supporting evidence are authentic, and the page structure serves the business goal |
| Distinctiveness | The overall expression differs materially from every reference; it is neither a generic template nor a collage of reference sections |
| Responsive quality | Alignment, wrapping, cropping, overflow, and rhythm are checked at all three viewport widths; the mobile task can be completed |
| Usability and accessibility | Semantic structure is sound, keyboard operation works, focus is visible, and necessary hover/focus/active/error and other states are defined; meaningful images have alt text, decoration does not interfere with screen readers, click targets are easy to reach, and motion respects reduced-motion |

Check only states the page actually needs; do not invent forms or menus. Primary actions should lead to valid targets. When a local demo has limitations, simulated behavior may be clearly labeled, but must not mislead users into believing something was sent or booked. Basic accessibility checks do not constitute full compliance certification.

## Self-Correction and Stopping

Fix serious defects first, then hierarchy/consistency, and finally decoration. Make each adjustment in response to an observed problem, then recheck affected viewport widths and key actions. Continue addressing fixable serious defects. If the same change brings no improvement, diagnose the cause before retrying. Stop random style changes when there is no new evidence, and stop unnecessary iteration once acceptance criteria are met. When tools, resources, or the ability to run the project truly block progress, list the issues, their impact, and unverified items; do not claim success. Continue if the user adds requirements.

Keep the delivery record brief: the final direction and reference decisions, result location, how to run it, completed verification, and unverified items. Keep the full analysis in the work record; the user need not read a design paper. Synthetic smoke tests verify only limited behavior. Generalization to real references, human preferences, and the formal thirty-trial evaluation must be recorded separately.
