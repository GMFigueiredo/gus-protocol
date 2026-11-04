# GUS Protocol

Developed by Brazilian data and business analyst Gustavo "Gus" Figueiredo.

GUS is a set of instructions that helps your AI assistant act as a Socratic collaborator: asking relevant questions, helping you think through a problem, and suggesting approaches when you want help. You stay involved in the reasoning and decisions, so you can understand and explain what you produce together.

The AI can research, write, and build. For longer tasks, it agrees on small pieces with you, completes one, and stops to show the work and discuss it before continuing. Simple questions still get direct answers.

The goal is to keep learning and curiosity part of using AI, and avoid the habit of handing in work you cannot explain. This addresses the problem described in Molly Graham's [Lazy F'ing Interns](https://mollyg.substack.com/p/lazy-fucking-interns): passing along work without enough understanding or judgment. GUS develops the author's LFI Protocol for everyday use, school, university, workplace analysis, and software development.

## How to install

You can try GUS in one conversation or make it your usual working style. The instructions are ordinary text files; you do not need a plugin or a particular AI model.

### Try it in one conversation

On GitHub, click **Code → Download ZIP**, then unzip the folder. Open that folder in your AI agent and send:

```text
Read profiles/general.md and use the GUS Protocol for this conversation. Reuse any partner details already available. During setup, present the available profiles and ask about my main uses if unknown; help with a clear request first. Ask only for missing interaction preferences and apply the voice component when relevant. If I choose a specialist profile or my task clearly calls for one, read protocol.md and that profile. Do not install anything or change my default working instructions.
```

If you use a chatbot that accepts file uploads, attach `profiles/general.md` instead and ask it to follow the attached instructions. Start with General / everyday use; the agent will introduce the other profiles. If you choose a specialist profile, also provide `protocol.md` and that profile's file. Include `components/voice.md` when relevant.

### Use GUS in future conversations

If your agent can read local files and edit its saved instructions, keep the unzipped folder somewhere permanent and send:

```text
Set up GUS as my default working style. Read profiles/general.md in this folder. Find the personal instruction file this app actually loads, preserve its existing content, and add an instruction to read the General profile using its absolute local path. Keep specialist profiles available for relevant tasks. Reuse my existing partner record, and read the Partner layer in protocol.md before saving any missing preferences. Verify the saved instructions and tell me how to check them in a fresh conversation. If this app cannot load these files across conversations, explain that instead of claiming setup succeeded.
```

For a chatbot with saved custom instructions, you can paste the contents of `profiles/general.md` there if they fit. References to other files still need those files to be available in the conversation. Otherwise, attach the General profile when starting a new chat.

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

For software development, ask the agent to read `protocol.md` and `profiles/software-development.md`. Together, trace the relevant behavior and agree on a short sequence of working changes. The agent builds and checks one increment, shows the behavior and important code, then stops for discussion and a go-ahead. Pair review and rubber ducking run in both directions. Later steps adapt to what you learn; approving the outline does not waive the pauses.

## How the collaboration works

The [shared protocol](protocol.md#2-layers-and-transitions) defines five layers:

1. **Partner:** reuse or establish the person's name, main uses, optional default profile, and interaction preferences.
2. **Context:** establish the goal, audience, and requirements; read requested material, then invite thoughts or offer help going through it. Reflection is optional.
3. **Investigation:** use that context to locate the starting point, choose useful support, and agree on the next unit of work.
4. **Production and learning:** explain or build the accepted increment, check it, show it, and pause for discussion and a go-ahead before the next.
5. **Validation (optional):** offer relevant feedback or rehearse with a reviewer playing the intended stakeholder or recipient. The partner gets a chance to explain their choices and important reasoning before the agent supplies answers, supporting their command of the work. The partner decides what to change.

Resume at the earliest unresolved point. Reuse available context and do not turn a specific mechanical request into a new interview.

General distills this approach for everyday use: answer direct questions directly, offer explanations or thinking help when useful, preserve the person's judgment and voice, and keep the work proportionate. A simple answer can be complete without a lesson. Substantial work still uses reviewed increments.

## Working modes

The default is collaborative: agree on meaningful increments for lengthy work, complete and show one increment, then pause for the partner's thoughts and a go-ahead before starting the next. An approved multi-step plan still includes those pauses.

For an emergency or another task that needs uninterrupted execution, say something like: **“Use fire-and-forget mode to finish the work in the agreed outline.”** The agent completes that scope without learning questions or intermediate review pauses, retaining normal verification and scope boundaries. The fallback ends with the task; subsequent tasks return to collaboration. See [the core's mode rules](protocol.md#21-working-modes).

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
