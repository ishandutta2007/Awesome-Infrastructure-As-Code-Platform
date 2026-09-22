# Awesome-Infrastructure-As-Code-Platform

## Top Infrastructure as Code (IaC) Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Terraform/OpenTofu Automation, Drift Detection, Policy as Code, Collaboration & Multi-IaC Orchestration*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Infrastructure as Code (IaC) management**. These systems orchestrate Terraform, OpenTofu, Pulumi, CloudFormation, and related tools—providing remote state, CI/CD runs, policy enforcement, drift detection, and team collaboration (sometimes called TACOS: Terraform Automation and Collaboration Software).



**Examples** include Terraform Cloud (HCP Terraform), Spacelift, env0, Scalr, Pulumi Cloud, Harness, Atlantis, Brainboard, Firefly, StackGen, Digger, Cloudify, Massdriver, Terramate, and CloudFormation StackSets (the category leaders).



**Open-source emphasis**: IaC has a very strong open-source foundation. **OpenTofu**, **Terraform CLI**, **Atlantis**, **Digger**, **Terragrunt**, **Pulumi**, and **Crossplane** enable full automation without commercial control planes. SaaS platforms add governance, scale, and support. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Terraform Cloud / HCP Terraform](https://www.hashicorp.com/products/terraform)**  

  HashiCorp’s managed platform for Terraform runs, remote state, policy as code, and team collaboration at scale.



- **[Spacelift](https://spacelift.io/)**  

  Multi-IaC automation platform supporting Terraform, OpenTofu, Pulumi, CloudFormation, Kubernetes, and Ansible with strong policy and drift features.



- **[env0](https://www.env0.com/)**  

  IaC automation platform for Terraform, OpenTofu, Pulumi, and more—focused on self-service environments, governance, and cost visibility.



- **[Scalr](https://scalr.com/)**  

  Terraform/OpenTofu automation platform with remote state, OPA policies, drift detection, and flexible run-based pricing.



- **[Pulumi Cloud](https://www.pulumi.com/)**  

  Managed platform for Pulumi IaC—state, deployments, policy, and collaboration for infrastructure defined in general-purpose languages.



- **[Harness IaC Management](https://www.harness.io/)**  

  Infrastructure-as-code capabilities within the Harness platform for pipelines, governance, and multi-cloud automation.



- **[Atlantis (hosted / enterprise support options)](https://www.runatlantis.io/)**  

  Open-source Terraform pull-request automation; commercial hosting and support available from ecosystem providers.



- **[Brainboard](https://www.brainboard.co/)**  

  Visual infrastructure design and IaC generation platform aimed at collaborative cloud architecture and Terraform workflows.



- **[Firefly](https://www.firefly.ai/)**  

  Cloud asset management and IaC platform focused on inventory, drift, and codifying existing cloud resources.



- **[StackGen / AI IaC generators](https://www.stackgen.com/)**  

  Platforms that generate and manage infrastructure code with AI assistance and governance controls.



- **[Digger (cloud / commercial options)](https://digger.dev/)**  

  Open-source IaC orchestration that runs in your CI; commercial offerings available for teams that want managed experience.



- **[Cloudify](https://cloudify.co/)**  

  Environment and IaC orchestration platform for multi-cloud and hybrid infrastructure automation.



- **[Massdriver](https://www.massdriver.cloud/)**  

  Platform engineering-oriented IaC and cloud operations product for standardized, self-service infrastructure.



- **[Terramate Cloud](https://terramate.io/)**  

  Automation and orchestration layer for Terraform/OpenTofu stacks, with cloud collaboration features.



- **[AWS CloudFormation StackSets](https://aws.amazon.com/cloudformation/)**  

  Native AWS capability for deploying and managing CloudFormation stacks across accounts and regions at scale.



## Open-Source GitHub Projects

- **[OpenTofu](https://github.com/opentofu/opentofu)**  

  Open-source, community-driven fork of Terraform under a truly open license—drop-in compatible IaC engine for multi-cloud infrastructure.



- **[Terraform (CLI / core)](https://github.com/hashicorp/terraform)**  

  The original IaC engine (note: BSL licensing for recent versions); still widely used with OpenTofu as an open alternative.



- **[Atlantis](https://github.com/runatlantis/atlantis)**  

  Open-source Terraform/OpenTofu pull-request automation that runs plans and applies from GitHub/GitLab/Bitbucket comments.



- **[Digger](https://github.com/diggerhq/digger)**  

  Open-source IaC management that orchestrates Terraform/OpenTofu in your own CI—collaboration, concurrency, and policy without a separate control plane.



- **[Terragrunt](https://github.com/gruntwork-io/terragrunt)**  

  Thin wrapper that keeps Terraform/OpenTofu configurations DRY and helps scale modules, backends, and environments.



- **[Pulumi](https://github.com/pulumi/pulumi)**  

  Open-source IaC SDK for defining infrastructure in Python, TypeScript, Go, .NET, Java, and YAML.



- **[Crossplane](https://github.com/crossplane/crossplane)**  

  CNCF open-source control plane that turns Kubernetes into a universal orchestration layer for cloud infrastructure.



- **[Terramate](https://github.com/terramate-io/terramate)**  

  Open-source tool for orchestrating and generating Terraform/OpenTofu stacks at scale.



- **[Open Policy Agent (OPA) / Conftest](https://github.com/open-policy-agent/opa)**  

  Policy-as-code engine widely used to enforce security and compliance rules on IaC plans.



- **[tfsec / Checkov / Trivy IaC scanners](https://github.com/)**  

  Open-source static analysis tools that scan Terraform, CloudFormation, and Kubernetes manifests for misconfigurations.



### Additional Strong Open-Source Options

- Preferring **OpenTofu + Atlantis or Digger** for a fully open automation pipeline.

- Using **Terragrunt** or **Terramate** to scale module usage across many environments.

- Adopting **Pulumi** or **Crossplane** when general-purpose languages or Kubernetes-native control planes are preferred.

- Combining open IaC engines with commercial TACOS platforms when advanced governance and support are required.

- Accepting that multi-tenant RBAC, audit, cost estimation, and enterprise support still favor commercial platforms (Terraform Cloud, Spacelift, env0, Scalr, Pulumi Cloud, etc.).

- Focusing open-source efforts on license freedom, data sovereignty, and CI-native orchestration.



**Frameworks for building custom systems**: Write modules in OpenTofu/Terraform or Pulumi → orchestrate with Atlantis or Digger in CI → enforce policy with OPA → detect drift with scheduled plans → store state in secure remote backends. Suitable for most platform teams. Large enterprises often add a commercial control plane for governance while keeping open engines underneath.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- IaC systems control production infrastructure. Misconfiguration can cause outages or security exposure. Open-source deployments require secure state storage, least-privilege credentials, and reviewed apply processes. This list is not operational or security advice.



---

**Made for platform engineers, DevOps, and SREs automating cloud infrastructure.**

Let's keep infrastructure code collaborative, governed, and as open as practical.
