# GUS Protocol — source notes for the first revision

Developed by Brazilian data and business analyst Gustavo "Gus" Figueiredo.

Reviewed on November 2, 2026 using the four PDFs supplied by Gus. These notes record the passages used, the distinction between source findings and design choices, and the resulting instruction changes. They are working references for protocol development, not material to append to every partner response or deliverable.

PDF-page references count from the first page of the review copy. Printed page numbers are also given where available. Review focused on the passages identified below; it was not an audit of cited studies, supplementary materials, or the entire research literature. The reviewed PDFs are not included in this repository.

## 1. Collins, Brown, and Holum: cognitive apprenticeship

**Source:** Allan Collins, John Seely Brown, and Ann Holum (1991), [“Cognitive Apprenticeship: Making Thinking Visible”](https://www.aft.org/ae/winter1991/collins_brown_holum). The review copy is a 31-page printout of the public article.

**Passages used:** PDF pp. 1–5 on making practice visible and adapting apprenticeship; pp. 6–10 on reciprocal teaching and shared producer/critic roles; pp. 20–27 on content, methods, sequencing, social context, and the conclusion.

**What the source contributes:**

- Modeling makes the task's processes available to observe. Coaching responds to an actual attempt. Scaffolding can include performing parts the learner cannot yet manage; fading transfers responsibility.
- A picture of the whole task helps the learner understand the purpose of a part. Complexity and variety should develop in ways that retain meaningful context.
- Articulation and reflection include explaining and comparing approaches. Exploration extends autonomy to posing problems, not merely solving assigned ones.
- The conclusion explicitly allows the learner to become the expert and challenge the teacher. It presents an instructional paradigm rather than a packaged formula.

**Changes made:** The core now calls for a compact whole-task orientation, models important decisions, supports both completing and posing problems, and fades support according to observed command. The workplace profile uses one row or comparison as a possible shared example. The school and university profiles use partial completion when helpful.

**Boundary:** The cited teaching examples are not trials of an AI agent or GUS. The protocol retains voluntary participation and human authority rather than importing every teacher/student authority relationship or forcing exploration.

## 2. Chi and colleagues: self-explanation

**Source:** Michelene T. H. Chi, Nicholas de Leeuw, Mei-Hung Chiu, and Christian LaVancher (1994), [“Eliciting Self-Explanations Improves Understanding”](https://doi.org/10.1207/s15516709cog1803_3), _Cognitive Science_, 18, 439–477.

**Passages used:** PDF pp. 1–5 for the question and conceptual framing; pp. 12–17 (printed pp. 450–455) for participants, procedure, group comparisons, and explanation coding; pp. 21–26 (459–464) for verbosity, integration, and component functions; pp. 32–37 (470–475) for mechanisms and limitations.

**What the study did:** Fourteen eighth-grade students were prompted to explain a text about the circulatory system; ten others read the text twice. The prompted group showed greater learning gains. Analyses also examined the content of explanations, inference questions, and mental models. The high/low-explainer comparisons are analyses within the prompted group, not a separate randomized treatment.

**What matters for GUS:**

- In the study's coding, a self-explanation added an inference beyond the given text. A paraphrase or a statement that one understands was not the same kind of contribution.
- Explanations linked new information with existing knowledge and other parts of the text. Focused, partial connections could expose and repair a particular misconception.
- A learner could reproduce an explanation based on the scientific account while retaining a conflicting personal account. Repeating the correct account alone did not establish that the conflict had been resolved.
- The discussion reports incorrect self-explanations as well as correct ones. Articulating a belief can make repair possible; it does not make that belief true or guarantee self-correction.

**Changes made:** The core now favors a focused question about a relationship or inference, distinguishes paraphrase from an explanatory connection, accepts partial formulations, and checks their substance. The academic profiles address a specific conflicting interpretation rather than demanding another polished recital. The voice component supports a small explanatory turn without making speaking time a learning measure.

**Boundary:** This was a small study of a particular text and population. Actual mean study time differed substantially between groups: 2 hours 5 minutes for prompted students versus 1 hour 6 minutes for controls (PDF p. 13). It is not a clean estimate of an isolated prompt effect at equal exposure. The original sentence-by-sentence prompting procedure is not adopted as a universal conversational rule. The study does not demonstrate that voice outperforms text or that diagrams alone produce equivalent effects.

## 3. Sweller: cognitive load

**Source:** John Sweller (2011), “Cognitive Load Theory,” chapter 2, _Psychology of Learning and Motivation_, volume 55, pp. 37–76. This supplied chapter substitutes for the initially suggested journal article.

**Passages used:** Introduction, PDF p. 2 (printed p. 38); intrinsic load and element interactivity, pp. 21–27 (57–63); worked examples, split attention, modality, redundancy, expertise reversal, completion and fading, and transient information, pp. 28–37 (64–73), especially sections 3.3.2–3.3.9 and the conclusion.

**What the chapter contributes:**

- The number of unfamiliar elements that must be processed together matters, along with the learner's existing knowledge. Difficulty is not simply the number of words or items.
- Worked examples can reduce unproductive solution search. With greater expertise, the same guidance can become redundant; partially completed problems provide one route to fading.
- Related representations can impose unnecessary integration work when separated. Additional representations can also be redundant. More explanation is not automatically better instruction.
- Spoken information can disappear before a learner has integrated it with what follows. Section 3.3.9 describes graph-reading studies in which the relative results of audiovisual and visual-only presentation differed between longer and shorter spoken instructions.
- The chapter explicitly cautions against treating instructional effects as universal rules detached from their conditions.

**Changes made:** The core now adjusts guidance to task-specific expertise, avoids a compulsory hint ladder, controls unfamiliar relationships, places explanations near their referents, and reduces redundant teaching. Voice instructions separate multi-action directions, provide persistent exact material when useful, and coordinate complementary speech and visuals without requiring duplicate narration. Requested captions, transcripts, and access needs remain available.

**Boundary:** The instruction to make one main conversational move per turn is a GUS design choice, not a tested threshold from this chapter. The source does not specify an ideal word count for an AI response or establish that every longer explanation is worse. Its graph-reading examples are not tests of free-form voice agents. The original Leahy and Sweller article has not been separately reviewed.

## 4. Bastani and colleagues: AI assistance and learning

**Source:** Hamsa Bastani et al. (2025), [“Generative AI without guardrails can harm learning: Evidence from high school mathematics”](https://doi.org/10.1073/pnas.2422633122), _PNAS_, 122(26), e2422633122.

**Passages used:** Main text, PDF pp. 1–7, particularly experimental design on pp. 2–3, Table 1 and interpretation on p. 4, mechanism analyses on pp. 5–6, and discussion on pp. 6–7. The supplied main paper describes the intervention, but the supplementary appendix and prompt details it references were not reviewed. Per Gus's direction, the correction is outside this conceptual revision.

**What the study did:** It compared two GPT-4 tutoring designs with a control during mathematics review sessions at one Turkish high school. Assisted practice was followed by an unassisted exam. The guarded tutor combined instructions about help with problem-specific teacher-supplied solutions, common mistakes, and hints.

**What matters for GUS:**

- Both AI treatments improved assisted practice performance. The base treatment reduced subsequent unassisted exam performance relative to control. The guarded treatment's unassisted result was statistically indistinguishable from control; the study did not establish that it improved learning over the control.
- The interventions differed in more than whether the agent supplied an answer. This comparison does not isolate a single “Socratic prompt” as the cause of the guarded result.
- Self-reported learning and perceived performance did not reliably track exam outcomes. The interaction analysis supports the authors' proposed reliance mechanism, but is not a separately randomized test of each mechanism.
- The authors identify the study's focus on short-term outcomes and a particular deployment context. Permanent skill atrophy across professions is not measured here.

**Changes made:** The core distinguishes an assisted correction from a new application with less help and treats confidence as insufficient evidence of command. It now explicitly verifies the teaching content and consults supplied solutions before making hints. It preserves direct explanation and worked examples; the study is not used to justify a universal refusal to show answers.

**Boundary:** GUS is not a replication of the paper's tutor, and none of these sources evaluates this protocol. Workplace understanding can include knowing how to use source material and receipts; it need not mean closed-book recall. Long-term independence remains a goal to investigate through actual use, not an outcome already established by this revision.

## 5. Design choices retained for Gus to evaluate in use

The sources inform the instructional methods. The following remain the author's protocol choices: the partner relationship and its authority boundaries; requested execution; optional validation; one main spoken move per turn; and leaving final audience context to the partner. They should not acquire a claim of empirical validation merely because research informs adjacent instructions.

Observe whether real conversations give the partner more control over explanations, decisions, and new questions as support fades. Revise a rule if it produces endless questioning, habitual answer-copying, redundant teaching, or a completed artifact the partner still cannot interpret. Do not infer success from the size of the package or the number of rules.
