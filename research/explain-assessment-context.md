# Explain assessment positioning

Research checked: 6 October 2026.

The strongest supported positioning is **a distinctive workflow within an emerging approach to formative assessment**. Student-created executable models, natural-language simulation authoring, and reasoning-driven diagnostic simulations have published precedents. This focused review cannot establish that Explain invented question-response-to-simulation assessment or was the first implementation.

Explain's specific design starts with a student's own answer to an ordinary open-ended science question, generates an interactive representation of that stated explanation, and places exploration and revision inside a teacher-managed assessment workflow. Its generation policy makes the student's text the source of domain facts and intentionally omits the assessment prompt and rubric. This is an implementation distinction and a design aim; it does not prove that every generated artifact is faithful or that the workflow improves learning.

## Related work

| Source | Relevant contribution | Relationship to Explain |
| --- | --- | --- |
| [Bollen and van Joolingen, SimSketch (2013)](https://research.utwente.nl/en/publications/simsketch-multiagent-simulations-based-on-learner-created-sketche/) | Learners draw and assign behaviors; the resulting models run as simulations. | Establishes a long-standing precedent for learners externalizing ideas as executable models. It uses sketches and behavior specifications rather than free-response generation. |
| [SageModeler, Concord Consortium](https://sagemodeler.concord.org/) | Visual systems modeling with static equilibrium and time-based dynamic models. | Establishes accessible learner modeling; the documented interface uses diagrams and relationships. |
| [Kaputa et al., SimStep (2025 preprint)](https://arxiv.org/abs/2507.09664), [CHI 2026 publication](https://doi.org/10.1145/3772318.3791514) | Educators use natural-language goals and editable intermediate representations to generate and refine simulations. | Shows that natural-language educational simulation generation predates the current review. Its described workflow centers on teacher authoring. |
| [MindTrace, developer's project description (2026)](https://devpost.com/software/mindtrace-1onyjq) | Student reasoning is analyzed for possible misconceptions, followed by an interactive diagnostic scenario and further questioning. | A close contemporary example connecting student explanation and simulation. The page records project creation on 3 September 2026. These are prototype authors' descriptions, not independent evidence of classroom effectiveness. |
| [Mootion, developer's repository](https://github.com/Goyam02/mootion-sahAI) | Combines natural-language simulation generation, student explanations, and teacher diagnostics. | Its described sequence begins with concept-based learning materials and simulations, then obtains and evaluates a student explanation. It is an adjacent implementation rather than the same answer-as-model-source workflow. |

The dates above concern the reviewed publications and public descriptions. This review did not reconstruct Explain's first implementation or release date, so it does not rank Explain and the contemporary prototypes chronologically.

## Product source check

Reviewed the public [generation implementation at commit e021234](https://github.com/jivishov/Causalyst/blob/e0212343301fd5494c7b00947f1403ff35caff90/worker/src/lib/openai.ts). The generation and refinement prompts constrain domain content to the student's description. The response payload states that the prompt and rubric are omitted, while the fidelity review compares the generated representation with the submitted description. These source-level rules support describing the intended workflow; they are not an independent study of generated-model fidelity or student learning.

## Public wording

> Explain explores an emerging approach to formative assessment: turning a student's answer to an ordinary open-ended science question into an interactive model of their stated explanation.

The website identifies the distinctive focus as using the submitted answer itself as the model's source within a teacher-reviewed assessment workflow. It links the four principal related sources and states the review's scope. Claims of worldwide priority, universal preservation of student misconceptions, and measured learning gains are not supported by this review.

## Review scope

Searched public scholarly and product sources for student explanations becoming simulations, student-created models, natural-language educational simulation generation, and simulations based on misconceptions. Reviewed the original paper or institutional record, official tool website, or developers' own descriptions for each source cited above. Did not treat prototype marketing claims as evidence of validated learning outcomes, and did not run the third-party AI generation services.
