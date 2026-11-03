# GUS Protocol

Developed by Brazilian data and business analyst Gustavo "Gus" Figueiredo.

GUS is a protocol for working and learning with an AI partner while retaining curiosity, understanding, judgment, and ownership. It develops the collaborative approach of Gus's LFI Protocol for broader settings.

## Choose a version

Every version combines the [shared protocol](protocol.md) with one profile:

| Version | Use it for |
| --- | --- |
| [School](profiles/school.md) | Learning school subjects, working through exercises, and developing explanations |
| [University](profiles/university.md) | Advanced study, disciplinary reasoning, research reading, and academic projects |
| [Workplace](profiles/workplace.md) | Learning through investigations and producing work the human can explain and own |

[Voice](components/voice.md) is a component of all three versions. The partner layer records the person's main interaction mode and activates the appropriate voice instructions. Dictating a message and listening to a response are separate preferences.

## How the collaboration works

The [shared protocol](protocol.md#2-layers-and-transitions) defines five layers:

1. **Partner:** reuse or establish the person's name, relevant context, and interaction preferences.
2. **Context:** establish the goal, audience, and requirements; read requested material, then invite thoughts or offer help going through it. Reflection is optional.
3. **Investigation:** use that context to locate the starting point, choose useful support, and agree on the next unit of work.
4. **Production and learning:** explain or build the accepted increment, check it, show it, and pause for discussion and a go-ahead before the next.
5. **Validation (optional):** offer relevant feedback or rehearsal; the partner decides what to change.

Resume at the earliest unresolved point. Reuse available context and do not turn a specific mechanical request into a new interview.

## Working modes

The default is collaborative: agree on meaningful increments for lengthy work, complete and show one increment, then pause for the partner's thoughts and a go-ahead before starting the next. An approved multi-step plan still includes those pauses.

For an emergency or another task that needs uninterrupted execution, say something like: **“Use fire-and-forget mode to finish the work in the agreed outline.”** The agent completes that scope without learning questions or intermediate review pauses, retaining normal verification and scope boundaries. The fallback ends with the task; subsequent tasks return to collaboration. See [the core's mode rules](protocol.md#21-working-modes).

## Try it in a fresh conversation

Download or clone this repository and make the folder available to your agent. From the repository folder, paste:

```text
Read protocol.md and profiles/school.md. Use the GUS Protocol for this conversation. Reuse any partner details already available. Ask only for missing setup details, including how I mainly interact, and then help me with my task. Apply the voice component when relevant. Do not install anything or change my default working instructions.
```

Replace `profiles/school.md` with `profiles/university.md` or `profiles/workplace.md` as appropriate. If the agent is working outside the repository folder, include the folder's path. The agent must be able to read these files; otherwise supply the core, selected profile, and voice component as attachments or text.

The files are ordinary Markdown instructions. They do not depend on a particular model, a skill installer, or integrations. A skill wrapper can be added later if useful for discovery; it would load these instructions rather than define a second protocol.

## Partner persistence

The core explains how to reuse or save a small partner record in the person's designated personal instruction file. The record includes interaction preferences. It does not change the default working style or contain task history. If no personal file is designated, use the details in the current conversation and offer persistence without blocking the task.

## Readings and source-based changes

The first source-based revision uses the four PDFs Gus supplied: Cognitive Apprenticeship, Chi et al. on self-explanation, Sweller's chapter on cognitive load, and Bastani et al. on AI-assisted mathematics. The [source notes](references/source-notes.md) identify the passages, their implications, and the changes made.

The resulting instructions make guidance responsive to prior knowledge, use focused self-explanations, provide a path from worked examples through partial completion to less supported use, verify teaching content, and account for the memory demands of voice. These sources inform the design; they do not establish the effectiveness of GUS itself.

The [reading list](references/reading-list.md) distinguishes supplied readings from optional further work. The original voice article is no longer needed for this revision because Sweller's supplied chapter addresses the relevant effects.

## License and attribution

Copyright © 2026 Gustavo "Gus" Figueiredo.

The GUS Protocol is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). See [LICENSE](LICENSE) for the full terms.

When sharing the protocol or adaptations, credit the author, link to the source and license, and indicate any changes. Suggested attribution:

> GUS Protocol, developed by Brazilian data and business analyst Gustavo “Gus” Figueiredo. Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

This license covers the original protocol text. Cited publications retain their respective licenses.
