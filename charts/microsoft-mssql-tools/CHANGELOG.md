# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
[markdownlint](https://dlaa.me/markdownlint/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.3.0] - 2022-06-10

### Added in 2.3.0

- `main.containerSecurityContext.enabled`
- `main.containerSecurityContext.runAsNonRoot`
- `main.containerSecurityContext.runAsUser`
- `main.customStartupProbe`
- `main.schedulerName`
- `main.startupProbe`

### Changed in 2.3.0

- In `poddisruptionbudget.yaml`: `labels`, `matchLabels`
- In `role.yaml`: `labels`
- In `rolebinding.yaml`: `labels`, `name`
- In `service-account.yaml`: `name`
- Update to template
- `main.image.pullPolicy` default value
- `main.podsecurityContext.enabled` default value
- `rbacEnabled` to `rbac.enabled`
- `serviceAccount.create` to `serviceAccount.enabled`

### Removed in 2.3.0

- `ingress`
- `main.containerSecurityContext.privileged`
- `main.podSecurityContext.runAsGroup`
- `main.podSecurityContext.runAsUser`
- `service`
- configmap.yaml
- tls-secret.yaml

## [2.2.0] - 2021-12-17

### Removed in 2.2.0

- Deleted clusterrolebinding.yaml

## [2.1.0] - 2021-11-19

### Added in 2.1.0

- Added support for PodDisruptionBudget

## [2.0.0] - 2021-11-15

### Changed in 2.0.0

- Migrated to new structure in [template](https://github.com/Senzing/charts/tree/main/template)

## [1.0.0] - yyyy-mm-dd

### Added in 1.0.0

1. Initial public version
