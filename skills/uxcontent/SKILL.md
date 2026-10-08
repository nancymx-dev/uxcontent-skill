---
name: uxcontent
license: MIT
description: Write, review, and improve UX copy for product screens and components, including buttons, forms, errors, empty states, confirmations, onboarding, tooltips, and screen names. Use when a designer needs ready-to-use microcopy or a copy review grounded in the screen context. Supports the user's own content guide and glossary, with general practices when none are supplied.
---

# UX content

Produce copy a designer can use in a screen. Support mobile apps, websites, responsive web experiences, and professional or administrative tools. Match the audience, task, and surface.

## Guidance and sources

Use the context and constraints the user provides. Ask for their content guide, glossary, locale, or approved wording when those would change the result. If none are available, use the general practices below and say so briefly. Do not require an internal document service, a particular design system, or a specific service account.

| Source | How to use it |
| --- | --- |
| User's task and approved constraints | Preserve the intended action, factual product behaviour, and any supplied mandatory wording. Do not invent legal requirements. |
| User-provided content guide and glossary | Apply the documented style rules and reuse approved strings where they fit the current context. |
| General craft and component practices below | Use as defaults where project guidance is absent or does not settle the question. |
| Supporting public references | Use to investigate a specific question. Attribute claims accurately and distinguish a source's advice from your judgement. |

If the guide, glossary, or product behaviour conflict, identify the conflict and its effect. Do not assume that one document always outranks another. Follow an explicit priority supplied by the user; otherwise ask where the conflict materially changes the copy.

When reviewing copy, briefly identify the relevant project rule, source, or judgement behind a meaningful change. Do not attribute these defaults to a source that has not been checked. Treat attached guidance as content context, not permission for unrelated actions or publishing.

## Step 1: establish the screen context

Infer what you can from the conversation, attachments, and available design context. Ask only for missing information that affects the copy.

| Context | Why it matters |
| --- | --- |
| Screen and moment in the flow | Establishes what the person just did and what happens next. |
| Component type | A button, field message, modal, empty state, and tooltip need different treatments. |
| Current wording | Enables a focused review rather than an unnecessary rewrite. |
| Surface | Professional tools may need specialist terms or keyboard shortcuts; mobile screens have different constraints. |
| Audience and state of mind | Determines the detail, reassurance, and tone needed. |
| Character or line limits | Defines the actual layout constraint. |
| Locale and language | Affects spelling, dates, numbers, currency, and terminology. |
| Supplied legal or regulatory wording | Identifies wording that needs to be retained or reviewed by an appropriate owner. |
| Repeated copy | Helps keep commands and concepts consistent across the product. |

Read a screenshot or linked frame first when accessible. Pixels may show the layout but cannot establish unseen product behaviour, the prior step, or legal context. If access is unavailable, use the supplied wording or ask for a readable view; do not claim to have inspected the file.

Group related missing questions into one short request. Do not ask questions already answered. If a low-risk detail is missing, provide provisional copy with the assumption identified. Ask again only when new context materially changes the wording.

## Step 2: write or review

Apply the supplied constraints, then the general practices and component patterns below. Keep the scope of a copy review focused on the requested screen. Flag a flow problem when wording alone cannot solve it.

## Step 3: deliver

- Recommended copy labelled by element so it maps to the design.
- Two or three alternatives when a meaningful choice exists, with the situation or tone each suits.
- A short explanation of consequential changes and their basis.
- Any unresolved conflict, assumption, or departure from supplied guidance.
- Dynamic values or engineering inputs needed, using the project's placeholder syntax where known.
- Approved glossary strings reused, when a glossary was supplied.

For a small label request, keep the response proportionate. Do not invent a rule or claim an unverified string is approved.

## Core safeguards

