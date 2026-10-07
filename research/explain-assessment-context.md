# Explain assessment positioning

Research checked: 6 October 2026.

**The complete workflow presents a plausible case for novelty as an assessment-feedback method. No direct match to that complete workflow was identified in this focused review.** The existence of model-building environments, teacher simulation-authoring tools, or diagnostic tutors does not establish that this particular method has already been implemented.

The defining sequence is:

1. A student answers a conventional open-ended subject question in their own words, including the kinds of questions familiar from AP Chemistry or AP Environmental Science.
2. Explain generates an interactive visualization from that actual answer.
3. The visualization serves as feedback on what the response communicates, supporting reflection on correctness, completeness, and comprehension.
4. The student refines the original answer and can inspect the resulting visualization again.

The student's task remains answering the subject question. The system generates the visualization; designing or programming a simulation is not the assessment task. The distinguishing contribution is the use of the generated representation as feedback on a conventional response, followed by revision of that response.

## Contextual comparisons, not direct precedents

| Source | Relevant contribution | Relationship to Explain |
| --- | --- | --- |
| [Bollen and van Joolingen, SimSketch (2013)](https://research.utwente.nl/en/publications/simsketch-multiagent-simulations-based-on-learner-created-sketche/) | Learners draw and assign behaviors; the resulting models run as simulations. | The learner authors a model through sketches and behavior specifications. This does not demonstrate automatic visualization of a conventional written answer as feedback for revising that answer. |
| [SageModeler, Concord Consortium](https://sagemodeler.concord.org/) | Visual systems modeling with static equilibrium and time-based dynamic models. | Learners construct diagrams and relationships. The submitted artifact and learning task differ from Explain's conventional-answer feedback loop. |
| [Kaputa et al., SimStep (2025 preprint)](https://arxiv.org/abs/2507.09664), [CHI 2026 publication](https://doi.org/10.1145/3772318.3791514) | Educators use natural-language goals and editable intermediate representations to generate and refine simulations. | The teacher authors a teaching resource. The paper does not demonstrate a student's ordinary answer being returned as interactive visual feedback for answer revision. |
| [MindTrace, developer's project description (2026)](https://devpost.com/software/mindtrace-1onyjq) | Reasoning is analyzed for suspected misconceptions, followed by a diagnostic scenario and Socratic questioning. | Its described intervention probes an inferred misunderstanding. It does not establish that the submitted answer itself is visualized as the feedback representation. It should not be treated as an equivalent assessment method. |
| [Mootion, developer's repository](https://github.com/Goyam02/mootion-sahAI) | Combines concept-based simulations, student explanations, and teacher diagnostics. | Its described learning sequence begins with generated teaching materials, then obtains and evaluates an explanation. It does not demonstrate the complete response-visualization feedback method. |
| [Li et al., AERA Chat (2025)](https://aclanthology.org/2025.emnlp-demos.39/) | Scores written answers, supplies rationales, and highlights answer components and scoring justifications. | Its visualizations explain scoring decisions and aid marking. The paper does not demonstrate an interactive simulation enacting the student's answer as feedback. |
| [Lee et al. (2021), feedback on scientific arguments using simulation data](https://link.springer.com/article/10.1007/s10956-020-09889-7) | Automated feedback supports revision of arguments and further use of existing groundwater simulations. | Provides pedagogical context for reflection, simulation use, and answer revision. Its described mechanism does not generate a visualization from the student's submitted explanation. |

These comparisons show overlapping goals or components. They are not evidence that Explain's complete assessment-feedback workflow already exists. Conversely, a focused search that finds no direct match does not establish worldwide priority. This review did not reconstruct Explain's first implementation or release date.

## Product source check

Reviewed the public [generation implementation at commit e021234](https://github.com/jivishov/Causalyst/blob/e0212343301fd5494c7b00947f1403ff35caff90/worker/src/lib/openai.ts). The generation and refinement prompts constrain domain content to the student's description. The response payload states that the prompt and rubric are omitted, while the fidelity review compares the generated representation with the submitted description. These rules support the intended answer-as-source mechanism. They do not independently establish that every generated representation is faithful or that students learn more through the workflow.

## Public wording

> An original approach to open-ended assessment feedback. Explain turns students' answers to ordinary science questions into interactive visual feedback they can inspect while reflecting on their understanding and refining their responses.

The potential novelty concerns the complete feedback mechanism and assessment workflow. Deeper comprehension is the intended learning goal. Demonstrated learning gains would require classroom evaluation, and a worldwide-first claim would require a broader systematic review. The earlier comparisons do not invalidate the narrower novelty case.

## Review scope

Searched public scholarly and product sources first for explanation-to-simulation tools, then more narrowly for visualizations or animations generated from student answers and responses as feedback, followed by answer revision. Reviewed original publications, institutional records, official tool websites, and developers' own descriptions. Kept learner model authoring, teacher authoring, diagnosis-driven tutoring, answer-scoring visualization, and visualization of a conventional answer distinct. Did not run third-party AI generation services or treat developers' descriptions as independent effectiveness studies.
