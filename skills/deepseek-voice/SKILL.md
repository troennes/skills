---
name: deepseek-voice
description: Draft, rewrite, edit, and audit content in DeepSeek's institutional technical voice across API documentation, integration guides, conceptual explanations, troubleshooting, pricing or policy pages, and model release announcements. Use when the user asks for DeepSeek voice, DeepSeek Voice DNA, DeepSeek-style writing, or wants content matched to the voice profile derived from DeepSeek writing samples.
---

# DeepSeek Docs Voice

Distilled voice DNA from https://api-docs.deepseek.com/

## Apply the voice

1. Identify the requested operation: draft, rewrite, edit, or audit.
2. Classify the content as documentation or a release announcement. Within documentation, identify API reference, integration tutorial, conceptual guide, troubleshooting, or pricing/policy content.
3. Read [references/voice-dna.md](references/voice-dna.md) completely before writing. Apply the register-specific guidance for the identified content type.
4. Preserve technical facts, commands, code, identifiers, links, dates, and constraints unless the user asks to change them. Treat the Voice DNA as a style source, not a factual source.
5. Lead with the capability, result, or required action. Arrange the remaining information in the shortest reliable sequence for the content type.
6. State conditions, consequences, limitations, and corrective actions explicitly. Distinguish required, recommended, default, and optional behavior.
7. Run the audit checklist in the reference. Revise any line that sounds chatty, vague, inflated, blameful, or mechanically imitative.

## Handle task types

### Draft

- Extract the facts, intended reader, desired outcome, and content type from the request.
- Use placeholders instead of inventing missing technical facts.
- Produce publication-ready copy in the requested format.

### Rewrite or edit

- Preserve the source meaning and technical behavior.
- Preserve code blocks and literal UI or API strings unless correction is explicitly requested.
- Reorganize when needed to improve scan speed, causal order, or proximity of warnings to affected steps.
- Return the finished copy without a change log unless the user requests one.

### Audit

- Identify deviations under tone, structure, precision, reader relationship, emotional register, formatting, and prohibited tendencies.
- Quote only the smallest useful excerpt from the supplied content.
- Recommend concrete revisions and, when useful, provide a corrected version.

## Guardrails

- Capture tone and decision logic; do not merely insert recurring phrases.
- Do not reproduce typos, doubled spaces, translation artifacts, or inconsistent source formatting.
- Do not turn the voice into a parody of technical formality or launch hype.
- Keep emoji and exclamation marks out of routine documentation.
- Anchor promotional claims to a supplied spec, benchmark, availability fact, cost change, limitation, or next step.
- Do not infer current product facts from the voice reference. Verify unstable facts when the task requires factual accuracy.
- Follow the user's requested length, format, and terminology when these differ from the defaults in the Voice DNA.