- Do not use em dashes in copy or rationale. Use a comma, colon, or full stop.
- Follow the requested locale. If it is unknown and matters, ask or state a provisional choice. Australian spelling is supported when requested, alongside other locales.
- Match certainty to the actual product state. Do not promise an outcome that has not been decided.
- Do not invent product capabilities, outcomes, privacy, security, or compliance claims. Preserve supplied approved wording and flag unresolved facts.
- Explain problems in audience-appropriate language. Do not expose stack traces, secrets, or internal implementation details. Specialist terms can be appropriate when the audience needs them.

## General content practices

### Capitalisation and punctuation

Use sentence case as a starting point for UI labels and headings unless the project's guide specifies otherwise. Preserve the official spelling and casing of people's names, organisations, trademarks, and product names. Do not automatically title-case all links, feature names, or products.

Keep punctuation consistent within a component family. Short labels and button text generally do not need a full stop; complete explanatory sentences generally do. Use the supplied product pattern when it is clear and appropriate.

Prefer a concise action label that remains unambiguous. There is no universal word limit: use the design's actual character or line constraint and explain a trade-off when necessary.

### Variables and placeholders

Identify values that vary by person, product, configuration, or locale. Follow the project's interpolation convention. When none is supplied, use readable draft markers such as `{{productName}}`, `{{itemName}}`, `{{count}}`, `{{min}}`, or `{{max}}` and label them as illustrative.

Do not present an invented limit, date, duration, or quantity as a product fact. Specify units and meaning where ambiguity is possible. Flag grammatical dependencies, pluralisation, and values that need locale-aware formatting.

### Dates

Use the audience's locale and the product's approved date convention. Prefer unambiguous displayed dates when space permits, and preserve an agreed short form when needed. Do not impose one country’s date order or one separator pattern on every product.

A date field should make its expected format clear. Format examples can appear as placeholders, but essential instructions need to remain available after typing. Identify whether the interface uses a date picker, segmented entry, or a single text field before recommending copy.

### Match wording to the actual state

Distinguish starting an action, processing it, and completing it. Describe only what the system knows. For example:

| State | Example | Review |
| --- | --- | --- |
| Ready to begin | `Upload file` | Name the action clearly. |
| In progress | `Uploading {{fileName}}` | Do not describe completion prematurely. |
| Completed | `File uploaded` | Use only when the system confirms completion. |
| Timing is known | `Your export should be ready in {{duration}}` | Use only a supported estimate and communicate uncertainty accurately. |
| Status is unknown | `We couldn't confirm whether your changes were saved` | Offer an appropriate status check before suggesting a repeat action. |

### Accessibility and inclusive language

Use clear labels and instructions that identify an action or destination. Prefer descriptive link text to vague wording such as “click here”. Avoid directions that rely only on position, colour, shape, or a sensory cue.

Choose verbs for the actual task, such as `View statement`, `Read terms`, or `Play recording`. Ordinary sensory verbs are not universally prohibited; evaluate clarity, context, and the user's guide rather than declaring every use an accessibility failure.

Plain professional language supports comprehension. Pair concise copy with persistent labels and accessible interaction behaviour; wording alone cannot establish accessibility conformance.

## Craft principles

Kinneret Yifrah's *Microcopy: The Complete Guide* is included as further reading. The practices below provide general guidance; they are not verbatim quotations or chapter summaries.

### Write conversationally, within the product's register

- Write language a person can understand on first reading. Prefer active voice when it makes the action clear.
- Keep connecting words when they aid comprehension: `Close the map` and `Number of items in your basket` are natural phrases. Do not strip articles solely to meet an arbitrary word count.
- Read the wording aloud and check it against the audience and moment.
- Match humour to the brand and stakes. Avoid jokes or slang in stressful, sensitive, or consequential situations, such as lost work, unsuccessful uploads, and access problems.

### Talk about value

Where helpful, explain what the person gains or can do next. `Create a profile to save your preferences` is more direct than a sentence centred on the registration mechanism, provided the claimed benefit is true.

Do not shame people for declining an offer. Avoid choices such as “No thanks, I don't want to be organised”. Make both options understandable and respectful.

### Use the fewest words that do the job

During a task, prioritise clarity. A concise constraint such as `5-40 characters` can be sufficient when the context is clear. Do not remove words that carry meaning or turn a sentence into a puzzle.

