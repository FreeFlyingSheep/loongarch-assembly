# Change Log

All notable changes to the "loongarch-assembly" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [Unreleased]

## [1.0.0] - 2021-08-18

### Added

- Syntax highlighting for LoongArch assembly language.

## [1.1.0] - 2021-09-15

### Added

- Support for comment shortcuts.

## [1.1.1] - 2021-11-24

### Changed

- Fix highlighting for terms like `$r0`.

## [1.1.2] - 2021-11-25

### Changed

- Fix highlighting for comments like `// xxx: xxx`.

## [1.1.3] - 2021-11-26

### Changed

- Change the minimum version of VS Code API that the extension depends on.

## [1.1.4] - 2021-12-02

### Changed

- Fix highlighting for words like `kernelsp`.
- Remove highlighting for registers not beginning with `$`.

## [1.2.0] - 2023-07-06

### Added

- Add highlighting for more escape sequences.
- Add highlighting for FCSR registers.
- Add highlighting for LVZ, LBT, LSX and LASX instructions.
