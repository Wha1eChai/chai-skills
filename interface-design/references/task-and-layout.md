# Task and Layout Decisions

Read before deciding or reviewing task order, navigation, structural layout, purchase consequences, forms, or cross-page behavior. Skip mechanical cosmetic changes. These questions are prompts for judgment, not mandatory interview fields.

**Working output:** actor/task, necessary information, structural choice and reason, action/state semantics, and next-step continuity. In advice mode, this is a concise recommendation. For a design specification, state the concrete structure, actions, states, and unresolved decisions. For implementation, use these decisions to build the requested flow; prose is not the final deliverable. Persist only when a durable project decision/specification was requested.

This reference owns information and behavior structure. Surface and Style owns expression direction; Taste owns the visual articulation of the chosen structure. Choosing list-detail does not by itself require a new brand direction.

## Task model before component inventory

Identify the actor, object, action, information needed, consequence, and next step. Distinguish documented facts from assumptions. Frequency informs prominence, but do not invent usage statistics. A rare high-risk recovery action may still deserve a stable, discoverable location.

Do not turn every backend resource into a navigation item. Organize around what users understand and accomplish. Distinguish:
- Navigation: changes location.
- Filtering: changes the visible set.
- Selection: changes the active object or objects.
- View switching: changes representation.
- Commands: cause an effect.

Their appearance, URL behavior, focus, and feedback should support their meaning. A tab is not a substitute for an unexplained command.

## Choose layout by information relationships

| Need | Useful starting structure | Check before choosing |
| --- | --- | --- |
| Compare many objects on common attributes | Table or aligned list | Are units, ordering, missing values, and meaningful differences clear? Can it work at narrow widths? |
| Scan distinct media or independently meaningful objects | Cards or gallery | Does each container represent a real object? Does varying content preserve rhythm? |
| Review a queue and inspect an item | List-detail or master-detail | Does detail have enough reading/editing space? Are selection, drafts, return position, and narrow-screen behavior clear? |
| Complete dependent decisions | Grouped form or steps | Are dependencies real? Can steps be removed? Are required context and progress honest? |
| Read or find an explanation | Reading column with navigation/search | Can users locate the answer without reading everything? Are code, tables, and prose allowed different widths? |
| Monitor and diagnose | Overview plus drill-down | Does each metric support a decision? Are scope, freshness, units, thresholds, and exceptions visible? |
| Create or edit media | Workspace with tools, preview, and output/history | Do tools support the artifact without crowding it? Are inputs, versions, job state, and results distinct? |

These structures can combine. Do not force one component type across a page for visual uniformity. Do not hide required comparisons just to remove horizontal density; a usable table may be better than a stack of attractive cards.

## Visual guidance follows the decision

Place information close to the action it supports. Use progressive disclosure for optional detail, not to conceal cost, limitations, destructive effects, or eligibility.

Prioritize regions, then prioritize elements within each region. Prefer a clear primary task where one exists; do not mechanically enforce one primary button across independent work areas.

Choose responsive transitions from content constraints: when comparison, reading, or editing stops working, change structure. Collapse navigation, move detail to an appropriate view, or offer a scoped table strategy. Do not simply shrink every element or hide overflow that contains necessary information.

## Purchases, entitlements, and trust

When a flow involves money or access, determine from available project facts:
- What is being purchased: credit, time, quantity, access, or an independent instance?
- How do existing entitlements change?
- What currency, billing period, usage window, expiry, and exclusions apply?
- When do payment, fulfillment, availability, and actual consumption occur?
- What can the user do after success, pending fulfillment, or failure?

If these are unknown, keep copy provisional or ask the narrow blocking question. Do not pick a business model from code fragments or a familiar checkout template.

Show comparable quantities with comparable units. Give prices their period and material conditions at the decision point. Preserve clear alternatives; do not fabricate scarcity, social proof, savings, or selected defaults that conceal recurring charges.

## Forms and action feedback

Use explicit labels, appropriate input modes, meaningful grouping, and specific action verbs. Validation timing should fit the field and avoid interrupting incomplete input. Do not replace labels with placeholders or prohibit paste without a compelling scoped requirement.

Match action feedback to consequence. A transient toast can acknowledge a low-risk save, but should not be the only location for an important failure or recovery path.

Confirmation is not automatically safer. Prefer a recoverable action when real undo exists; use confirmation for consequential or irreversible actions where appropriate. Do not promise undo, cancellation, retry safety, or restoration unless implemented.

## State and continuity

Select applicable states, not every state for every component:
- Initial loading, background refresh, empty data, filtered no-results.
- Error, partial success, stale information, uncertain result.
- Permission denied, expired session, unavailable capability.
- Draft, submitting, queued, running, completed, failed, cancelled when supported.

Loading is not zero; unknown is not failure; payment is not fulfillment; saving is not publishing. Use vocabulary that matches actual effects.

For a cross-page or asynchronous flow, identify who owns the draft/query/selection and what survives navigation, login, refresh, and object changes. Do not apply an old response to a newly selected object. Preserve input on recoverable failure where safe.

Represent shareable navigation/filter state in URLs where useful, but never expose secrets or sensitive form content there. Some state belongs to a session or local component, not a deep link.

For an uncertain costly operation, help users check its actual status before offering another submission. Keep results discoverable after completion and provide supported next actions.

## Scope guard

Finding a missing API or unclear commercial rule does not authorize implementing it. Report the seam, continue independent design work, and avoid adding dead controls that imply the missing capability exists.
