# Topic playbooks

Read only the section that matches the topic. Each gives the usual sticking point, a default sequence, what to do and avoid, and how strong the evidence is. Evidence labels: **Supported** (meta-analyses or trials), **Promising** (some evidence, limited or from other settings), **Heuristic** (expert practice or theory).

Contents:
1. Mathematics and symbolic reasoning
2. Programming and debugging
3. Computer science and algorithms
4. Physics and other technical subjects
5. Abstract theories and philosophical arguments
6. Research papers and academic literature
7. Business, finance and economics
8. Processes, workflows and systems architecture
9. History and narrative material
10. Practical procedures and unfamiliar tools

## 1. Mathematics and symbolic reasoning

**Sticking point:** holding several symbols and intermediate results in mind at once; not seeing why a step is allowed.

**Default sequence:** what the formula or idea is for (one sentence), then a worked example with real numbers, then the general symbolic form, then why each step holds, then conditions and edge cases.

**Do:**
- Name each step of a worked example ("Step 2: substitute u = x²"). Named steps let learners reuse the method.
- Write every non-trivial algebra step on its own line, with the reason beside it.
- Restate what each symbol means when it returns after a gap.
- Use small concrete numbers before symbols for newcomers; drop them for experienced users.
- Give a sanity check: plug in a simple value, or check a limiting case.
- In Practice mode, use faded examples: first fully worked, then with one step blank, then the learner does it all.

**Avoid:** "it follows that" across hidden steps; introducing three new symbols in one sentence; incorrect-example-only practice for novices.

**Evidence:** Worked examples in math g = 0.48, correct examples strongest (Supported). Fading guidance and concreteness fading (Promising).

## 2. Programming and debugging

**Sticking point:** error messages that name the symptom, not the cause; long code where the relevant line is buried.

**Default sequence for an error:** the cause in plain words (first sentence), then the line or construct responsible, then the fix, then the mechanism (why the language does this), then how to recognize this error next time.

**Do:**
- Quote only the relevant lines. Show a minimal reproducible example when the user's code is long.
- Show the fix as a small diff or the changed lines, not a rewritten file, unless they asked for the full file.
- Explain how to read this error message: which part of the traceback points at the cause.
- When explaining a concept, use a tiny runnable snippet and say what it prints.
- Flag anything the snippet leaves out that real code needs (error handling, input validation, concurrency, security).
- If the user is learning, let them apply the fix or predict the output before you show it; if they need it working now, just fix it.

**Avoid:** dumping a full implementation; changing unrelated code; "simplified" code that silently fails on real input.

**Evidence:** Subgoal-labeled worked examples improved novice programming (Promising). Enhanced error messages: mixed results, one classroom study found no learning benefit, which is a reason to teach how to read the message, not only to replace it (Promising). Unrestricted AI answers can reduce later unassisted performance; scaffolding when the goal is learning (Supported, from math).

## 3. Computer science and algorithms

**Sticking point:** the abstract description does not connect to what the algorithm actually does step by step.

**Default sequence:** the problem it solves, then a trace on a tiny input (4 to 6 elements) with the state shown after each step, then the key idea (often an invariant: what stays true each step), then correctness, then complexity, then edge cases.

**Do:**
- Show state tables or ASCII sketches of the data structure after each step.
- State the invariant in one sentence; it is usually the real explanation.
- Derive complexity from the trace ("each pass halves the range, so about log₂ n passes").
- Contrast with the naive approach so the idea's purpose is visible.

**Avoid:** pseudocode without a trace; big-O stated without the reason.

**Evidence:** Worked examples and step-level tracing follow worked-example and segmenting research (Supported in general, Heuristic for this application).

## 4. Physics and other technical subjects

**Sticking point:** equations learned as symbol manipulation without a physical picture; misconceptions from everyday intuition.

**Default sequence:** the physical situation in words (what is happening, what you would see), then the governing relation, then a worked numeric example with units, then checks (units, limiting cases, sign), then where the model stops applying.

**Do:**
- Name the misconception directly if one is common ("Heavier objects don't fall faster in a vacuum; here is why it feels like they do").
- Carry units through every line of a calculation.
- Check limits: what happens as mass goes to zero or time to infinity.
- State the idealizations (frictionless, point mass, small angle).

**Avoid:** analogies that carry over wrong features (current as water works for flow; it misleads about what happens in a broken circuit, so say so).

**Evidence:** Refutation texts for misconceptions g = 0.41, 0.28 bias-adjusted (Supported). Interactive engagement beats passive lecture in physics, and students may feel they learned less while learning more (Supported).

## 5. Abstract theories and philosophical arguments

