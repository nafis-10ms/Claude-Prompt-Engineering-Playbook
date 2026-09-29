# Contributing

Thank you for helping keep this playbook accurate. Claude models and products change often, so corrections are the most valuable contributions.

## Ways to contribute

- **Report outdated information.** [Open an issue](../../issues/new?template=outdated-information.md) using the *Outdated information* template.
- **Fix an error.** Open a pull request with the correction and its source.
- **Add material.** New blueprints, snippets or model profiles are welcome when they are backed by documentation or by evaluation results you can describe.

## Standards for changes

1. **Cite a primary source for every factual claim.** Prefer Anthropic's documentation at `platform.claude.com`, `code.claude.com` and `support.claude.com`. Add new sources to Appendix A.1.
2. **Date what you verified.** Update the "Last verified" date only when you re-checked the relevant facts, and record what you checked in Appendix A.2.
3. **Keep tested snippets verbatim.** A snippet marked **(tested)** must match Anthropic's published wording exactly. If you adapt one, remove the **(tested)** label and describe it as adapted.
4. **Label heuristics.** Advice that comes from experience rather than documentation must say so.
5. **Match the existing style.** Plain, direct sentences; placeholders in `{{UPPER_SNAKE_CASE}}`; prompt templates in fenced blocks using four backticks so that nested code fences survive copy-paste.
6. **Keep the protocol stable.** Changes to Section 1 (operating protocol) affect everyone who loads the file into Claude. Explain the reason and the expected effect in the pull request.

## Before you open a pull request

- Check that every internal link and anchor still resolves (GitHub's rendered view is a quick way to confirm).
- Check that every code fence closes, and that templates still render as a single block.
- Update the version number in the playbook header, the footer and the README badge.
- Add an entry to [CHANGELOG.md](CHANGELOG.md).

## Versioning

The project follows [Semantic Versioning](https://semver.org/). See [CHANGELOG.md](CHANGELOG.md) for how major, minor and patch changes are defined.
