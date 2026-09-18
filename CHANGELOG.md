# Changelog

All notable changes to this template are documented here. The format is based on
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added

- `tools/validate_template.py`: standard-library structural validator for the
  core files, internal Markdown links and anchors, fenced blocks, tables, and the
  uninitialized checkpoint/report state. Makes the review notes' "PASS - N
  structural checks" claim reproducible.
- `.github/workflows/validate.yml`: CI that runs the validator on pushes to
  `main` and on pull requests.
- `LICENSE`: MIT license (update the copyright holder before reuse).
- `CLAUDE.md` and `.claude/commands/setup.md` + `.claude/commands/loop.md`: a thin
  Claude Code adapter and slash commands that wrap the canonical README prompts.
- `CHANGELOG.md`: this file.
- README note pointing to the maintainer tooling above.

### Changed

- Renamed space-containing paths for portability: `prompt log/` → `prompt-log/`
  and the prompt files within it (`guiding-advise-prompt.txt`,
  `modification-prompt.txt`, `starter-prompt.txt`); updated references in
  `README.md` and `docs/TEMPLATE_REVIEW.md`.
