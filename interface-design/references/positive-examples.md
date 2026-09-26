# Positive Design Examples

Use these cases to expand the possibilities when forming a composition, developing an expression, or comparing plausible alternatives. Start with a relevant case, adapt useful relationships, and combine or extend them for the brief. The cases illustrate reasoning within a larger design space; projects and supplied references can suggest other equally strong approaches. Mechanical edits and settled choices can proceed directly.

**Output:** a chosen approach, concrete design moves, and the reason they fit; a small comparison only if it resolves a material choice. Apply the result in the artifact the user requested. These are original teaching scenarios informed by the linked sources, not copied screenshots or validated implementations.

## Choose a case

| Decision | Case |
| --- | --- |
| Where should extra width go? How should navigation relate to content? | 1. Reading and workspace composition |
| How can one brand feel precise or expressive without changing its identity? | 2. Two typographic voices |
| What should align, and how should groups feel related? | 3. Separate destinations or a shared overview |
| When is a list stronger than a card, and when is a card stronger? | 4. Reviewing one object or several |
| How much motion should a moment earn? | 5. Everyday feedback and milestone expression |

Use the local reasoning without mandatory web access. Consult sources for deeper examples when useful. The inspected source guidance is primarily enterprise and public-service design; it is not a complete reference for consumer, cultural, or artistic expression. Source prose and some example markup were inspected; rendered screenshots, motion, and interactions were not independently verified. These sketches are structural, not visual specimens. No upstream images or code are bundled.

## 1. Reading and workspace composition

**Shared brief:** A technical knowledge product needs readable explanations, discoverable topics, and access to examples. Keep its typography, brand, and content. Decide where space belongs rather than merely widening everything.

### A. Centered reading composition

```text
|                    global header                    |
|            title / short orientation                |
|            reading column                           |
|            example                                  |
|            next section                             |
```

**Design moves:** Center a bounded reading area; use section spacing and a stable text edge to establish rhythm. Let a useful diagram or code example break out of the prose width deliberately. Put light navigation near the reading flow.

**Why it works:** The composition forms a calm, self-contained reading object. Good for a standalone guide, an essay, or a short collection where continuous reading matters more than frequent topic switching.

**Choose another approach when:** Persistent deep navigation is central, or users repeatedly move between distant sections.

### B. Navigation-anchored reading composition

```text
|                    global header                    |
| topic nav | title / content       | local outline   |
| topic nav | bounded prose        | optional help   |
| topic nav | wider code/table area|                 |
```

**Design moves:** Keep navigation and the reading region spatially connected. Bound prose separately from the outer shell. Show a local outline where content depth earns it. On wider screens, preserve the relationship instead of spreading every column apart.

**Why it works:** Users keep a stable location while switching topics. Good for deep documentation and reference-heavy products. A short page may work better without the local outline.

**Choose another approach when:** Navigation overwhelms a simple reading task, or the main work is simultaneous analysis rather than prose.

### C. Expanding workspace composition

```text
|                    global header                    |
| navigation | controls / scope                       |
| navigation | comparison / results | detail          |
| navigation | comparison / results | detail          |
```

**Design moves:** Use additional width for relevant columns, a detail region, or comparison. Keep explanatory paragraphs at a readable measure inside the workspace. When width becomes insufficient, switch structure rather than compressing text indefinitely.

**Why it works:** Extra space increases useful visible information. Good for an API explorer, operational analysis, or a searchable resource collection adjoining documentation.

**Selection:** A and B suit reading; C suits concurrent work. The familiar three-column silhouette is not itself a quality signal. Check the actual content and navigation frequency, then verify the affected width constraints.

