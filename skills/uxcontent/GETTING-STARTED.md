# UX Content Skill

A reusable AI skill for writing and reviewing product microcopy.

Give the assistant a screen, current wording, audience, and task. It helps produce copy for buttons, forms, validation, errors, confirmations, empty states, onboarding, and professional tools.

## Install

Download the [single-skill ZIP](https://github.com/nancymx-dev/uxcontent-skill/releases/latest/download/uxcontent.zip). Import it if your assistant supports that feature, or copy the entire `uxcontent/` folder (under `skills/` in the repository layout) into its documented skill directory. Reload skills if required by the assistant.

If your assistant does not support skills, attach `SKILL.md` to a conversation and ask it to use the guidance. This supplies context for that conversation rather than installing automatic discovery.

You can also install with the [Skills CLI](https://github.com/vercel-labs/skills):

```sh
npx skills add nancymx-dev/uxcontent-skill
```

## Supply your own context

Attach your content guide and glossary if you want project-specific wording. Include the language or locale, audience, surface, task, character limits, and any approved wording or facts that must be retained.

Without a supplied guide, the skill uses general content practices and identifies assumptions. It does not require a named design system or an internal document service.

Keep private project documents in an approved workspace. Do not upload confidential copy or guidance to a public skill repository.

## Example requests

> Use uxcontent to review this file-upload error. Here is the current copy and screenshot. The upload status is unknown. Give me recommended wording and identify what product information you need before suggesting a retry.

> Use uxcontent to write an empty state for a saved-items screen. The audience is new users, the locale is Australian English, and the primary action adds the first item. Follow the attached content guide.

> Use uxcontent to review these form labels and helper messages. I have no style guide. Use general practices, preserve the meaning, and explain consequential changes briefly.

## Figma access

Screenshots and pasted wording are enough to begin a copy review. If you want the assistant to read your Figma glossary or screen, connect a supported Figma MCP integration and provide the exact selection link. Direct updates also require editing tools, file permissions, and authorization for the target changes.

## Included guidance

- Screen context and a proportionate delivery format.
- Conversational language, clarity, reassurance, and error prevention.
- Labels, commands, placeholders, errors, confirmations, and empty states.
- Locale-aware dates, dynamic values, and accurate certainty language.
- Professional tools and optional screen-naming suggestions.
- Handling conflicts between supplied guidance, approved strings, and product facts.

The skill is design assistance. Product behaviour, accessibility, and any mandatory wording still need the appropriate review in the implemented experience.

## License

[MIT](LICENSE.txt). Created by [Nancy](https://github.com/nancymx-dev).
