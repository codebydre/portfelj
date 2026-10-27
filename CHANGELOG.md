# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.5.2] - 2026-10-27

### Changed

- Reduce download size of Homebrew distribution.


## [0.5.1] - 2026-10-27

### Changed

- End year-to-date flex reports on the last weekday, e.g. Friday when downloading over the weekend
- Stop downloading flex reports once IBKR blocks the Flex Web Service token for 24 hours after too many failed attempts (error 1025)
- Retry flex report downloads whenever IBKR asks to try again shortly, with requests spaced 6 seconds apart to stay within IBKR's limit of 10 requests per minute
- Explain expired or invalid tokens and invalid query IDs when downloading flex reports


## [0.5.0] - 2026-10-19

### Added

- Add shell completions via `portfelj completions <SHELL>`, installed by Homebrew, deb, pkg and MSI installers
- Add ability to download flex reports directly from IBKR (e.g: `portfelj flex web-service download 2026`)

### Changed

- Recognize all IBKR order types and the `LF` notes code; unknown order types and notes codes no longer prevent flex reports from loading

### Removed

- Breaking: remove `--xml-dir` parameter from `edavki` and `ledger` CLI commands. Default `flex` folder in the current directory is used instead.


## [0.4.0] - 2026-03-02

### Added

- Add distribution for ARM64 Linux builds

### Changed

- Streamline integration with external data provider services


## [0.3.2] - 2026-03-02

### Changed

- Improve XML parsing performance


## [0.3.1] - 2025-12-28

### Added

- [Windows] Add automatic updates on Windows. Example: `portfelj software-update upgrade`

### Fixed

- [Windows] Fix issues with missing vcruntime140.dll


## [0.3.0] - 2025-12-26

### Added

- EDGAR: add company sector in the output when available
- Add offline cache for tickers and business data for over 12,000 companies trading on the US exchanges
- Add support for dividends (Doh-Div)
- Display "report date" for corporate actions and cash transactions to indicate when corrections take place.
- Add software update check. Example: `portfelj software-update check`

### Changed

- [Linux] Breaking: change deb installation directory from `/usr/local/bin` to `/usr/bin`

### Fixed

- Handle special reverse split involving issue change
- Handle mergers with multiple share distributions


## [0.2.1] - 2025-12-06

### Added

- Add missing transaction codes: automatic exercise (AEx), automatic FX conversion (AFx), margin violation (L)


## [0.2.0] - 2025-07-20

### Added

- Add D-IFI generator
- Add option to override working directory via `-w` or `--working-directory`


## [0.1.0] - 2025-05-18

### Added

- Initial release
