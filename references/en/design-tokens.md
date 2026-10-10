# Unified Visual Rules

Use after choosing a direction. Generate concrete values for this task and map them to project variables; no default palette, font, or corner radius suits every business.

## How to Generate Them

Check the existing design system first. Keep suitable semantics, variables, and components. Limit necessary changes to this page and explain them. Translate reference methods into values for shared roles, rather than retaining each reference's parameters in separate sections. Calibrate all values against real content before implementation.

| Category | Required values or rules for this task |
| --- | --- |
| Color roles | canvas, surface, text-primary, text-secondary, accent, on-accent, border; add focus and error/success states when interactions require them. Check contrast for actual adjacent combinations, not just the palette |
| Typography roles | Font stacks, sizes, weights, line heights, and letter spacing for headings, body text, supporting text, and buttons; Chinese fonts and available fallbacks. Define desktop and mobile changes, and avoid inconsistent glyphs caused by English fonts without Chinese support |
| Spacing scale | Discrete spacing values from small to large, mapped separately to component interiors, content groups, and sections. Allow exceptions only for a justified composition |
| Layout | Maximum content width, viewport margins, column counts, gutters, text line widths, and image aspect ratios; collapse layouts according to content and describe the results at 1440/768/390px |
| Component form | Corner radii, borders, shadows, padding, and icon sizes for required components such as buttons, cards, and inputs; keep the same roles consistent |
| Motion | Purpose, trigger, duration, easing, interruptibility, and reduced-motion behavior for necessary effects. Explicitly keep the page static when motion is unnecessary; do not add animation just to fill this table |

Proposal mode also requires concrete values, such as actual colors, font sizes, line heights, and margins, rather than only words such as “clean” or “premium.” In implementation mode, output CSS custom properties or equivalent tokens in the existing stack and have components reference them.

## Content Calibration

- Test wrapping with the user's longest actual headings and paragraphs. Do not force English-style wide letter spacing, all caps, or a fixed single line onto Chinese text. Give headings sensible line breaks and widths; do not fix them by shrinking the whole heading until it is hard to read.
- Use the actual available number and aspect ratios of images, and define crop focal points and alt text. If assets are insufficient, change the composition and how it conveys information; image frames must not depend on nonexistent assets to work.
- Use fluid sizing and necessary breakpoints to fit content. Do not fix the entire page height or scale all elements to the screen. A tablet layout is more than a compressed desktop layout; explicitly define navigation, reading order, and the placement of buttons and images on mobile.
- Body text needs at least 4.5:1 contrast, and large text at least 3:1 (at least 24 CSS px regular or approximately 18.7px bold). Necessary non-text information, such as control boundaries and focus indicators, needs at least 3:1. Do not communicate states through color alone. If contrast cannot be calculated, mark it unverified.
- Avoid adding separate fonts, shadows, and corner radii for different sections. Extend tokens only for exceptions with clear semantic meaning, and check consistency across the whole page.
