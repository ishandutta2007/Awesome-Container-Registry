# Awesome-Container-Registry

# Top Container Registry Platforms Ecosystem
**Curated List of SaaS Products & Open-Source GitHub Projects**
*Focused on OCI Image Storage, Vulnerability Scanning, Replication, RBAC, Helm/OCI Artifacts & Private Registries*
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Container Registries**. These systems store, distribute, scan, and govern container images and OCI artifacts for development, CI/CD, and production Kubernetes environments.

**Examples** include Docker Hub, GitHub Container Registry, GitLab Container Registry, Harbor, Amazon ECR, Google Artifact Registry, Azure Container Registry, JFrog Artifactory, Quay.io, and Nexus Repository (the category leaders).

**Open-source emphasis**: Container registries have excellent open-source options. **Harbor** (CNCF graduated), **Distribution** (OCI registry), **Zot**, and related projects enable fully self-hosted, secure private registries. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms
- **[Docker Hub](https://hub.docker.com/)**  
  The largest public container registry—default for many developers, with official images, automated builds, and private repositories.

- **[GitHub Container Registry](https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry)**  
  GitHub’s integrated OCI registry tightly coupled with repositories, Actions, and package permissions.

- **[GitLab Container Registry](https://docs.gitlab.com/ee/user/packages/container_registry/)**  
  Built-in registry for GitLab projects—CI/CD native push/pull and integrated with GitLab security features.

- **[Harbor](https://goharbor.io/)**  
  CNCF graduated open-source registry with commercial support options—scanning, signing, replication, and RBAC (also widely self-hosted).

- **[Amazon ECR](https://aws.amazon.com/ecr/)**  
  AWS-managed container registry with IAM integration, image scanning, and tight coupling to ECS/EKS/Fargate.

- **[Google Artifact Registry](https://cloud.google.com/artifact-registry)**  
  GCP’s unified artifact registry for containers and other package formats with IAM and regional control.

- **[Azure Container Registry](https://azure.microsoft.com/en-us/products/container-registry/)**  
  Azure-managed registry with geo-replication, security integrations, and AKS-friendly workflows.

- **[JFrog Artifactory](https://jfrog.com/artifactory/)**  
  Universal artifact repository supporting Docker/OCI along with many other package types and deep DevOps integration.

- **[Quay.io](https://quay.io/)**  
  Red Hat’s hosted container registry with strong security focus, Clair-based scanning, and access controls.

- **[Nexus Repository](https://www.sonatype.com/products/sonatype-nexus-repository)**  
  Sonatype’s repository manager with Docker/OCI support alongside Maven, npm, and other formats (OSS and Pro editions).

## Open-Source GitHub Projects
- **[Harbor](https://github.com/goharbor/harbor)**  
  Leading CNCF graduated open-source cloud-native registry—stores, signs, and scans images; RBAC, replication, and vulnerability scanning.

- **[Distribution (Docker Registry / OCI)](https://github.com/distribution/distribution)**  
  Core open-source OCI Distribution Specification implementation—foundation for many registries including Docker Hub components and Harbor.

- **[Zot Registry](https://github.com/project-zot/zot)**  
  Lightweight, OCI-native open-source registry focused on simplicity, security, and modern distribution features.

- **[Nexus Repository OSS](https://github.com/sonatype/nexus-public)**  
  Open-source edition of Nexus Repository Manager with Docker and multi-format artifact support.

- **[Quay (Project Quay)](https://github.com/quay/quay)**  
  Open-source container registry codebase underlying Quay.io, with security and multi-tenancy features.

- **[Docker Registry UI / community frontends](https://github.com/)**  
  Open web UIs and management interfaces for self-hosted Distribution-based registries.

- **[Kraken / dragonfly-style P2P distribution](https://github.com/)**  
  Open projects for large-scale, efficient image distribution across clusters.

- **[cosign + registry integration](https://github.com/sigstore/cosign)**  
  Open signing and verification workflows commonly paired with Harbor and other OCI registries.

- **[Clair](https://github.com/quay/clair)**  
  Open-source vulnerability scanner frequently integrated with Quay, Harbor, and other registries.

- **[Documentation and Harbor / Distribution playbooks](https://goharbor.io/docs/)**  
  Guides for deploying, securing, and operating self-hosted container registries.

### Additional Strong Open-Source Options
- Self-hosting **Harbor** for enterprise-grade private registry with scanning and RBAC.
- Running plain **Distribution** for simple, lightweight private registries.
- Using **Zot** when a minimal OCI-native registry is preferred.
- Combining open registries with **Trivy/Clair** scanning and **cosign** signing.
- Accepting that fully managed multi-region, zero-ops cloud registries and deep vendor IAM integration still favor SaaS options (ECR, Artifact Registry, ACR, Docker Hub, GHCR, etc.).
- Focusing open-source efforts on data sovereignty, air-gapped environments, and cost control at scale.

**Frameworks for building custom systems**: Deploy Harbor or Distribution on Kubernetes → enable scanning and retention policies → replicate to edge/regional registries → sign images with cosign → enforce pulls via admission controllers. Suitable for platform teams and regulated environments. Many organizations still use cloud-managed registries for simplicity.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- Container registries store critical build artifacts. Secure access control, scanning, and backups are essential for any self-hosted deployment. This list is not security advice.

---
**Made for platform engineers, DevOps teams, and open-source registry advocates.**
Let's keep images trusted, distributed efficiently, and registries as open as practical.
