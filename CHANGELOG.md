# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

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
