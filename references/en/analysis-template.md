# Reference Analysis Template

Use while examining references. Create one record for each readable reference; analyze unsuitable references before discarding them. This is a working record and need not be delivered to the user verbatim.

## Evidence Inventory

| Field | What to record |
| --- | --- |
| ID and source | R-number, file or URL, screenshot dimensions, recording timestamp; clearly label synthetic materials |
| Readability | Readable, partly readable, or unreadable; actual observation scope and reasons for failure |
| Page purpose and character | Known business context; explain its character through visible design relationships rather than a list of adjectives |
| Evidence location | Image region, scroll position, or frame timestamp; save screenshot locations when needed |

Visual analysis requires viewing the visuals. If a URL cannot render, text can help explain the business, but mark the visual analysis unreadable. A long screenshot establishes only the captured scope; a screenshot crop does not establish the real container boundaries. If fonts, colors, or dimensions cannot be identified accurately from an image, record estimates or ranges rather than claiming exact CSS values. Hover states, scroll stages, mobile layouts, and transitions absent from a recording remain unknown.

## Analysis Table for Each Reference

For each row, record “observed facts + evidence,” “design inferences + confidence / needs verification,” and “transferable relationships.” Explain why a dimension is inapplicable or unobservable; do not invent content to fill the table.

| Dimension | Relationships to record |
| --- | --- |
| Hierarchy and reading | Order of headline, body, CTA, and images; contrast strength; main visual focus; how these support the task |
| Grid and proportions | Column count, alignment lines, content width, text-to-image proportions; distinguish measurable dimensions from visual estimates |
| Typography | Roles of headline, body, and supporting text; size steps, weight, line height, and letter spacing; whether Chinese glyphs actually appear |
| Color | Roles and approximate areas of background, text, and accent colors; how local contrast directs attention |
| Spacing and rhythm | Spacing within lines, components, and between sections; visible evidence of density changes, grouping, and scrolling rhythm |
| Images | Subject position, composition, cropping, proportions, and relationship to the background; how illustrations or product views explain the content |
| Components | Corner radii, borders, shadows, sizes, and icon stroke or fill style; shared rules |
| Interaction and motion | Observed triggers, feedback, and estimated durations; mark unseen behavior unknown |

Rewrite vague judgments as actionable relationships. For example: “The headline occupies roughly 40% of the width on the left and shares a bottom alignment line with the product image on the right. The primary button follows the summary; readers first understand the purpose, then see evidence and act.” Then assess whether this relationship accommodates the user's long Chinese headline rather than copying the proportions directly.

## Cross-reference Summary

List shared patterns, significant conflicts, transferable methods, unusable brand assets, and unknowns. Distinguish “the reference appears suitable” from “suitability has been verified with actual content.” Unknowns may be resolved through reasonable design decisions, but those decisions must not be attributed to the reference.
