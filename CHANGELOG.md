# Changelog

All notable changes to this project are documented in this file.

## [0.2.1] - 2026-08-23

### Fixed

- Selector-based exclusion (`exclude.selectors`) was broken: special regex characters in a selector (e.g. the leading `.` in `.llm-ignore`) were being escaped instead of stripped, so the generated regex could never match against class attributes. Selectors are now sanitised correctly, and selector-based exclusion works as documented. ([#2](https://github.com/velohost/astro-llm/pull/2), thanks [@ttntm](https://github.com/ttntm))

## [0.2.0] - 2026-04-01

### Added

- Support for Astro 6.

## [0.1.0] - 2026-01-08

- Initial release.
