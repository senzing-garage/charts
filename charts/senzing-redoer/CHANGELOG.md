# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
[markdownlint](https://dlaa.me/markdownlint/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.4.2] - 2022-07-29

### Changed in 2.4.2

- Added support for `main.senzing.awsAccessKeyId`
- Added support for `main.senzing.awsDefaultRegion`
- Added support for `main.senzing.awsMetadataServiceNumAttempts`
- Added support for `main.senzing.awsMetadataServiceTimeout`
- Added support for `main.senzing.awsSecretAccessKey`
- Added support for `main.senzing.awsSessionToken`
- Rename `senzing.azureConnectionString` to `senzing.azureQueueConnectionString`

## [2.4.1] - 2022-06-30

### Changed in 2.4.1

- Added support for `main.senzing.licenseStringBase64`

## [2.4.0] - 2022-06-10

### Added in 2.4.0

- `main.containerSecurityContext.enabled`
- `main.containerSecurityContext.runAsNonRoot`
- `main.containerSecurityContext.runAsUser`
- `main.customStartupProbe`
- `main.schedulerName`
- `main.startupProbe`

### Changed in 2.4.0

- In `horizontalpodscaler.yaml`: `labels`
- In `poddisruptionbudget.yaml`: `labels`, `matchLabels`
- In `role.yaml`: `labels`
- In `rolebinding.yaml`: `labels`, `name`
- In `service-account.yaml`: `name`
- Update to template
- `main.image.pullPolicy` default value
- `main.podsecurityContext.enabled` default value
- `rbacEnabled` to `rbac.enabled`
- `serviceAccount.create` to `serviceAccount.enabled`

### Removed in 2.4.0

- `ingress`
- `main.containerSecurityContext.privileged`
- `main.podSecurityContext.runAsGroup`
- `main.podSecurityContext.runAsUser`
- `service`
- configmap.yaml
- ingress.yaml

## [2.3.0] - 2022-05-09

### Changed in 2.3.0

1. Support for senzingdata v3.0.0

## [2.2.1] - 2022-03-02

### Changed in 2.2.1

- Updated to senzing-common 1.0.2

## [2.2.0] - 2021-12-17

### Removed in 2.2.0

- Deleted clusterrolebinding.yaml

## [2.1.0] - 2021-11-19

### Added in 2.1.0

- Added support for PodDisruptionBudget

## [2.0.0] - 2021-11-15

### Changed in 2.0.0

- Migrated to new structure in [template](https://github.com/Senzing/charts/tree/main/template)

## [1.3.0] - 2021-09-22

### Added in 1.3.0

1. Add support for:
   - `senzing.azureConnectionString`
   - `senzing.azureFailureConnectionString`
   - `senzing.azureFailureQueueName`
   - `senzing.azureInfoConnectionString`
   - `senzing.azureInfoQueueName`
   - `senzing.azureQueueName`
   - `senzing.mountOptMicrosoft`

## [1.2.0] - 2021-05-05

### Changed in 1.2.0

1. Support for senzingdata v2.0.0

## [1.0.4] - 2021-04-19

### Added in 1.0.4

1. Fixed label indentation errors

## [1.0.3] - 2020-10-16

### Added in 1.0.3

1. Added annotations

## [1.0.2] - 2020-03-24

### Added in 1.0.2

1. Added support for the following environment variables:
    1. `SENZING_CONFIG_PATH`
    1. `SENZING_KAFKA_BOOTSTRAP_SERVER`
    1. `SENZING_KAFKA_FAILURE_BOOTSTRAP_SERVER`
    1. `SENZING_KAFKA_FAILURE_TOPIC`
    1. `SENZING_KAFKA_INFO_BOOTSTRAP_SERVER`
    1. `SENZING_KAFKA_INFO_TOPIC`
    1. `SENZING_KAFKA_REDO_GROUP`
    1. `SENZING_KAFKA_REDO_BOOTSTRAP_SERVER`
    1. `SENZING_KAFKA_REDO_TOPIC`
    1. `SENZING_RABBITMQ_DELIVERY_MODE`
    1. `SENZING_RABBITMQ_FAILURE_HOST`
    1. `SENZING_RABBITMQ_FAILURE_PASSWORD`
    1. `SENZING_RABBITMQ_FAILURE_QUEUE`
    1. `SENZING_RABBITMQ_FAILURE_USERNAME`
    1. `SENZING_RABBITMQ_HOST`
    1. `SENZING_RABBITMQ_INFO_HOST`
    1. `SENZING_RABBITMQ_INFO_PASSWORD`
    1. `SENZING_RABBITMQ_INFO_QUEUE`
    1. `SENZING_RABBITMQ_INFO_USERNAME`
    1. `SENZING_RABBITMQ_PASSWORD`
    1. `SENZING_RABBITMQ_PREFETCH_COUNT`
    1. `SENZING_RABBITMQ_REDO_HOST`
    1. `SENZING_RABBITMQ_REDO_PASSWORD`
    1. `SENZING_RABBITMQ_REDO_QUEUE`
    1. `SENZING_RABBITMQ_REDO_USERNAME`
    1. `SENZING_RABBITMQ_USERNAME`

## [1.0.1] - 2020-02-07

### Added in 1.0.1

1. Added `serviceAccountName`

## [1.0.0] - 2020-01-23

1. Initial chart
