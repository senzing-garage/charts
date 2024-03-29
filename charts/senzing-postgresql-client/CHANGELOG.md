# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
[markdownlint](https://dlaa.me/markdownlint/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.2.0] - 2022-06-10

### Added in 2.2.0

- `main.containerSecurityContext.enabled`
- `main.containerSecurityContext.runAsNonRoot`
- `main.containerSecurityContext.runAsUser`
- `main.customStartupProbe`
- `main.schedulerName`
- `main.startupProbe`
- `rbac`
- `serviceAccount`
- role.yaml
- rolebinding.yaml
- service-account.yaml

### Changed in 2.2.0

- In `poddisruptionbudget.yaml`: `labels`, `matchLabels`
- Update to template
- `main.image.pullPolicy` default value
- `main.podsecurityContext.enabled` default value

### Removed in 2.2.0

- `ingress`
- `main.containerSecurityContext.privileged`
- `main.podSecurityContext.runAsGroup`
- `main.podSecurityContext.runAsUser`
- `service`
- configmap.yaml

## [2.1.0] - 2021-11-19

### Added in 2.1.0

- Added support for PodDisruptionBudget

## [2.0.0] - 2021-11-15

### Changed in 2.0.0

- Migrated to new structure in [template](https://github.com/Senzing/charts/tree/main/template)

## [1.0.2] - 2021-06-24

### Changed in 1.0.2

1. Changed to `senzing/postgresql-client`

## [1.0.1] - 2020-10-16

### Added in 1.0.1

1. Added annotations

## [0.3.0] - 2019-09-10

### Added in 0.3.0

1. Migrate to RPM installation.

## [0.2.0] - 2019-06-15

### Added in 0.2.0

1. Initial public version
