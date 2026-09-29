# Changelog

All notable changes to this project are documented in this file.
The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and the project uses [Semantic Versioning](https://semver.org/):

- **Major:** restructuring that changes how the playbook is used, or the operating protocol's output format.
- **Minor:** new sections, blueprints, snippets or model profiles.
- **Patch:** corrections, clarifications and re-verification against updated documentation.

## [1.0.0] - 2026-09-29

### Added
- Operating protocol that lets Claude act as a prompt architect, with defaults, a question policy and a fixed output format.
- Core principles, prompt anatomy and a master template.
- Surface profiles for the Claude app, Claude Design, Claude Code, the Claude API, agents, Claude in Chrome, Claude for Microsoft 365 and Claude Tag.
- Model capability matrix and prompting notes for Claude Fable 5.1 / Mythos 5.1, Opus 5.5, Sonnet 5.5 and Haiku 4.5, with notes for Opus 5, Sonnet 5 and the 4.x generation.
- 20 task blueprints and 35 snippet modules.
- Table of outdated techniques and their replacements.
- Quality gate, testing guide, four worked examples and a quick reference card.
- Sources and validation log.

### Verified
- Model identifiers, thinking modes, effort defaults and levels, output limits, and parameter restrictions against Anthropic's Thinking and Effort documentation.
- Claude Code features against *Best practices for Claude Code*.
- Claude Design workflow against the Claude Help Center.
- All snippets marked **(tested)** match Anthropic's published wording.

### Known gaps
- Structured-output support by model was not re-verified for this release.
