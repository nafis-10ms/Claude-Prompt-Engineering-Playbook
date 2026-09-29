<div align="center">

# Claude Prompt Engineering Playbook

**A verified field guide and prompt-architect system for getting production-quality results from every Claude model and product.**

[![Version](https://img.shields.io/badge/version-1.0.0-2f6feb)](CHANGELOG.md)
[![Last verified](https://img.shields.io/badge/last%20verified-2026--09--29-2da44e)](claude-prompt-playbook.md#a2-validation-log)
[![Models](https://img.shields.io/badge/models-Fable%205.1%20%7C%20Opus%205.5%20%7C%20Sonnet%205.5%20%7C%20Haiku%204.5-8250df)](claude-prompt-playbook.md#5-model-profiles)
[![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-lightgrey)](LICENSE)

[Read the playbook](claude-prompt-playbook.md) · [Quick start](#quick-start) · [What's inside](#whats-inside) · [Contributing](CONTRIBUTING.md)

</div>

---

## Overview

Prompting advice for Claude is spread across tutorials, model-specific guides, product help pages and API references, and much of it changes with each model release. This project consolidates it into a single, versioned Markdown file that does two jobs:

- **It turns Claude into a prompt architect.** Load the playbook into any Claude conversation, describe your task, and Claude returns a copy-ready prompt tuned to the product, model and task, with the settings, placeholders, rationale and test cases you need to use it.
- **It works as a reference for people.** Every technique is explained, tied to the specific model where behavior differs, and linked to its source.

It is written for developers, designers and AI product builders who prompt Claude across its products: the Claude app, Claude Design, Claude Code, the Claude API and custom agents.

## Quick start

1. Download [`claude-prompt-playbook.md`](claude-prompt-playbook.md).
2. Load it where you work:

   | Surface | How |
   |---|---|
   | Claude app | Attach the file to a conversation, or add it to a Project's knowledge. |
   | Claude Code | Reference it in a message with `@path/to/claude-prompt-playbook.md`. |
   | Claude API | Include it as reference material in the first user message. |

3. Ask for a prompt:

   ```text
   Using the playbook, craft a prompt for Claude Code to add rate limiting
   to our Express API. Tests must pass.
   ```

Claude responds with its assumptions, the prompt in a copy-ready block, any API settings, the placeholders to fill, why the prompt is built that way, and inputs to test it with. The full request template is in [section 0](claude-prompt-playbook.md#0-quick-start).

## What's inside

| Section | Contents |
|---|---|
| [Operating protocol](claude-prompt-playbook.md#1-operating-protocol-instructions-for-claude) | The procedure Claude follows: defaults, when to ask questions, and a fixed output format |
| [Core principles](claude-prompt-playbook.md#2-core-principles-that-work-on-every-claude-model) | 14 techniques that hold on every Claude model |
| [Prompt anatomy](claude-prompt-playbook.md#3-anatomy-of-a-strong-prompt) | A ten-element structure and a master template |
| [Surface profiles](claude-prompt-playbook.md#4-surface-profiles-where-the-prompt-will-run) | How prompts differ across the Claude app, Claude Design, Claude Code, the API, agents, Chrome, Microsoft 365 and Slack |
| [Model profiles](claude-prompt-playbook.md#5-model-profiles) | API capability matrix, model selection guide, and prompting notes for each model |
| [Task blueprints](claude-prompt-playbook.md#6-task-blueprints) | 20 templates: features, bug fixes, migrations, code review, UI builds, design briefs, product system prompts, extraction, RAG, agents, research, docs, data analysis, vision, subagents, `CLAUDE.md`, `SKILL.md`, eval graders, CI |
| [Snippet library](claude-prompt-playbook.md#7-snippet-library) | 35 drop-in instruction modules, including snippets reproduced verbatim from Anthropic's tested guidance |
| [Outdated techniques](claude-prompt-playbook.md#8-outdated-techniques-and-their-modern-replacements) | Techniques that now cause API errors or poor results, and their replacements |
| [Quality gate](claude-prompt-playbook.md#9-quality-gate) | A pre-delivery checklist and a symptom-to-fix table |
| [Worked examples](claude-prompt-playbook.md#11-worked-examples) | Claude Code feature, product system prompt, Claude Design brief, and a legacy prompt migration |
| [Quick reference](claude-prompt-playbook.md#12-quick-reference-card) | The essentials on one screen |

## Coverage

| | |
|---|---|
| **Models** | Claude Fable 5.1 and Mythos 5.1, Claude Opus 5.5, Claude Sonnet 5.5, Claude Haiku 4.5, with notes for Opus 5, Sonnet 5 and the 4.x generation |
| **Surfaces** | Claude app (chat, long-running tasks, artifacts), Claude Design, Claude Code, Claude API and Console, Agent SDK and custom agents, Claude in Chrome, Claude for Microsoft 365, Claude Tag (Slack) |

## Accuracy and verification

Model behavior and API details change between releases, so every factual claim is dated and sourced.

- **Last verified:** 29 September 2026, against Anthropic's public documentation.
- **What was checked:** model identifiers, thinking modes, effort defaults and levels, output limits, parameter restrictions, Claude Code features and Claude Design workflows. Details are in the [validation log](claude-prompt-playbook.md#a2-validation-log).
- **Tested snippets:** snippets marked **(tested)** are reproduced verbatim from Anthropic's model-specific guides; their measured effects are Anthropic's findings.
- **Known gaps and volatile details** are listed in [A.3](claude-prompt-playbook.md#a3-details-likely-to-change).

Found something out of date? [Open an issue](../../issues/new?template=outdated-information.md) with a link to the current documentation.

## Repository structure

```text
.
├── claude-prompt-playbook.md   # The playbook
├── README.md                   # This page
├── CHANGELOG.md                # Version history
├── CONTRIBUTING.md             # How to propose changes
├── LICENSE                     # CC BY 4.0
└── .github/
    └── ISSUE_TEMPLATE/
        └── outdated-information.md
```

## Contributing

Corrections and additions are welcome, especially when a new model or product release changes recommended practice. Every factual change needs a link to a primary source. See [CONTRIBUTING.md](CONTRIBUTING.md).

## Acknowledgements

This playbook builds on Anthropic's [Prompt Engineering Interactive Tutorial](https://github.com/anthropics/prompt-eng-interactive-tutorial), the [prompt engineering documentation](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/overview) and its model-specific guides, [Best practices for Claude Code](https://code.claude.com/docs/en/best-practices), and the [Claude Design help article](https://support.claude.com/en/articles/14604416-get-started-with-claude-design).

## License and disclaimer

The playbook's original text is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). Excerpts reproduced from Anthropic's documentation remain the property of Anthropic and are included for reference with attribution.

This is an independent community project. It is not affiliated with, endorsed by, or maintained by Anthropic. "Claude" and related product names are trademarks of Anthropic, PBC.
