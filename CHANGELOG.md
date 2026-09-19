# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2026-09-19

### Added
- Configurable PDF export font sizes: `exports.pdf.font_size` (summary paragraphs), `exports.pdf.table_font_size` (activities table header and body), and `exports.pdf.heading_font_size` (report title). All default to their previous hardcoded values (12/12/24pt).
- Configurable default PDF page orientation via `exports.pdf.orientation`, now defaulting to `landscape` (previously hardcoded to `portrait` unless overridden per-request via `options.orientation`).

## [1.0.0] - 2026-09-18

### Changed
- Renamed the package to `wg-vn/laravel-activitylog-ui`.
- Replaced `maatwebsite/excel` and `barryvdh/laravel-dompdf` with `paperdoc-dev/paperdoc-lib` for Excel and PDF exports, removing those optional dependencies.
- Moved the documentation into the repository as `DOCUMENTATION.md`.

### Added
- GitHub Actions workflow to publish releases to Packagist on tag push.
