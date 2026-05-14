# Changelog

All notable changes to this project will be documented in this file. The format
is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). This
project adheres to [Semantic Versioning](https://semver.org/).

## [Unreleased]

## [0.3.7] - 2026-05-15

### Changed

- Migrated off the deleted `hjkl_engine::step` and `Editor::step_input` — now
  drives the FSM through `hjkl_vim::dispatch_input`. No public API change for
  hjkl-form consumers.
- Bumped `hjkl-engine` dep to `0.7` and `hjkl-vim` dep to `0.19` (Phase 6.6 FSM
  extraction).

## [0.3.6] - 2026-05-13

### Changed

- Bumped `hjkl-engine` dep requirement from `^0.5` to `^0.6` (engine removed the
  transitional `enter_op_*` controller methods; no API impact for hjkl-form).

## [0.3.5] - 2026-05-10

### Changed

- Bumped `hjkl-buffer` dep requirement from `^0.5` to `^0.6` and `hjkl-engine`
  from `^0.4` to `^0.5`.

## [0.3.4] - 2026-05-06

### Changed

- Bumped `hjkl-buffer` dep requirement to `^0.5` and `hjkl-engine` to `^0.4`.

## [0.3.3] - 2026-05-04

### Docs

- Internal CHANGELOG hygiene: backfilled missing release entries and added
  reference link definitions for all version headings. No functional changes.

## [0.3.2] - 2026-05-03

### Docs

- Dropped 0.3.0 milestone callout from the README status section. Per the org's
  "no SPEC frozen claims" stance.

## [0.3.1] - 2026-04-30

### Changed

- Migrated `hjkl-form` from the `kryptic-sh/hjkl` monorepo into its own
  repository ([kryptic-sh/hjkl-form](https://github.com/kryptic-sh/hjkl-form))
  with full git history preserved.
- Relaxed inter-crate dependency requirements from `=0.3.0` to `0.3` (caret),
  matching the standard SemVer pattern for library dependencies.

### Added

- Standalone `LICENSE`, `.gitignore`, and `ci.yml` workflow at the repo root.

[Unreleased]: https://github.com/kryptic-sh/hjkl-form/compare/v0.3.6...HEAD
[0.3.7]: https://github.com/kryptic-sh/hjkl-form/compare/v0.3.6...v0.3.7
[0.3.6]: https://github.com/kryptic-sh/hjkl-form/compare/v0.3.5...v0.3.6
[0.3.5]: https://github.com/kryptic-sh/hjkl-form/compare/v0.3.4...v0.3.5
[0.3.4]: https://github.com/kryptic-sh/hjkl-form/releases/tag/v0.3.4
[0.3.3]: https://github.com/kryptic-sh/hjkl-form/releases/tag/v0.3.3
[0.3.2]: https://github.com/kryptic-sh/hjkl-form/releases/tag/v0.3.2
[0.3.1]: https://github.com/kryptic-sh/hjkl-form/releases/tag/v0.3.1