**Sticking point:** losing the structure of an argument in long prose; mixing the author's view with objections.

**Default sequence:** the thesis in one sentence, then the argument as numbered premises leading to the conclusion, then a concrete case that shows what is at stake, then the strongest objection and the best reply, then what is still disputed.

**Do:**
- Present the argument as a numbered premise list; mark which premise is doing the work.
- Separate what the thinker claims from how it is usually interpreted and from your assessment.
- Use one concrete thought experiment or case; abstract theory becomes graspable through what it implies.
- Keep the field's terms of art, each defined once.

**Avoid:** caricatures to make a view easy to reject; presenting one school's reading as settled.

**Evidence:** Argument mapping for critical thinking (Promising, small studies). Concrete cases before abstraction (Promising).

## 6. Research papers and academic literature

Use Research mode. Additional moves:

- First give the one-sentence takeaway and whether the evidence supports it.
- Translate the design into plain terms: who was studied, what was compared, what was measured.
- Report effect sizes or absolute differences, not only "significant".
- Name the population and setting, and whether the result should generalize beyond them.
- Separate the authors' claims, the data and your evaluation, and say which is which.
- For a long paper, go section by section only if asked; otherwise follow a three-pass logic: the gist (claim, contribution, whether it is credible), then figures and main evidence, then assumptions and weak points.

**Evidence:** The three-pass method is an expert heuristic, not tested (Heuristic). Claim, evidence, limitation separation reflects standard critical appraisal (Heuristic).

## 7. Business, finance and economics

**Sticking point:** jargon hides a simple relationship; models depend on assumptions nobody states.

**Default sequence:** the relationship in plain words ("higher rates make borrowing costlier, so spending falls"), then one worked example with round numbers, then the mechanism and what drives what, then the assumptions and where the model fails, then what this means for the decision at hand.

**Do:**
- Use one small, consistent set of numbers through the whole example.
- Distinguish accounting definitions from economic concepts when they share a name (profit, cost, capital).
- State the assumptions behind any model or rule of thumb.
- For a personal financial or legal decision, give the information needed to decide and note that you are not a financial or legal adviser.

**Avoid:** formula dumps without a worked number; presenting contested economics as settled.

**Evidence:** Worked examples and concrete-first sequencing transfer from math research (Promising); little direct research for this domain.

## 8. Processes, workflows and systems architecture

**Sticking point:** many components at once overload working memory; the interactions matter more than the parts.

**Default sequence:** what the system is for, then the components, each with a one-line role, then one request traced end to end through them, then what happens when something fails, then trade-offs and alternatives.

**Do:**
- Name the components before describing interactions (learning the parts first helps).
- Trace one concrete request with numbered hops.
- Draw a simple diagram when the interface supports it.
- Explain each component by structure (what it is), behavior (what it does) and function (why it is there).
- Cover failure modes; they reveal why the design is the way it is.

**Avoid:** listing every component of a large system at once; abstract box descriptions with no traced example.

**Evidence:** Pre-training on component names, median d = 0.85 (Supported, narrated-animation settings). Structure-behavior-function framing (Heuristic).

## 9. History and narrative material

**Sticking point:** lists of dates and names without the causal thread.

**Default sequence:** the central question or conflict, then the key actors and what each wanted, then the causal chain (this happened because of that), then the turning point and outcome, then how historians disagree, if they do.

**Do:**
- Organize around a question or conflict, not a timeline.
- Make every causal link explicit ("because", "which led to").
- Use dates only as anchors; a few, placed where they matter.
- Separate well-established facts from interpretation and debate.

**Avoid:** colorful anecdotes that are not part of the causal story; presenting one interpretation as the only one.

**Evidence:** Causal story structure improves comprehension and recall (Promising). Irrelevant interesting details lower learning (Supported).

## 10. Practical procedures and unfamiliar tools

**Sticking point:** reading long instructions before acting; not knowing what success looks like or what to do when a step fails.

**Default sequence:** what they will have at the end (one sentence), then numbered steps: one action each, with what they should see after, and a recovery line at error-prone steps.

**Do:**
- Start acting by step 1; put background after the steps or skip it.
- Tie steps to the user's real task, not a generic demo.
- Add "If you see X instead, do Y" at the steps where things commonly go wrong.
- Group long procedures into stages of 3 to 7 steps, each with a checkpoint.
- Use the exact labels the tool shows (button names, menu names) when you know them; say when you are unsure because interfaces change.

**Avoid:** conceptual explanation before the first action; steps that combine several actions.

**Evidence:** Minimalist, action-first instruction beat standard manuals in usability studies (Promising, older studies). Separating each instruction is W3C cognitive-accessibility guidance (Heuristic).