**Source basis:** [Carbon 2x Grid usage — Style models](https://carbondesignsystem.com/elements/2x-grid/usage/#style-models) distinguishes centered editorial, left-aligned product/docs, and full-width high-density models. These scenarios adapt the relationships, not Carbon's column counts, breakpoints, or prescribed alignment for all projects.

## 2. Two typographic voices

**Shared brief:** Present the same release guide: title, short summary, three capabilities, one technical example, and a next action. Keep the same content order, font family, palette, and action. Change the expression through proportion, weight, and rhythm.

### A. Precise working guide

**Design moves:** Give the title a clear but compact step above body text. Use medium-weight section headings, regular prose, aligned metadata, and close grouping within each capability. Keep code legible and adjacent to the instruction it supports. Use the accent on the useful action or current location.

**Resulting character:** Competent, quick to scan, ready for repeated consultation. The craft lives in consistent baselines, measured spacing, readable density, and distinction between labels and values.

**Fits when:** Readers know the product and want to act or locate a detail quickly.

### B. Editorial introduction

**Design moves:** Give the title more scale and surrounding space, potentially at a lighter weight. Keep comfortable body text rather than enlarging everything. Let the summary introduce the subject; use stronger section breaks and a deliberate pause around the technical example. Carry a consistent type edge through the page so expressive scale still feels ordered.

**Resulting character:** More inviting and authored, with typography providing presence without a new font, palette, or animation library.

**Fits when:** Readers need orientation and the guide introduces a significant idea. Space is serving comprehension and emphasis, not merely stretching the page.

**Selection:** Repeated lookup favors A; introductory reading may favor B. Both can be good within the same brand. A narrow viewport needs recomposition and sensible title wrapping, not preservation of desktop line breaks. Chinese and mixed-script content need their own font and line-height checks.

**Transferable craft move:** Make the important region distinct using a coordinated combination of scale, space, weight, color, or placement. Keep supporting content comfortably readable and easy to locate. Carry that relationship into the next section so the hierarchy remains recognizable. Holding the palette and font constant here isolates typography for teaching; other briefs can explore those dimensions too.

**Source basis:** [Carbon Typography overview — Productive and expressive type sets](https://carbondesignsystem.com/elements/typography/overview/) describes compact product typography and more dramatic editorial typography in one family. The paired release-guide treatments here are our synthesis, not IBM examples or a requirement to use IBM Plex or its scale.

## 3. Separate destinations or a shared overview

**Shared brief:** Show four areas of a service with a name, status, short explanation, and detail action. Use the same four items; decide what their grouping should communicate.

### A. Distinct destinations

```text
Section heading
| Area A           |    | Area B           |
| Status / summary |    | Status / summary |
| Open details     |    | Open details     |

| Area C           |    | Area D           |
| Status / summary |    | Status / summary |
| Open details     |    | Open details     |
```

**Design moves:** Give each independent destination a clear boundary and enough separation. Align titles and corresponding content roles; accommodate longer text without clipping. Use consistent action placement where practical, not a fixed card height that truncates meaning.

**Why it works:** Each item is understood as independently selectable. Useful for a resource catalog or entry screen.

### B. One composed overview

```text
Service overview                     Updated / scope
| Area A             | Area B                       |
| status / summary   | status / summary             |
|--------------------|------------------------------|
| Area C             | Area D                       |
| status / summary   | status / summary             |
```

**Design moves:** Group the areas in a common surface with lighter internal divisions. Align labels, values, and text starts across regions. Place shared scope/freshness once above the group; keep object-specific information local.

**Why it works:** The areas read as parts of one larger picture. Useful when a user judges the service as a whole before investigating an area.

**Selection:** Use separation to express independence, and continuity to express a shared picture. Responsive stacking should retain each area's identity in either approach.

**Transferable craft move:** Decide whether the main alignment is a text edge, a value column, or a container edge. A heading above padded cards may align with their inner text rather than their outer borders. Repeat that chosen relationship consistently; adjust the grid or inset deliberately, rather than adding unrelated nudges.

**Source basis:** [Carbon 2x Grid usage — Gutter modes and mixing modes](https://carbondesignsystem.com/elements/2x-grid/usage/#gutter-modes) relates spacing and typographic alignment to independent destinations versus information forming a larger picture. Adapt that intent to the existing layout system; its exact gutters are not universal tokens.

## 4. Reviewing one object or several

**Shared brief:** Help someone check entered details, correct an answer, and submit. Keep the actual business consequence and draft semantics unchanged.

### A. One object's summary

```text
Check application
Contact
Name       Sample applicant                 Change
Email      applicant@example.test           Change

Application
Type       Selected option                  Change

[Submit application]
```

**Design moves:** Use headings and aligned label/value/action rows. Keep change actions close enough to their values to be associated easily. Short answers can use a bounded width; long answers may need more room. Make the final action explicit.

**Why it works:** The page reads as one coherent record rather than unrelated boxes. Fits one object with a manageable set of sections.

### B. Several identifiable objects

```text
Check participants
+ Participant A                      Remove +
| Name       Sample person A         Change |
| Details    ...                     Change |
+-------------------------------------------+
+ Participant B                      Remove +
| Name       Sample person B         Change |
| Details    ...                     Change |
+-------------------------------------------+
[Submit application]
```

**Design moves:** Give each object a distinct heading and container. Put object-level actions in its heading region and field-level actions beside fields. Preserve consistent role alignment while allowing content to vary.

**Why it works:** The container clarifies identity and action scope. Fits repeated people, addresses, appointments, or similar records. Visible labels may repeat; accessible action names should identify the affected object/field.

**Selection:** Object count and action scope determine whether cards add clarity. For either approach, editing should preserve previous input and return users to the appropriate review position, subject to real dependencies. The examples are synthetic; removal and submission controls apply only if supported.

**Source basis:** GOV.UK [Summary list](https://design-system.service.gov.uk/components/summary-list/) distinguishes plain summaries from summary cards for multiple same-type objects or whole-list actions. [Check answers](https://design-system.service.gov.uk/patterns/check-answers/) explains answer-length-based width choices and returning from changes. Borrow the relationship and continuity, not the government's visual identity.

## 5. Everyday feedback and milestone expression

**Shared goal:** Confirm a completed action without disconnecting the user from the next useful step.

**A. Frequent work:** A local saved state appears beside the edited object, with immediate feedback and a brief or instant transition. Focus and working position remain stable. Useful when a person saves or updates repeatedly.

**B. Meaningful milestone:** First-time setup completion receives a more prominent success region and a clear next step. A short, coordinated reveal can mark the transition if it suits the brand and does not delay action. The static or reduced-motion version communicates the same result.

**Selection:** Actual completion, frequency, and significance earn the treatment. Richer expression can be appropriate; familiarity can be appropriate. Avoid adding a celebratory pause to every ordinary action.

**Source basis:** [Carbon Motion overview](https://carbondesignsystem.com/elements/motion/overview/) provides productive and expressive motion with contextual easing/duration guidance. These paired scenarios are our synthesis; the source motion was not independently played or measured in this research.

## Use a reference as a design move

Identify the relationship worth borrowing and adapt it to actual content and existing components. For example, keeping navigation connected to readable prose can lead to several layouts depending on content depth and available space. Evaluate the result by readability, priority, visual appeal, and task fit rather than resemblance to the sketch.

Where the choice is already clear, implement one coherent direction. Where uncertainty matters, compare the relevant dimension while holding content and constraints constant. Judge the result with real content and appropriate rendered checks; links and structural sketches are not visual acceptance evidence.
