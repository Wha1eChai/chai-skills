# Taste and Craft

Read before actively choosing or reviewing composition, typography, density, color, detail, or motion. The user need not explicitly ask for beauty: original visual implementation includes these decisions. For a narrow issue, read only its relevant sections. Skip mechanical application of an already decided component/token.

**Working output:** concrete visual choices linked to task/identity, or specific critique with reasons. Advice ends with recommendations; a design specification includes usable proportions, type/color roles, and relevant states; implementation must apply the choices in actual components/styles. A before/after specimen is optional when it clarifies a material choice, not mandatory paperwork.

Aim for comfortable readability, salient priorities, and an appealing whole. People should be able to find their way, enjoy the presentation, and recognize the product's character. Typography, color, imagery, spacing, shape, and motion offer a broad expressive vocabulary; select and combine them for the content, audience, and desired experience.

## Turn a reference into a deliberate design

When a concrete reference would strengthen a composition or expression, start with a relevant case in [Positive design examples](positive-examples.md), a supplied reference, or an appropriate project example. Borrow its reasoning and develop an approach for the current brief, including approaches outside the supplied cases. An established local fix can proceed directly.

1. Hold the real content, task, and established identity in view.
2. Select a useful relationship from the reference: a navigation anchor, a text alignment, a rhythm, or an action grouping.
3. Translate it into concrete choices in the existing system. Make priorities distinct through an effective combination of scale, weight, color, imagery, placement, or space. Keep supporting information easy to read and find.
4. Carry the choice through related regions: type, spacing, surfaces, and feedback should support the same intention.
5. Inspect the result with realistic content. Where a material choice remains, compare that dimension; otherwise develop one direction fully.

The output is a more coherent requested artifact, not a mandatory mood board, new skin, or extra report.

## Compose a whole, not a collection of attractive components

Build a recognizable organizing idea around comparison, reading, selection and detail, creation, or a persuasive sequence. Develop composition with the real content and expressive material: imagery can establish rhythm, typography can connect sections, and color can give a group identity.

Ask:
- Does prominence follow the user's decision, or whichever component is easiest to make large?
- Are related elements closer than unrelated ones?
- How do imagery, shape, color, and detail contribute to orientation, atmosphere, recognition, or enjoyment?
- Do repeated patterns remain consistent while distinct regions have appropriate rhythm?

A useful heuristic is to inspect the page at reduced scale: can the major regions and attention order still be understood? This is a composition check, not an accessibility test. Dashboards may require multiple concurrent signals rather than one hero element.

## Typography is structure and voice

Use a deliberate role system: page title, section, body, label, value, metadata, code. Not every role needs a different size. Combine size, weight, spacing, and color without making secondary text unreadable.

For an existing product, retain suitable type choices. For a new direction, one well-chosen family may be enough. Add another only for a clear role or expressive reason. System fonts and common sans families are valid, especially for multilingual tools and performance-sensitive interfaces.

- Product controls generally need a tighter hierarchy than a brand headline.
- Choose prose width for the language and font; 65–75ch is a Latin-text starting point, not a Chinese reading rule. `ch` is based on the zero glyph, not a universal character count.
- Validate Chinese punctuation, mixed scripts, long labels, numbers, IDs, and fallback fonts. Do not copy English uppercase or tracking treatments into Chinese text.
- Use tabular numerals where changing or compared values benefit from stable alignment; label units and align comparable numeric data.
- Use monospace for code and identifiers where helpful, not as a costume for every technical page.
- Balance headings when supported and useful; do not enforce a fixed line count at the expense of meaning.

## Space, proportion, and density

Choose density by task, content, device, and frequency. Tight toolbars can coexist with a generous reading area. Dense does not mean tiny text; spacious does not mean empty filler.

Use an existing spacing scale, or a small coherent one. Give groups stronger separation than elements inside a group. Align related labels, baselines, columns, and actions. Allow optical adjustments where geometric centering looks wrong.

Proportions should express priority: a detail pane needs enough width to read or edit, not whatever remains after oversized navigation. Avoid nested scrolling unless each region has a clear purpose and remains reachable.

Spacing scales are coordination aids, not laws of geometry. Do not reject a necessary optical adjustment because it is not a multiple of four.

## Color, surfaces, and shape

Separate brand expression from action, selection, and status semantics. Color should help users distinguish roles; pair consequential statuses with text, shape, or icons rather than hue alone.

Compose color relationships for legibility, emphasis, atmosphere, and brand recognition. Choose lightness, saturation, hue, area, and adjacency together: a broad colored surface, a vivid accent, a monochrome composition, or several coordinated colors can each support a strong direction. Give important information a distinct presence and maintain readable text and recognizable states across the palette.

Use borders, shadows, and surface changes to express grouping or depth. They may coexist with distinct roles: dividers separate, shadows lift, focus outlines identify interaction. Do not make every panel look like a floating modal.

Cards are useful for independent objects and grouped actions. Nested containers can be appropriate when relationships justify them; avoid nesting that merely adds padding, borders, and visual noise.

Radius should fit scale and containment. For concentric rounded shapes, outer radius approximately equal to inner radius plus inset can be a useful starting point, not a universal formula.

Check actual foreground/background combinations, including alpha, hover, selected, disabled, focus, and theme variants. Subtlety must not erase input boundaries or essential text.

## Recognizable and engaging expression

Develop an identity through relationships among typography, composition, imagery, color, shape, and motion. Carry the selected character across the page so its strongest moments and everyday details feel connected.

Familiar interaction patterns help people act confidently. A product can combine them with a vivid palette, distinctive typography, rich imagery, or precise understated detail. Choose the combination that makes the experience appealing and useful to its audience.

Use imagery that fits the content, with honest provenance and appropriate rights. Decorative imagery must not masquerade as a real product result, customer, testimonial, or performance claim.

## Motion and interaction feel

Decide in this order:
1. Does a transition help explain feedback, state, spatial continuity, or a deliberate expressive moment?
2. How often is it encountered, and does it delay work?
3. Can it be interrupted or reversed cleanly?
4. Does it respect reduced-motion preferences and input methods?
5. Does it remain smooth on target devices?

Frequent actions usually need immediate feedback and minimal choreography. Rare onboarding or expressive surfaces can allow more movement. Do not mandate animation on every button or ban every keyboard-triggered transition.

Prefer compositor-friendly properties when they fit, but do not claim every transform is automatically GPU-accelerated. Layout, blur, clipping, and other effects require measured performance judgment. Follow existing motion tokens and libraries before inventing curves or adding dependencies.

Popover movement should reflect its anchor when useful; modal movement need not. Limit hover-only behavior and provide touch/keyboard equivalents. Preserve comprehension under reduced motion, using instant or gentler transitions as appropriate.

## Final craft questions

Is content comfortable to read and scan? Are important information and actions easy to notice? What makes the experience appealing and recognizable for this audience? Do the design choices work together with long content, multiple states, and narrow space? Check these outcomes in the result, as well as explaining the intention.

Passing technical checks does not prove strong composition. A visually impressive screenshot does not prove correct behavior. Assess both.
