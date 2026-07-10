---
name: google-tech-writing
description: Draft, restructure, rewrite, and review technical documents using a token-efficient adaptation of Google's Technical Writing course. Use for documentation created from scratch or edits to API docs, tutorials, how-to guides, conceptual guides, design documents, reference pages, READMEs, troubleshooting content, and documents containing sample code, tables, or diagrams; also use for clarity, audience-fit, organization, style, and usability reviews.
---

# Google Technical Writing

Distilled writing guidance from Google's technical writing course at https://developers.google.com/tech-writing/overview

Prioritize clarity over every other writing rule. Preserve technical meaning, obey the project's style guide when one exists, and never invent facts to make prose smoother.

## Establish the reader contract

Before drafting or reviewing, determine the following:

- **Audience:** Identify readers' roles and proximity to the subject.
- **Goal:** State why readers opened the document.
- **Starting point:** Record what readers already know and any prerequisites.
- **Outcome:** State what readers should know or be able to do afterward.
- **Scope:** State what the document covers.
- **Non-scope:** State what readers might expect but the document excludes.

Infer low-risk details from the request or source material. Ask only when missing context would materially change the document. For a review, flag contradictions between the stated reader contract and the actual content.

## Draft from scratch

1. Write the reader contract.
2. List the tasks readers must perform or the points they must learn. Order prerequisites before dependent material.
3. Build an outline with one concept or task per entry. Prefer task-based headings that readers will recognize.
4. Explain why a task matters before giving its steps. Alternate concepts with practical application when useful.
5. Open with the scope, audience, prerequisites, exclusions, and essential takeaway. Revise the opening after finishing the draft.
6. Draft one topic per paragraph and one idea per sentence.
7. Add lists, tables, code, and figures only when they make information easier to use.
8. Disclose information progressively: start simple, introduce a concept near its first use, and move optional depth later or link to it.
9. Run the review workflow before delivering the draft.

Choose shorter interconnected pages for novice how-to guides, overviews, and conceptual introductions. Consider longer pages for narrative tutorials, in-depth guidance, and searchable reference material. Break up even a long page when readers need distinct entry points.

## Review an existing document

Review from large concerns to small ones:

1. Verify technical claims, procedures, code, links, and examples when evidence is available. Mark unverifiable claims; do not silently guess.
2. Check whether the audience, goal, prerequisites, scope, and outcome are explicit and aligned.
3. Check the outline, information order, headings, navigation, and progressive disclosure.
4. Check each paragraph, sentence, term, list, table, figure, and sample against the rules below.
5. Remove repetition, detours, marketing language, and details that do not help satisfy the scope.
6. Read difficult passages aloud or simulate doing so. Fix awkward phrasing and sentences that exceed a comfortable breath.

When asked for a critique, lead with the highest-impact findings. Identify the affected passage, explain the reader impact, and propose a concrete revision. Separate correctness problems from style preferences. When asked to edit, preserve the author's meaning and terminology unless a change improves accuracy or consistency; surface unresolved questions after the revision.

## Apply the core rules

### Fit words to the audience

- Define or link unfamiliar terms at first use. Use a glossary when many definitions accumulate.
- Use one term for one concept. Introduce a short form explicitly before using it.
- Define an unfamiliar acronym on first use as **Full Term** (**FT**), then use one form consistently. Create an acronym only when it is substantially shorter and appears often.
- Prefer simple, culturally neutral English. Avoid idioms, obscure words, insider references, and unexplained team abbreviations.
- Address the reader as **you**, not **we**.
- Format code-related text as code according to the project's conventions.
- Replace subjective promotion with evidence. Prefer “reduces latency by 40%” to “blazingly fast.”

### Make sentences direct

- Prefer active voice and name the actor: “Python interprets code.” Use passive voice sparingly, and never let it hide an actor the reader needs.
- Choose precise verbs. Replace `is`, `occur`, and `happen` when a stronger verb improves meaning.
- Replace `there is` or `there are` with a real subject and action.
- Put conditions before instructions: “If the build fails, rerun the command.”
- Express one main idea per sentence. Split branches into separate sentences.
- Convert embedded or complicated alternatives into lists.
- Delete filler: replace “is able to” with “can” and “provides a description of” with “describes.”
- Keep pronouns close to unmistakable antecedents. Repeat the noun when another noun intervenes or the reference is distant. Follow `this` or `that` with a noun when ambiguity is possible.
- In US English, use `that` for essential clauses and `which` with a preceding comma for nonessential clauses.

### Build focused paragraphs

- Make the opening sentence state the paragraph's central point.
- Keep every sentence on that topic; move or delete digressions.
- Answer **what**, **why**, and **how** when readers need all three.
- Aim for roughly three to five sentences. Consider splitting paragraphs longer than seven sentences and combining repeated one-sentence paragraphs.

### Use lists and tables deliberately

- Use bullets for unordered items and numbers for ordered steps.
- Start procedural steps with parallel imperative verbs: “Download,” “Configure,” “Start.”
- Keep items parallel in grammar, logical category, capitalization, and punctuation.
- Introduce every list or table with a contextual sentence ending in a colon.
- Capitalize each item. End complete sentences with sentence punctuation.
- Give every table column a meaningful header. Keep each column internally parallel, avoid cells longer than two sentences, and consider narrow screens.

### Organize for scanning and action

