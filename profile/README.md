# SS Series: Repository Naming Convention

[한국어 버전 (Korean Version)](./README_KO.md)

## 1. Overview

What does "SS" stand for? While its official name is the **SS Series**, it can mean many things:

- **Super Sexy**: Because good structure is attractive.
- **StarterStack**: A template to kickstart any full-stack project.
- **ScaffoldSuite**: A collection of boilerplates equipped with various features.
- **SpeedySetup**: Emphasizing the ability to set up projects quickly.
- **SmartScaffold**: A template that intelligently lays out your project structure.
- **SuperStructure**: Highlighting a stable and robust architecture.

At its core, the "SS Series" is a systematic repository naming convention for managing Microservice Architecture (MSA) based services. The primary goal is to provide an intuitive and unified structure that allows anyone to understand a repository's domain, service, function, and technology stack at a glance.

## 2. Service Domains

We categorize our services into the following major domains:

*   **Data**: Services related to data collection, processing, and storage.
*   **Authentication/Authorization**: Includes services like the main authentication server and API gateways.
*   **Core Business**: Core services that represent our business logic, such as User, Product, and Order services.
*   **Infra/Ops**: Services for infrastructure and operations, including workers, schedulers, logging, and monitoring.
*   **Common/Util**: Shared libraries and utilities, such as configuration managers and common modules.

## 3. Repository Naming Structure

All repositories in the SS series follow the structure below. Some components are optional but recommended for clarity.

**`ss-<domain>-<service/feature>-<framework>-<language>`**

### Component Breakdown

| Component           | Description                                                                                             | Examples                             |
| ------------------- | ------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| `ss-`               | **Prefix**: Identifies the repository as part of the SS Series.                                         | `ss-`                                |
| `<domain>`          | **Domain**: The broad category of the service.                                                          | `front`, `back`, `data`, `infra`     |
| `<service/feature>` | **Service/Feature**: The name of the microservice and/or its specific feature.                          | `boilerplate`, `auth`, `permission`  |
| `<framework>`       | **Framework**: The primary framework used in the project.                                               | `next`, `spring`, `nest`             |
| `<language>`        | **Language**: (Optional) The primary programming language.                                              | `ts`, `java`, `js`, `go`, `py`       |

### Examples

#### Frontend Boilerplate: `ss-front-boilerplate-next-ts`

*   **Domain**: `front`
*   **Service/Feature**: `boilerplate`
*   **Framework**: `next`
*   **Language**: `ts`

#### Authentication Server: `ss-back-auth-spring-java`

*   **Domain**: `back`
*   **Service/Feature**: `auth`
*   **Framework**: `spring`
*   **Language**: `java`

#### Authorization Service: `ss-back-permission-nest-ts`

*   **Domain**: `back`
*   **Service/Feature**: `permission`
*   **Framework**: `nest`
*   **Language**: `ts`




---
todo: 통합해서 올려주는 repo 만들기 내용 추가 