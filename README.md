# GUS Protocol

Developed by Brazilian data and business analyst Gustavo "Gus" Figueiredo.

GUS is a protocol for working and learning with an AI partner while retaining curiosity, understanding, judgment, and ownership. It develops the collaborative approach of Gus's LFI Protocol for broader settings.

## Choose a profile

Start with [General / everyday use](profiles/general.md), a short profile you can use on its own. For a specialist setting, combine the [shared protocol](protocol.md) with the relevant profile:

| Profile | Use it for |
| --- | --- |
| [General / everyday use](profiles/general.md) (default) | Everyday questions, curiosity, personal planning, creative work, and conversation |
| [School](profiles/school.md) | Learning school subjects, working through exercises, and developing explanations |
| [University](profiles/university.md) | Advanced study, disciplinary reasoning, research reading, and academic projects |
| [Workplace analysis](profiles/workplace.md) | Learning through investigations and producing work the human can explain and own |
| [Software development](profiles/software-development.md) | Pairing on code, debugging, and design through small working changes reviewed together |

During first partner setup, the agent presents all five profiles and asks what you mainly use AI for. You can choose several or begin with General. A clear request can proceed first; setup questions do not block an ordinary answer. You can switch profiles at any time.

[Voice](components/voice.md) applies to every profile. Partner setup records the person's main interaction mode and activates the appropriate voice instructions. Dictating a message and listening to a response are separate preferences.

## How the collaboration works

The [shared protocol](protocol.md#2-layers-and-transitions) defines five layers:

1. **Partner:** reuse or establish the person's name, main uses, optional default profile, and interaction preferences.
2. **Context:** establish the goal, audience, and requirements; read requested material, then invite thoughts or offer help going through it. Reflection is optional.
3. **Investigation:** use that context to locate the starting point, choose useful support, and agree on the next unit of work.
4. **Production and learning:** explain or build the accepted increment, check it, show it, and pause for discussion and a go-ahead before the next.
5. **Validation (optional):** offer relevant feedback or rehearsal; the partner decides what to change.

Resume at the earliest unresolved point. Reuse available context and do not turn a specific mechanical request into a new interview.

General distills this approach for everyday use: answer direct questions directly, offer explanations or thinking help when useful, preserve the person's judgment and voice, and keep the work proportionate. A simple answer can be complete without a lesson. Substantial work still uses reviewed increments.

## Working modes

The default is collaborative: agree on meaningful increments for lengthy work, complete and show one increment, then pause for the partner's thoughts and a go-ahead before starting the next. An approved multi-step plan still includes those pauses.

For an emergency or another task that needs uninterrupted execution, say something like: **“Use fire-and-forget mode to finish the work in the agreed outline.”** The agent completes that scope without learning questions or intermediate review pauses, retaining normal verification and scope boundaries. The fallback ends with the task; subsequent tasks return to collaboration. See [the core's mode rules](protocol.md#21-working-modes).

## Try it in a fresh conversation

Download or clone this repository and make the folder available to your agent. From the repository folder, paste:

```text
Read profiles/general.md and use the GUS Protocol for this conversation. Reuse any partner details already available. During setup, present the available profiles and ask about my main uses if unknown; help with a clear request first. Ask only for missing interaction preferences and apply the voice component when relevant. If I choose a specialist profile or my task clearly calls for one, read protocol.md and that profile. Do not install anything or change my default working instructions.
```

For a specialist setting, ask the agent to read `protocol.md` plus `profiles/school.md`, `profiles/university.md`, `profiles/workplace.md`, or `profiles/software-development.md`. If the agent is working outside the repository folder, include the folder's path. The agent must be able to read the required files; otherwise supply the General profile, or the core and selected specialist profile, as attachments or text. Include the voice component when relevant.

For software development, ask the agent to read `protocol.md` and `profiles/software-development.md`. Together, trace the relevant behavior and agree on a short sequence of working changes. The agent builds and checks one increment, shows the behavior and important code, then stops for discussion and a go-ahead. Pair review and rubber ducking run in both directions. Later steps adapt to what you learn; approving the outline does not waive the pauses.

The files are ordinary Markdown instructions. They do not depend on a particular model, a skill installer, or integrations. A skill wrapper can be added later if useful for discovery; it would load these instructions rather than define a second protocol.

## Partner persistence

The core explains how to reuse or save a small partner record in the person's designated personal instruction file. It includes stated main uses, interaction preferences, and a default profile only if explicitly chosen. A profile chosen for one task does not become a permanent default; a saved default applies when it fits the current task. If no personal file is designated, use the details in the current conversation and offer persistence without blocking the task. Saving these preferences does not install GUS as a default working style or store task history.

## Research and sources

The learning guidance draws on four readings: Cognitive Apprenticeship, Chi et al. on self-explanation, Sweller's chapter on cognitive load, and Bastani et al. on AI-assisted mathematics. The [source notes](references/source-notes.md) identify relevant passages and explain how they inform the instructions.

The instructions make guidance responsive to prior knowledge, use focused self-explanations, provide a path from worked examples through partial completion to less supported use, verify teaching content, and account for the memory demands of voice. These sources inform the design; they do not establish the effectiveness of GUS itself.

The [reading list](references/reading-list.md) records reviewed sources and suggests further reading. Sweller's chapter provides the source for the voice guidance on memory demands.

The software development profile draws on the [Agile Manifesto](https://agilemanifesto.org/) and its [principles](https://agilemanifesto.org/principles.html). Its pairing loop and required review pauses apply those principles to human–agent work. They are GUS design choices, documented in the [source notes](references/source-notes.md#6-software-development-agile-principles).

## License and attribution

Copyright © 2026 Gustavo "Gus" Figueiredo.

The GUS Protocol is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). See [LICENSE](LICENSE) for the full terms.

When sharing the protocol or adaptations, credit the author, link to the source and license, and indicate any changes. Suggested attribution:

> GUS Protocol, developed by Brazilian data and business analyst Gustavo “Gus” Figueiredo. Licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

This license covers the original protocol text. Cited publications retain their respective licenses.
