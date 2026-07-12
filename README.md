# Homelab Catalog

This repository serves as the central, reusable catalog of "building blocks" for the Kubernetes platform. It stores the definitions, Helm charts, and raw YAML manifests for all platform services and applications that can be deployed.

## Key Features

- **Reusable Components**: Contains battle-tested, versioned definitions for infrastructure services like ingress controllers, monitoring stacks (Prometheus/Grafana), logging, and databases.
- **Multi-Environment Ready**: Manifests are designed to be parameterized, allowing the same component to be deployed across different environments (development, staging, production) with distinct configurations.
- **Source of Truth**: Acts as the single source of truth for component libraries, promoting consistency across all clusters in the homelab ecosystem.

## Structure

- **`/platform`**: Contains definitions for core infrastructure services (e.g., HAProxy Ingress).
- **`/apps`**: Contains definitions for example applications or internal workloads.

## Technologies

- **Helm/Kustomize**: Manifests are structured to work seamlessly with Helm charts or Kustomize for flexible customization.
- **YAML**: Standard resource definitions are written in YAML to be consumed by GitOps tools.

This repository acts as the **catalog layer**, decoupling the "what to deploy" (the definition) from the "where and how to deploy" (the GitOps orchestration).