- Put essential conclusions and key points at the beginning.
- Compare new ideas with concepts the audience already understands.
- Use headings that describe reader tasks, not unfamiliar tools or implementation details.
- Put orienting text between a parent heading and its first child heading.
- Provide useful navigation: introductions, summaries, a logical heading hierarchy, a table of contents for long material, related links, and next steps.
- Break walls of text and long procedures into meaningful sections, lists, tables, or diagrams. Do not fragment material merely for visual variety.

### Use punctuation for clarity

- Use the serial comma in embedded lists, but prefer displayed lists for complex items.
- Put a comma between a leading condition and its consequence.
- Do not join independent sentences with only a comma. Use a period, or use a semicolon only when both complete sentences are closely related.
- End a sentence that introduces a list or table with a colon.
- Use em dashes and parentheses sparingly. Avoid en dashes under Google style. Verify compound-word hyphenation against the chosen style guide or dictionary.

## Handle technical assets

### Sample code

- Test code and ensure it builds, performs the stated task, follows language conventions, avoids vulnerabilities, and represents the recommended approach.
- Prefer a short, complete, educational sample over production noise or a repurposed unit test. Never sacrifice correctness merely to shorten it.
- Use descriptive names and straightforward control flow. Avoid clever tricks and deep nesting.
- Comment non-obvious decisions. Explain **why** for experienced readers; avoid narrating obvious syntax.
- Put long conceptual explanations before the code. Keep comments that users need after copying inside the code.
- State dependencies, setup, run instructions, expected output, and meaningful side effects.
- Show an anti-example when a common mistake is otherwise hard to recognize.
- Sequence a sample set from simple to moderate to complex.

### Figures and screenshots

- Write a brief caption first; make it state the takeaway and focus attention. Place it after the figure.
- Limit one figure to roughly one paragraph or five bullets of information.
- Show a simple overview before separate subsystem details.
- Use callouts, cropping, or highlighting to direct attention without clutter.
- Check label readability, contrast, and scaling. Prefer SVG for diagrams when practical.
- Revise figures as rigorously as prose; split any figure that carries multiple messages.

## Use compact examples

Use these patterns as demonstrations, not as copy-and-paste boilerplate. Adapt names, tone, and detail to the reader contract.

### Terms and acronyms

Define a short form before switching names:

> **Protocol Buffers** (**protobufs**) provide a definition language. Protobufs encode structured data.

Do not alternate unexplained synonyms; readers may assume that each name represents a different concept.

Define an acronym only when it recurs enough to repay the learning cost:

> This guide introduces the **Telekinetic Tactile Network** (**TTN**). Use TTN to send tactile events.

### Ambiguous pronouns

Ambiguous:

> Python is interpreted, while C++ is compiled. It has many users.

Clear:

> Python is interpreted, while C++ is compiled. Python has many users.

Ambiguous:

> Running the process configures permissions and creates a user ID. This lets users authenticate.

Clear, depending on the intended meaning:

> This user ID lets users authenticate.

### Active voice and strong verbs

| Weak or indirect | Direct |
| --- | --- |
| Code is interpreted by Python. | Python interprets code. |
| The exception occurs when dividing by zero. | Dividing by zero raises the exception. |
| There is a `met_trick` variable that stores accuracy. | The `met_trick` variable stores accuracy. |
| The design provides a description of Frambus. | The design describes Frambus. |

### One idea per sentence

Crowded:

> IBM introduced Fortran in 1957 and John McCarthy introduced Lisp the following year, which gave programmers iterative and recursive approaches.

Focused:

> IBM introduced Fortran in 1957. John McCarthy introduced Lisp the following year. These languages gave programmers iterative and recursive approaches.

### Lists

Replace an embedded set of capabilities with a parallel list:

> The API supports the following operations:
>
> - Create and query llamas.
> - Analyze alpacas.
> - Delete vicunas.
> - Track dromedaries.

Use imperatives for an ordered procedure:

1. Download the Frambus app.
2. Configure the app.
3. Start the app.

### Paragraphs

Use the opening sentence to announce the topic, then answer what, why, and how:

> The `garp()` function measures the difference between a dataset's mean and median. Extreme values can distort a mean. Call `garp()` to check for that distortion; a small result suggests that the mean represents the dataset more reliably.

### Reader contract and introduction

Use a compact introduction such as the following:

> This guide explains how to publish Markdown files with Froobus. It is for readers who know Markdown and can run basic Linux commands. It covers publishing and verification, but not Froobus installation or administration. After completing the guide, you can publish a file and confirm its public URL.

For a design document, state knowledge outcomes rather than user tasks:

> After reading this design, engineers can explain why Zylmon replaces Zyljeune, identify the migration risks, and evaluate the proposed rollout.

### Task-based headings

Prefer a reader goal:

> ## Create the site

Avoid naming an unfamiliar implementation detail:

> ## Run the `carambola` command

Add context before a child heading:

```markdown
## Create the site

Run the `carambola` command to create and configure the site.

### Set configuration values
```

### Conditions before instructions

Preferred:

> If the program runs slowly, use the `--perf` flag.

Less scannable:

> Use the `--perf` flag if the program runs slowly.

### Code example and anti-example

Show both forms when a small syntax difference causes a common failure:

```bash
# Valid: Bash assignments contain no spaces around =.
s="The rain in Maine."
```

```bash
# Invalid: Bash interprets the spaces as command separators.
s = "The rain in Maine."
```

Accompany a runnable sample with setup, the command to run, expected output, and any side effects. Test the sample rather than assuming that a short snippet still works.

## Finish the work

Adopt the project's style guide. Recheck the document from the reader's perspective, then read it aloud, revisit it after a break when possible, and request a peer review for important material. Treat samples and documentation as maintained artifacts.
