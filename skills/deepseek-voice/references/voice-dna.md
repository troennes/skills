# DeepSeek Docs Voice DNA Reference

## Contents

1. [Core identity](#core-identity)
2. [Register selection](#register-selection)
3. [Documentation register](#documentation-register)
4. [Release register](#release-register)
5. [Reader relationship](#reader-relationship)
6. [Emotional range](#emotional-range)
7. [Sentence and paragraph rhythm](#sentence-and-paragraph-rhythm)
8. [Language patterns](#language-patterns)
9. [Information architecture](#information-architecture)
10. [Formatting](#formatting)
11. [What to avoid](#what-to-avoid)
12. [Content recipes](#content-recipes)
13. [Quality checklist](#quality-checklist)
14. [Calibration examples](#calibration-examples)

## Core identity

Write like a pragmatic engineering organization hosting capable developers: calm, exact, direct, and generous with implementation detail. Make the useful fact or action visible immediately. Project confidence without hiding limits.

The target feeling is:

> You can act on this now, and we have told you the important boundaries.

Preserve these traits across every register:

- **Concrete over abstract:** Name the command, field, model, condition, failure, date, or measured result.
- **Confident but bounded:** Make clear claims and state unsupported behavior, compatibility gaps, costs, deadlines, and known issues plainly.
- **Technically generous:** Supply enough implementation detail for action, including complete examples when missing context could cause errors.
- **Low-ego and institutional:** Prefer `we`, `DeepSeek`, and `you`; avoid a personal `I` voice.
- **Forward-moving:** Make every section advance toward an action, decision, or clearer mental model.
- **Scannable:** Use modular structure and information-dense labels.
- **Respectful:** Treat the reader as capable, provide a recommended default, and preserve meaningful alternatives.

Utility must come before personality. Even promotional writing needs a spec, benchmark, date, endpoint, availability fact, migration action, or constraint close to every major claim.

## Register selection

| Content type | Energy | Stance | Typical structure | Emotional color |
| --- | ---: | --- | --- | --- |
| API reference | Low | Concise authority | Definition → requirements/table/code → result/reference | Neutral confidence |
| Integration tutorial | Low to moderate | Patient implementer | Disclaimer if needed → definition → install → configure → verify/run | Reassuring practicality |
| Troubleshooting/compatibility | Moderate seriousness | Candid expert | Symptom/risk → cause → exact fix → known limit | Controlled caution |
| Conceptual technical guide | Low | Systematic teacher | Mental model → rules → example → interpretation → caveat | Measured precision |
| Pricing/policy | Low | Responsible operator | Units/rules → table → deduction or caveat | Financial caution |
| Release announcement | High | Proud launch announcer | Headline value → capabilities → evidence → access → caveat/resources | Excitement and ambition |

Do not blend registers indiscriminately. A routine API page should not sound like a launch post. An announcement should not read like a compatibility matrix from its first line.

## Documentation register

Set the default levels as follows:

| Trait | Level |
| --- | ---: |
| Technical confidence | 9/10 |
| Clarity/directness | 9/10 |
| Formality | 7/10 |
| Detail | 8/10 when needed |
| Warmth | 4/10 |
| Energy | 3/10 |
| Humor | 1/10 |
| Promotional intensity | 2/10 |
| Transparency about limits | 9/10 |

Open with the capability, governing mental model, observed problem, or required action. Use calm declarative prose. Move quickly into exact commands, values, or rules. End at the successful state, final material caveat, or one focused reference.

Use firm language only when a requirement has a concrete consequence:

> The `reasoning_content` value must be passed back in subsequent tool-call requests. If it is omitted, the API returns an HTTP 400 error.

Avoid vague commands such as “configure it correctly.” Name the field, valid value, and expected result.

### Documentation personality

- Competent rather than showy.
- Pragmatic rather than theoretical.
- Patient without overexplaining basics.
- Candid about beta behavior and known issues.
- Supportive without using generic reassurance.
- Firm when privacy, compatibility, cost, or request validity is at risk.

## Release register

Set the default levels as follows:

| Trait | Level |
| --- | ---: |
| Technical confidence | 9/10 |
| Clarity/directness | 9/10 |
| Formality | 5/10 |
| Detail | 6/10 |
| Warmth | 6/10 |
| Energy | 8/10 |
| Humor | 2/10 |
| Promotional intensity | 7/10 |
| Transparency about limits | 8/10 |

Name the release immediately and put the largest value change in the opening lines. Use compact parallel claims, strong verbs, bold benefit labels, and selective emoji. Pair excitement with evidence.

Allowed emotional colors include pride, ambition, momentum, gratitude, and community responsiveness. Preserve credibility by stating higher token usage, temporary availability, unsupported modes, retirement deadlines, or other tradeoffs as clearly as benefits.

Useful launch logic:

> Announce the release. Isolate the top benefits. Back them with specs or evidence. Give access instructions. End with resources, a deadline, a caveat, or gratitude.

Use words such as `introducing`, `latest`, `enhanced`, `stronger`, `faster`, `efficient`, `stable`, `reliable`, `official`, `open-source`, `world-class`, `available`, and `live` only when the supplied facts support them.

## Reader relationship

Treat the reader as a technically capable peer who may be unfamiliar with this specific system.

- Use **you** for reader actions: install, set, pass, select, verify.
- Use **we** for product support, organizational recommendations, mapping behavior, and company commitments.
- Use **DeepSeek**, **the API**, or the model name when behavior belongs to the system.
- Give a recommended default and explain why when the reason changes the reader's decision.
- Label optional paths without weakening the required path.
- Never scold. Convert mistakes into cause → consequence → correction.

Preferred troubleshooting tone:

> `Authentication Fails` or `401`: Check that the API key is valid and placed in the API key field. Do not enter the API URL in this field.

Avoid:

> You clearly pasted the wrong thing. Fix your key and try again.

## Emotional range

Use composed confidence as the baseline.

Documentation may add:

- reassurance when familiar APIs or existing installations can be reused;
- seriousness when configuration can cause privacy issues, cost, errors, or incompatibility;
- candor when behavior is beta, best-effort, temporary, or incomplete;
- mild enthusiasm when an integration is notably capable or convenient.

Release writing may add strong excitement, competitive pride, gratitude, and future-facing ambition. Do not let excitement erase tradeoffs or turn every feature into a superlative.

## Sentence and paragraph rhythm

1. Use short sentences for actions, outcomes, warnings, and verified rules.
2. Use medium sentences to connect a condition to its consequence.
3. Reserve long sentences for technical distinctions that lose clarity when split.
4. Keep most paragraphs to one to three sentences, each performing one job.
5. Let a short rule interrupt dense explanation when the reader must remember it.
6. Use parallel syntax in lists and announcements: **label + colon + fact or benefit**.
7. Use fragments only in headings, labeled bullets, compact product descriptions, or high-energy announcements.

Statements are the default. Commands are common in procedures. Questions should normally appear only as user examples, quoted interface prompts, FAQ headings, or genuine troubleshooting labels. Avoid rhetorical questions used to manufacture suspense.

## Language patterns

Use these as structural models, not phrase quotas.

### Capability

- “The API supports…”
- “You can use…”
- “This feature allows…”

### Condition

- “If you already have…”
- “When using…”
- “For requests that…”

### Sequence

- “First…”
- “Then…”
- “Next…”
- “After installation…”
- “Once complete…”

### Requirement and reason

- “Set the parameter to…”
- “The value must…”
- “Do not include…”
- “This ensures…”
- “Without this…”
- “To avoid compatibility issues…”

### Consequence and verification

- “The API will return…”
- “The request will…”
- “This counts as…”
- “If the version number is displayed…”
- “If the request succeeds…”

### Caveat, example, and reference

- “Please note that…”
- “However…”
- “The feature works on a best-effort basis…”
- “The following example demonstrates…”
- “In this example…”
- “For more details, refer to…”

### Launch

- “Introducing…”
- “Now live…”
- “Available today…”
- “Try it now…”

Favor concrete verbs:

> use, support, enable, set, pass, return, run, install, configure, select, enter, add, append, map, validate, check, verify, retry, persist, match, switch, update

Favor operational nouns:

> request, response, parameter, field, model, mode, context, configuration, endpoint, output, limit, error, provider, result, usage, support, compatibility

## Information architecture

Use this general sequence for technical content:

1. **What it is:** State the capability or problem in one sentence.
2. **Who or when it applies:** Name the condition, platform, mode, or prerequisite.
3. **What to do:** Give the exact command, field, path, or UI sequence.
4. **What happens:** State the expected output or behavior.
5. **What can go wrong:** Add the important exception, failure mode, or unsupported case.
6. **Where to go next:** Include one relevant reference if needed.

Omit stages that do not help the reader. Stop once the result is reliable.

Keep caveats near the action they constrain. State the condition, consequence, and fix together. Do not collect unrelated warnings at the end merely for convenience.

## Formatting

### Documentation

- Use one descriptive H1.
- Use H2 sections for major concepts or paths.
- Use numbered subheads or numbered lists for sequences.
- Use bullets for options, prerequisites, mappings, or independent facts.
- Use tables for exact mappings, matrices, and comparisons.
- Put commands, paths, parameters, and identifiers in code formatting.
- Provide complete code or configuration when omitted context could cause failure.
- Use **bold** for warning clauses, UI labels, critical requirements, and compact labels—not decoration.
- Avoid italics; the source voice relies on structure and bold labels instead.
- Keep emoji out of technical documentation unless it is literal quoted output.

### Releases

- Use emoji to label sections or bullets, usually no more than one per line.
- Keep sections short and benefit-led.
- Use bold labels followed by a colon and one precise claim.
- Use exclamation marks selectively for launch, availability, or a major price change.
- Combine excitement with links, specs, benchmarks, dates, and constraints.

## What to avoid

- Sarcasm, cynicism, profanity, memes, or insider jokes.
- Personal anecdotes, confessions, lifestyle details, or `I think`/`I feel` framing.
- Rhetorical questions intended only to create engagement.
- Long metaphorical openings or narrative scene-setting.
- Vague reassurance such as “Don't worry, it's super easy.”
- Unbounded promises such as “always perfect.”
- Blaming readers or third parties for errors.
- Excessive hedging around known facts.
- Decorative bold, italics, emoji, or exclamation marks in routine documentation.
- Promotion without a spec, benchmark, availability fact, cost change, or action nearby.
- Repeated overuse of `simply`, `just`, `seamlessly`, or `easy`.
- `must`, `always`, or `never` without a real requirement and consequence.
- Source artifacts such as doubled spaces, inconsistent heading levels, awkward punctuation, or translated grammar errors.
- Generic closings that repeat the introduction, sell again, or invite further chat.

## Content recipes

### API feature page

1. Define the feature and practical outcome.
2. List enablement requirements.
3. Show complete code.
4. Show or describe the output.
5. Add only material caveats.

### Integration guide

1. Add a third-party disclaimer when required.
2. Define the tool in one sentence.
3. Offer a migration path before a clean-install path.
4. Separate OS-specific commands.
5. Add verification and targeted troubleshooting.
6. End at the working state.

### Conceptual guide

1. State the governing mental model.
2. Explain the rules and important distinctions.
3. Show a complete example.
4. Interpret how the example behaves.
5. Close with operational caveats.

### Compatibility warning

1. State the safe configuration.
2. Name the incorrect configuration and exact failure.
3. Explain the underlying requirement.
4. Give the corrected configuration in full.
5. Use bold or a note block to make the warning scannable.

### Pricing or policy page

1. Define the unit or scope.
2. Present exact values in a table.
3. Explain deduction or enforcement rules.
4. State variability, account-level behavior, or review guidance.

### Release announcement

1. Announce the model and largest benefit immediately.
2. Give each model or capability a clear role.
3. Support competitive claims with benchmark or technical evidence.
4. State where it is live and how access changes.
5. Include price, availability, retirement, or temporary-endpoint details.
6. Close with primary resources or brief gratitude.

## Quality checklist

Before returning content, verify:

- Is the capability, result, or required action visible in the opening?
- Can the reader distinguish required, recommended, default, and optional behavior?
- Are exact commands, values, paths, and failure outcomes included where needed?
- Does every warning explain its trigger, consequence, and correction?
- Is the content scannable without losing causal explanation?
- Are limitations stated with the same confidence as benefits?
- Does the emotional energy match the content type?
- Are emoji and exclamation marks confined to genuine announcement content?
- Have source-language artifacts been removed without making the voice chatty?
- Does the ending stop at a result, resource, caveat, deadline, or concise gratitude?
- Are technical facts preserved and unsupported claims excluded?
- Does the draft capture the voice's feeling rather than merely repeat its phrases?

## Calibration examples

### Neutral technical guidance

> A backup only protects your files if it can be restored. Keep one local copy and one copy in a separate location, then restore a small folder to verify that both copies are usable. If the test fails, check the destination permissions and available storage before running the backup again.

### Compatibility warning

> **Important:** Use `anthropic` as the provider type. The `openai` provider does not preserve the required reasoning field across tool-call turns, causing subsequent requests to return an HTTP 400 error.

### Release pattern

> 🚀 **Model X is now live:** Faster long-context processing with the same API format.
>
> 🔹 **Longer context:** Supports up to 1M tokens.
> 🔹 **Lower cost:** Input pricing is reduced by 40%, effective today.
> 🔹 **Same access:** Keep the existing base URL and update the model name to `model-x`.

Treat the release example as structure only. Never reuse its invented facts in real content.
