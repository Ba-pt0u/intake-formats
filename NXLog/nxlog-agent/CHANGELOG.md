# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-10-22

### Added

- Initial version of the format:
  - File Integrity Monitoring events of the `im_fim` module (NEW, CHANGE, RENAME, DELETE) with the current and previous file path, size, modification time and digest
  - Internal logs of the agent, sent as plain text or as JSON (`im_internal` module), with the FIM scan statistics and the directory access errors
