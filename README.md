# Content Repurposer

Turn ideas, drafts, work stories, and long notes into social posts, threads, or replies while preserving the facts and your chosen voice.

This skill separates the task, writing style, and destination. It helps an agent adapt your material without inventing your experience or forcing every idea into the same template.

## Modes

| Mode | Use it to |
|---|---|
| Refine | Improve an existing draft while preserving its intent |
| Develop | Build an undeveloped idea into a connected argument |
| Counter | Respond to a specific claim with evidence and a useful alternative |
| Angles | Explore different approaches before choosing one |
| Story | Shape a real supplied experience into a useful lesson |
| Translate | Explain technical work to the intended audience |
| Extract | Find useful insights in one long supplied source |

Styles are operator, educator, and contrarian. Platform guides cover LinkedIn, X, and Threads. These are drafting preferences, not promises about algorithmic reach or engagement.

## Install

Copy the repository into a skill directory supported by your agent, under `content-repurposer`. For hosts using a user-level `~/.agents/skills` directory:

```sh
git clone https://github.com/pvaskas/content-repurposer.git ~/.agents/skills/content-repurposer
```

Use an empty destination and avoid duplicate installations under the same name. Keep the mode, style, platform, and voice resources together.

## Example requests

```text
Use $content-repurposer to refine this LinkedIn draft.
Keep my argument and uncertainty. Use a direct, conversational voice.
Do not invent examples or results: [paste draft].
```

```text
Use $content-repurposer to give me three angles from these notes.
The audience is operations managers. Show the angles before drafting:
[paste notes].
```

```text
Use $content-repurposer in TRANSLATE mode for the explanation below.
Explain the mechanism to a non-technical owner and retain the trade-off.
Do not claim time savings unless the source supports them: [paste explanation].
```

## Set your voice

Supply approved writing samples or preferences for audience, language, formality, humor, directness, formatting, and words to avoid. Without samples, the skill uses neutral plain-language defaults rather than claiming to reproduce your personal voice.

`voice.md` contains those defaults. `examples.md` starts empty. Persistent changes to the voice or example corpus require your instruction; drafts are not automatically added to a public repository or shared skill.

For finding ideas across a collection of recent work, use the optional companion `work-to-content`: https://github.com/pvaskas/work-to-content. This skill also works independently with supplied material.

## Boundaries and requirements

No API key or connector is required to work on supplied text. Browsing is useful when a factual claim needs verification, but missing access must be disclosed rather than hidden behind invented sources.

Private client details, credentials, personal examples, and another writer's identity are not included in the package. Runtime source material may still be sensitive: anonymize it and review the final copy. Requests to draft do not authorize publishing, scheduling, messaging, or sending source text to another service.

Writing quality depends on the source and the host model. The skill does not promise audience growth, detector outcomes, or authenticity through fabricated personal details.

## Files

- `SKILL.md`: workflow, task routing, and evidence rules.
- `voice.md`: configurable voice guidance and neutral defaults.
- `modes/`: seven task workflows.
- `styles/`: three writing approaches.
- `platforms/`: destination-specific drafting guidance.
- `examples.md`: an empty, opt-in approved-example corpus.
- `agents/openai.yaml`: display metadata.

## Author and license

Paulius Vaskas · [GitHub](https://github.com/pvaskas)

Released under the [MIT License](LICENSE), permitting use, modification, and redistribution subject to its terms.
