# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.1.0] - 2026-10-20

### Added

- Parse new custom fields of Kerberos service ticket events (4769) added by recent Windows Server updates:
  - `action.properties.RequestTicketHash` and `action.properties.ResponseTicketHash`
  - `action.properties.AccountSupportedEncryptionTypes`, `action.properties.ServiceSupportedEncryptionTypes`, `action.properties.DCSupportedEncryptionTypes` and `action.properties.ClientAdvertizedEncryptionTypes`
  - `action.properties.AccountAvailableKeys`, `action.properties.ServiceAvailableKeys` and `action.properties.DCAvailableKeys`
  - `action.properties.SessionKeyEncryptionType`
- Set `action.name` for Microsoft Defender events 1151 and 5007 and for AppLocker events (8002 to 8007, 8020 to 8025)
- Parse `file.name` and `file.path` for AppLocker audit and blocked events (8003, 8004, 8006, 8007)
- Add 27 smart descriptions (group membership, account and computer changes, account lockout, scheduled tasks, audit policy, AD objects, certificate services, NPS, service installation, Microsoft Defender, Sysmon process tampering)

## [1.0.4] - 2026-10-20

### Changed

- Extend parsing of existing custom fields:
  - `action.properties.Path` from PowerShell event message payloads when top-level `Path` is absent or empty

## [1.0.3] - 2026-09-30

### Added

- Parse new custom fields:
  - `action.properties.DnsHostName` for computer account change events
  - `action.properties.PasswordLastSet` for account-management events

## [1.0.2] - 2026-09-10

### Added

- Parse new custom fields:
  - `action.properties.ImpersonationLevel` for Windows 4624 events (`An account was successfully logged on`)

## [1.0.1] - 2024-02-29

### Add

- Parse new ECS fields:
  - `registry.path`
