# Scientific Writer Skill

Scientific Writer is an agent skill for drafting, diagnosing, reviewing, and teaching scientific manuscript writing. It combines section-level rhetorical models with sentence-level clarity audits.

## What It Does

The skill supports four modes:

- **WRITE**: drafts manuscript sections using function-first section scaffolds.
- **REVIEW**: audits scientific prose for clutter, voice, sentence architecture, terminology, and internal numerical/citation consistency.
- **DIAGNOSE**: maps existing manuscript text to expected section components and identifies structural gaps.
- **LEARN**: teaches scientific writing concepts interactively.

## Method Sources

This skill is a synthesized and adapted writing aid based on two sources:

- Hilary Glasman-Deal, *Science Research Writing for Native and Non-Native Speakers of English*. This source informs the SRW/Narrative Wrap section models for Introduction, Methods, Results, Discussion, Conclusion, Abstract, and Title writing.
- `Allan9719/sci_write`, forked from `labarba/sciwrite`, based on Dr. Kristin Sainani's *Writing in the Sciences* methodology. This source informs the 5-pass writing quality audit. The SciWrite repository is licensed under CC BY 4.0.

This repository is not a replacement for either source. It reformulates selected writing principles into operational instructions for an AI assistant.

## License

This project is released under the Creative Commons Attribution 4.0 International License (CC BY 4.0). See `LICENSE`.

## Repository Layout

- `SKILL.md`: main agent-skill instruction file.
- `references/section-models.md`: compact section models and language reference.
- `references/writing-quality.md`: compact writing-quality checks.
- `extracted-models/`: detailed private extraction notes used to build the compact references. Do not include this directory in the public release package.

## Use

Install or copy `SKILL.md` into an AI tool that supports agent skills or persistent custom instructions. Then ask for a specific mode, for example:

```text
Review the writing quality of this Discussion section.
```

```text
Help me draft an Introduction for a paper about [topic]. Build the scaffold first.
```

```text
Diagnose whether this Abstract follows the expected model.
```

## Attribution And Licensing Notes

The 5-pass review component is adapted from SciWrite, which is licensed under CC BY 4.0. Attribute the original SciWrite project when sharing or publishing derivative versions.

The Glasman-Deal material is used here as a methodological inspiration and condensed operational summary. If you publish this repository, avoid distributing long excerpts from the book or files that reproduce the source text too closely. Prefer original examples, paraphrased rules, and links or bibliographic references to the book.

Source links:

- SciWrite fork: https://github.com/Allan9719/sci_write
- Original SciWrite project: https://github.com/labarba/sciwrite
- CC BY 4.0: https://creativecommons.org/licenses/by/4.0/

## Safety Boundaries

The skill improves communication, structure, and clarity. It does not validate experiments, perform statistical analysis, verify citations against databases, or determine whether scientific claims are true. For numerical and citation checks, it only audits internal consistency in the text provided by the user.
