# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.0.0] - 2026-10-22

### Added

- Initial version of the format:
  - incident reports sent by CybelAngel, parsed as alerts
  - audit logs of the platform: logins, logouts and actions of the users on the incident reports, the keywords and the users
  - ECS fields are used whenever possible (`event.*`, `server.*`, `host.name`, `threat.software.name`, `tags`, `related.*`, `user.*`)
