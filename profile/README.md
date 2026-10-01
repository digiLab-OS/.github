<div align="center">

<img width="128" height="128" src="../assets/icons/digiLab-OS.svg" alt="digiLab-OS logo" />

# digiLab-OS

### digiLab's framework for building and integrating uncertainty-aware AI systems.

</div>

## Architecture

<div align="center">
<img width="256" src="../assets/diagrams/dependencies.svg" alt="Dependencies diagram" />
</div>

## Core

| Repository                                 | Status                                                                                                                                        | Description                                                        |
| ------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| [Core](https://github.com/digiLab-OS/Core) | [![CI](https://github.com/digiLab-OS/Core/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/Core/actions/workflows/ci.yaml) | Shared interfaces, errors, validators and data models definitions. |

## Composition

| Repository                               | Status                                                                                                                                      | Description                            |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- |
| [API](https://github.com/digiLab-OS/API) | [![CI](https://github.com/digiLab-OS/API/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/API/actions/workflows/ci.yaml) | Adapter composition and digiLab-OS API |

## SDKs

| Adapter                                              | Status                                                                                                                                                  | Description                                                    |
| ---------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------- |
| [PythonSDK](https://github.com/digiLab-OS/PythonSDK) | [![CI](https://github.com/digiLab-OS/PythonSDK/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/PythonSDK/actions/workflows/ci.yaml) | Python client library for interacting with the digiLab-OS API. |

## Adapters

### Authentication

| Adapter                                                                     | Status                                                                                                                                                                                              | Description                                                                             |
| --------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| [OIDC](https://github.com/digiLab-OS/AuthenticationAdapter-OIDC)            | [![CI](https://github.com/digiLab-OS/AuthenticationAdapter-OIDC/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/AuthenticationAdapter-OIDC/actions/workflows/ci.yaml)           | Authentication adapter for verifying user credentials using OpenID Connect.             |
| [Local JSON](https://github.com/digiLab-OS/AuthenticationAdapter-LocalJson) | [![CI](https://github.com/digiLab-OS/AuthenticationAdapter-LocalJson/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/AuthenticationAdapter-LocalJson/actions/workflows/ci.yaml) | Authentication adapter for verifying user credentials using a local JSON configuration. |

### Authorization

| Adapter                                                                      | Status                                                                                                                                                                                              | Description                                                              |
| ---------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| [Local Cedar](https://github.com/digiLab-OS/AuthorizationAdapter-LocalCedar) | [![CI](https://github.com/digiLab-OS/AuthorizationAdapter-LocalCedar/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/AuthorizationAdapter-LocalCedar/actions/workflows/ci.yaml) | Authorization adapter for enforcing access control policies using Cedar. |

### Ephemeral

| Adapter                                                       | Status                                                                                                                                                                            | Description                           |
| ------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------- |
| [Redis](https://github.com/digiLab-OS/EphemeralAdapter-Redis) | [![CI](https://github.com/digiLab-OS/EphemeralAdapter-Redis/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/EphemeralAdapter-Redis/actions/workflows/ci.yaml) | Redis-backed short-term data storage. |

### Persistence

| Adapter                                                                              | Status                                                                                                                                                                                                    | Description                              |
| ------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| [Local Filesystem](https://github.com/digiLab-OS/PersistenceAdapter-LocalFilesystem) | [![CI](https://github.com/digiLab-OS/PersistenceAdapter-LocalFilesystem/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/PersistenceAdapter-LocalFilesystem/actions/workflows/ci.yaml) | Local filesystem long-term data storage. |

### Execution

| Adapter                                                   | Adapter Status                                                                                                                                                                | Worker Status                                                                                                                                                               | Description                                            |
| --------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| [Ray](https://github.com/digiLab-OS/ExecutionAdapter-Ray) | [![CI](https://github.com/digiLab-OS/ExecutionAdapter-Ray/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/ExecutionAdapter-Ray/actions/workflows/ci.yaml) | [![CI](https://github.com/digiLab-OS/ExecutionWorker-Ray/actions/workflows/ci.yaml/badge.svg)](https://github.com/digiLab-OS/ExecutionWorker-Ray/actions/workflows/ci.yaml) | Execution adapter for distributed computing using Ray. |

### Orchestration

Upcoming