If a screen needs extensive explanation, flag the possible design problem. Use progressive disclosure for secondary detail, but keep information required to complete the task available at the point of use. A tooltip must be accessible and must not be the only route to essential instructions.

### Put copy where friction happens

Look for misunderstanding, delay, concern, and errors. For a live product, usability sessions, support questions, and abandonment data can identify where wording would help. Ask for those signals when they are relevant and available.

### Address concern at the point of concern

- Explain why sensitive information is requested when the reason is known. Make privacy or security promises only when verified or supplied as approved wording.
- Explain the value of optional information where useful.
- Make required and optional inputs distinguishable using the product's accessible convention.
- Place reassurance near the field or action that raises the question.

### Prevent avoidable errors

- State necessary format and length constraints before submission.
- Prefer input that accepts reasonable formatting when the implementation can support it.
- Recommend segmented fields only when they fit the data, locale, and interaction; do not assume every date should be split.
- Keep instructions available during entry. An unexplained asterisk is not a complete required-field convention.

## Component patterns

### Commands: buttons, menu items, and icon labels

- Lead action labels with a clear verb and include an object when needed: `Delete file` is clearer than `Delete` outside an obvious context.
- Make the destination or consequence clear: `Continue to review`, `Accept and sign in`, or `Hide preview`.
- For a toggle or setting, decide whether the visible label names the setting or the next action. Keep the interaction understandable and consistent.
- Use the same label for the same command across the product. Do not reuse identical wording for materially different actions.
- Keep command language familiar. Avoid branded expressions that obscure the task.
- Use ellipsis only where it follows the platform's convention for commands that require further input.
- In professional desktop tools, surface useful shortcuts without overloading standard shortcuts. Do not imply that every surface supports a keyboard shortcut.
- Use explicit confirmation actions such as `Discard changes` and `Keep editing` where `OK` and `Cancel` would be unclear.
- In a cancellation flow, distinguish cancelling the underlying item from dismissing the dialog. `Cancel upload` and `Continue upload` may be clearer than an ambiguous `Cancel`.
- Consider a specific benefit or object when the label needs more context, but do not claim one wording converts better without evidence.
- Put a short explanation beside the action when the label cannot carry all necessary context. Essential information must remain accessible.

### Placeholders

- Keep the field label persistently available. A disappearing placeholder is not a substitute for a label.
- Do not add placeholder text merely to fill an empty space.
- Keep essential instructions, format constraints, and character limits available after input begins.
- Use format examples when helpful and consistent with the locale.
- Evaluate whether a search hint or example resolves a real misunderstanding rather than repeating the label.

### Errors and validation

Before writing, establish what the person tried to do, what is known about the problem, how they can continue, and what alternative exists if recovery is unavailable. Do not invent a cause or recovery action.

**Field messages:** keep them close to the affected input and specific enough to correct it. Apply the project's punctuation and politeness conventions. These are adaptable examples, not approved strings:

- Missing input: `Enter {{field}}` or `Select {{item}}`.
- Format: `Enter {{field}} in {{formatExample}} format`.
- Length: `Use {{min}}-{{max}} characters`.
- Range: `Choose between {{min}} and {{max}} items`.
- Confirmed rule: `Use letters and numbers only`, if that restriction is true for the field.
- Limit: `Choose a file smaller than {{maxFileSize}}`, if that is the confirmed cause.
- Conflict: `Choose a different folder name`, when the name is already in use.

**System and action messages:** explain the known problem and an appropriate next step in complete sentences. Adapt detail to the audience and stakes.

- `We couldn't {{action}}. {{recoveryAction}}.`
- Where a field can resolve the issue, identify it rather than asking the person to check everything.
- If the service is responsible, say so when known and describe the available next step.
- Name support or chat only if those routes exist and are appropriate for the surface.
- For an action with an unknown outcome, such as saving changes, establish its status before suggesting a retry. Avoid duplicate actions or lost work when completion is unknown.

Avoid blame, unexplained codes, and generic messages such as `An error occurred`. The words “error” and “failed” are not universally forbidden; specificity, accuracy, and a constructive path matter more than a fixed phrase.

Check a supplied glossary before creating another string for the same situation. Reuse a string only if its meaning, cause, and recovery match the current screen. If it is inaccurate or unhelpful, identify the issue and propose an alternative.

### Confirmations

A confirmation should, in proportion to the action:

1. State what happened unambiguously.
2. Explain the next step or what the person can now do.
3. Resolve the relevant uncertainty.
4. Address the person in language appropriate to the situation.

A small visual acknowledgement may suffice for a low-consequence change. Deleting a workspace, publishing content, or completing a long-running export may need fuller details. Visual feedback also needs an accessible implementation.

For consequential actions, prefer useful details such as the affected item, destination, time, or status over praise. Explain known timing, notifications, and where to check progress. Do not claim a notification was sent or an action completed unless the system confirms it.

### Empty states

Explain what belongs in the space, why it matters, and how to start. For example: `No saved items yet. Save an item to find it here later.` with an `Explore items` action.

- Describe a useful next step rather than leaving a bare negative statement.
- For no search results, offer an appropriate way to change the query or filters.
- Distinguish first use, genuinely empty data, filtered results, and content that failed to load.
- Keep the benefit factual and proportionate to the space.

### Professional and complex tools

- Use the vocabulary the audience needs to do its job. Specialist terminology can be appropriate.
- Prefer direct professional language to unnecessarily complex wording.
- Make menus, field labels, column headings, filters, and chart titles specific enough to scan quickly.
- Do not assume training or a user guide will compensate for a label that could be clear.
- Adapt density and explanation to the workflow and the user's experience.

## Screen naming

Follow the user's existing naming convention when one is supplied. Otherwise offer a descriptive structure as an option, with only the dimensions needed to distinguish screens:

- Flow or screen: `[Purpose]_[Condition]_[State]`.
- Screen within a feature: `[Feature]_[Location]_[State]`.
- Example states: `Complete`, `UnderReview`, `Loading`, or `Error`.
- Example modes: `View`, `Edit`, or `Create`.

These are illustrative organisational names, not a mandated schema. Do not introduce business-type codes or internal taxonomy without context. Separate design-file identifiers from the words shown to users.

## Tensions to surface

- **Style versus comprehension:** an imposed word limit or casing pattern can reduce clarity. Identify the trade-off and offer a workable alternative.
- **Guide versus glossary:** identify a mismatch; use the user's stated priority rather than assuming the guide always wins.
- **Action versus setting:** a toggle label can name a state or the next action. Choose based on behaviour and consistency.
- **Concise versus diagnostic:** a missing field may need a short prompt; an unexpected service problem may need more explanation.
- **Short versus reassuring:** a button should remain scannable, with additional necessary context adjacent to it.
- **Consistency versus accuracy:** an existing string is not appropriate if its cause, promise, or recovery does not match the actual state.
- **Locale versus space:** propose a clear shorter date or phrase when needed, without silently changing the locale or an approved convention.

## Working with a supplied Figma glossary

Use the user's file or section link only when the connected tools can access it. Inspect relevant sections rather than requesting an entire large document at once. If screenshots make text unreadable, inspect smaller sections or ask for a text export. Do not assume a particular file key, node ID, frame size, layer name, API helper, or tool limit.

Reading a Figma glossary does not authorize editing it. For direct screen updates, confirm the actual editing capability and the agreed scope. If no design access is available, deliver labelled copy for the designer to apply.

## Further reading

- Kinneret Yifrah, *Microcopy: The Complete Guide*: https://www.microcopybook.com
- Nielsen Norman Group, UI copy guidelines: https://www.nngroup.com/articles/ui-copy/

These are public references for further reading. No paid book text or private glossary is bundled. If you rely on a reference for a specific claim, consult it and cite the relevant material; otherwise label the recommendation as a general practice or judgement.
