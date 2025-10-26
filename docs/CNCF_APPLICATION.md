# CNCF Sandbox Application Materials
## DevOps AI Toolkit

**Application Date**: TBD
**Prepared By**: Viktor Farcic (viktor@farcic.com)
**Project Repository**: https://github.com/vfarcic/dot-ai
**Current Version**: 0.118.0 (Beta)

---

## Table of Contents

- [Section 1: Basic Project Information](#section-1-basic-project-information)
- [Section 2: Governance & Community](#section-2-governance--community)
- [Section 3: Cloud Native Context](#section-3-cloud-native-context)
- [Section 4: Legal & Compliance](#section-4-legal--compliance)
- [Section 5: Additional Information](#section-5-additional-information)

---

## Section 1: Basic Project Information

### 1.1 Project Summary (Single Line)

**Question**: Provide a one-line summary of your project.

**Answer**:
AI-powered DevOps automation: infrastructure provisioning, issue remediation, governance management, and project setup through natural language.

---

### 1.2 Project Description (100-300 words)

**Question**: Describe your project in detail. What problem does it solve? How does it work? What makes it unique?

**Answer**:
DevOps AI Toolkit democratizes platform engineering and cloud native operations through AI-powered automation across multiple workflow areas: infrastructure provisioning, issue remediation, governance management, and project setup.

The project addresses critical challenges in modern DevOps:
- **Capability Discovery**: Teams struggle to understand what their Kubernetes clusters can provision (operators, CRDs, native resources)
- **Troubleshooting Complexity**: Diagnosing issues requires deep expertise and multi-step investigation
- **Knowledge Silos**: Platform engineering best practices and governance policies locked in expert engineers' heads
- **Repetitive Toil**: Setting up repositories with proper governance, security, and automation files is manual and inconsistent

**How it works**: Discovers cluster capabilities (resources, operators, CRDs) and uses AI to semantically understand what each resource does. Users describe needs in plain English ("I need a PostgreSQL database"), and the system matches intent to available capabilities, generates manifests, and provisions resources across any infrastructure. It performs multi-step root cause analysis for issues with executable remediation commands, codifies organizational best practices as reusable patterns, and generates 25+ governance/security files for repository standardization.

Built on the Model Context Protocol (MCP), it integrates with any MCP-compatible AI agent and supports multiple AI providers (Claude, GPT, Gemini, Mistral, DeepSeek, XAI).

**What makes it unique**: First project combining semantic capability discovery, MCP integration, and AI-powered automation across infrastructure provisioning, remediation, governance, and project setup. Unlike single-purpose tools like K8sGPT, provides a comprehensive DevOps automation platform working with any infrastructure operators and MCP-compatible agents.

---

### 1.3 Organization Repository URL

**Question**: GitHub organization or user account URL where the project lives.

**Answer**:
https://github.com/vfarcic

---

### 1.4 Project Repository URL

**Question**: Direct link to the project repository.

**Answer**:
https://github.com/vfarcic/dot-ai

---

### 1.5 Additional Repositories

**Question**: List any additional related repositories (optional).

**Answer**:
None currently. The project is consolidated in a single monorepo containing the MCP server, CLI tools, AI integrations, and comprehensive documentation.

---

### 1.6 Website URL

**Question**: Project website URL.

**Answer**:
https://github.com/vfarcic/dot-ai

**Rationale**: Following CNCF Sandbox convention, we use the GitHub repository as the project website. The comprehensive README serves as the homepage, with detailed documentation in the `docs/` directory. This approach is standard for early-stage Sandbox projects and can be upgraded to a dedicated site post-acceptance.

---

### 1.7 Application Contact Emails

**Question**: Primary contacts for this application (who TOC should reach out to).

**Answer**:
- **Primary Contact**: Viktor Farcic (viktor@farcic.com) - Project Creator & Maintainer
- **Secondary Contact**: Same (single maintainer currently)

---

## Section 2: Governance & Community

### 2.1 Roadmap + Context

**Question**: Link to project roadmap and context about project direction.

**Answer**:
https://github.com/vfarcic/dot-ai/blob/main/docs/ROADMAP.md

**Key Roadmap Highlights**:
- **Phase 1 (Current)**: Semantic capability management, MCP integration, core deployment recommendations
- **Phase 2 (6 months)**: Enhanced AI model support (Bedrock, etc.), improved remediation playbooks, web UI
- **Phase 3 (12 months)**: Advanced pattern learning, multi-cluster support, ecosystem integration with more CNCF projects

The roadmap emphasizes building a robust foundation for AI-powered platform engineering while maintaining flexibility to respond to community feedback and cloud native ecosystem evolution.

---

### 2.2 Contributing Guide

**Question**: Link to contribution guidelines.

**Answer**:
https://github.com/vfarcic/dot-ai/blob/main/CONTRIBUTING.md

The contributing guide covers:
- Development environment setup
- Code contribution workflow (fork, branch, PR)
- Coding standards and testing requirements
- Integration test standards and patterns
- Documentation guidelines
- Community communication channels (GitHub Issues, Discussions)

---

### 2.3 Code of Conduct

**Question**: Link to Code of Conduct.

**Answer**:
https://github.com/vfarcic/dot-ai/blob/main/CODE_OF_CONDUCT.md

We've adopted the **Contributor Covenant v2.1**, the industry-standard code of conduct used across CNCF projects. This ensures consistent community expectations and clear enforcement procedures.

---

### 2.4 Adopters File

**Question**: Link to adopters list (optional for Sandbox).

**Answer**:
Not yet created. As an early-stage project (6 months old), we're building initial adoption and will create `ADOPTERS.md` as production users emerge. Current indicators of interest (as of October 2025):
- 151 GitHub stars
- 31 forks
- 8 watchers
- Growing npm download trend

Sandbox acceptance will help us attract and document production adopters more effectively.

---

### 2.5 Maintainers File

**Question**: Link to maintainers file or OWNERS file.

**Answer**:
https://github.com/vfarcic/dot-ai/blob/main/docs/MAINTAINERS.md

**Current Maintainers**:
- Viktor Farcic (GitHub: @vfarcic) - Project Creator, Lead Maintainer

**Maintainer Responsibilities**: Code review, release management, community support, technical direction.

**Future Plans**: As the project matures in Sandbox, we aim to recruit additional maintainers from the community to ensure sustainability and diverse perspectives.

---

### 2.6 Security Policy

**Question**: Link to security policy and vulnerability disclosure process.

**Answer**:
https://github.com/vfarcic/dot-ai/blob/main/SECURITY.md

The security policy includes:
- Supported versions and security update policy
- Vulnerability reporting process (private disclosure via GitHub Security Advisories)
- Expected response times (48 hours acknowledgment, 7 days for assessment)
- Security best practices for deployment
- OpenSSF Scorecard integration for automated security monitoring

---

### 2.7 Standard/Specification

**Question**: Does your project implement or define a standard or specification? If so, provide link and details.

**Answer**:
**No formal specification**, but the project implements:
- **Model Context Protocol (MCP)** specification for AI tool integration (https://modelcontextprotocol.io/)
- **Kubernetes API** standards for cluster interaction
- **OpenAPI 3.0** for REST API endpoints

The project follows cloud native best practices and standards but does not define new specifications. It acts as an implementation layer that bridges AI assistants with Kubernetes infrastructure.

---

### 2.8 Product/Service Separation

**Question**: Describe any commercial products or services built on this project. How is the open source project separated from commercial offerings?

**Answer**:
**DevOps AI Toolkit is 100% open source with no commercial product or service**.

- All code is MIT licensed and publicly available
- No "enterprise" or "pro" versions exist
- No hosted SaaS offering
- No vendor lock-in or proprietary extensions
- No commercial entity backing the project

The project creator (Viktor Farcic) is a Developer Advocate at Upbound and maintains this as an independent open source project separate from any employer. This ensures neutral governance aligned with CNCF principles.

---

## Section 3: Cloud Native Context

### 3.1 Why CNCF?

**Question**: Why are you applying to join CNCF? What do you hope to gain?

**Answer**:
We're applying to CNCF for four strategic reasons:

**1. Natural Ecosystem Fit**
DevOps AI Toolkit is fundamentally a cloud native project built on Kubernetes, integrating with CNCF projects (Kubernetes, Argo CD, Crossplane, Kyverno, Prometheus), and solving cloud native pain points. CNCF is the natural home for projects in the Kubernetes ecosystem.

**2. Neutral Governance & Sustainability**
As a single-maintainer project with growing adoption, we need neutral governance to ensure long-term sustainability. CNCF provides the framework to transition from individual project to community-governed initiative, reducing single-point-of-failure risk.

**3. Community & Visibility**
CNCF membership will significantly increase project visibility within the platform engineering and DevOps communities we serve. Access to CNCF resources (events, marketing, technical guidance) will accelerate community building and contributor recruitment.

**4. Credibility for Adopters**
Enterprise teams hesitate to adopt single-maintainer projects without formal governance. CNCF Sandbox membership signals project viability, governance structure, and community backing thus lowering the adoption barrier for organizations.

**What we hope to gain**:
- Access to CNCF technical advisory groups for guidance on architecture and integrations
- Visibility at KubeCon, CloudNativeCon, and CNCF channels
- Connection to potential contributors and adopters
- Governance best practices and mentorship
- Integration opportunities with other CNCF projects
- Long-term project sustainability beyond single maintainer

---

### 3.2 Landscape Benefit

**Question**: What benefit does your project bring to the Cloud Native Landscape?

**Answer**:
DevOps AI Toolkit fills a critical gap in the cloud native landscape: **AI-powered DevOps automation platform for infrastructure provisioning, remediation, governance, and project setup**.

**Problem It Solves**:
Modern Kubernetes clusters have evolved with sophisticated operators and CRDs that can provision resources inside and outside the cluster, but teams struggle to discover and leverage these capabilities. Platform engineers encode knowledge in operators, but developers don't know what exists or how to use it. Additionally, teams need help with issue diagnosis, governance enforcement, and project standardization. This creates:
- **Knowledge gap**: "What can my cluster do?" is difficult to answer
- **Underutilization**: Teams don't leverage available operators and capabilities
- **Tribal knowledge**: Platform capabilities and best practices locked in expert engineers' heads
- **Slow onboarding**: New team members struggle to discover available resources
- **Manual toil**: Repetitive tasks like project setup, issue diagnosis, and governance enforcement

**Landscape Impact**:
1. **Democratizes Infrastructure Operations**: Makes capability-driven provisioning accessible through natural language, working with any operators on any infrastructure
2. **Increases CNCF Project Adoption**: Helps teams discover and leverage any operators already in their clusters
3. **Bridges AI & Cloud Native**: First project combining Model Context Protocol (MCP) with Kubernetes for conversational DevOps automation
4. **Enables Semantic Discovery**: Introduces vector database-powered semantic search to understand cluster capabilities
5. **Comprehensive Automation**: Covers full DevOps lifecycle from provisioning to remediation to governance

**Unique Position**:
Unlike single-purpose tools (K8sGPT for troubleshooting, Helm for packaging), DevOps AI Toolkit provides a comprehensive AI-powered automation platform covering infrastructure provisioning (any resources inside/outside cluster via any operators), issue remediation, governance management, and project setup. This integrated approach is a net-new category in the landscape.

---

### 3.3 Cloud Native Fit

**Question**: How does your project align with cloud native principles?

**Answer**:
DevOps AI Toolkit embodies core cloud native principles:

**1. Kubernetes-Native**
- Built entirely on Kubernetes APIs for resource and infrastructure management
- Discovers and leverages any Kubernetes operators and CRDs that exist in clusters
- Works with resources inside the cluster (native Kubernetes) and outside (via any operators)
- Follows Kubernetes patterns (declarative configuration, controller-based reconciliation)
- Universal compatibility with any infrastructure operators on any environment (cloud, on-prem, edge)

**2. API-Driven & Extensible**
- Exposes capabilities via RESTful HTTP API and Model Context Protocol
- Extensible through pluggable AI providers (Claude, GPT, Gemini, Mistral, DeepSeek)
- Integrates with external systems (Qdrant vector DB, Kubernetes clusters)
- Container-first: Runs as container or npm package

**3. Declarative & Intent-Based**
- Users declare intent in plain English ("I need a PostgreSQL database")
- System generates appropriate Kubernetes manifests based on discovered capabilities (whatever operators exist)
- Those manifests provision resources wherever capabilities reach (cluster-internal or external infrastructure)
- Supports organizational patterns/policies for declarative governance

**4. Observable & Debuggable**
- Comprehensive logging and error handling
- AI-powered remediation with root cause analysis
- Integration with existing observability tools (Prometheus, Grafana)

**5. Composable & Interoperable**
- Works alongside existing CNCF tools (doesn't replace, enhances)
- MCP protocol enables integration with any AI coding assistant
- Multi-cloud via Kubernetes control plane abstraction

**6. Community-Driven Development**
- Open source (MIT license) with transparent development
- Public roadmap and GitHub-based collaboration
- Comprehensive documentation and contribution guidelines

---

### 3.4 Cloud Native Integration (Complementary Projects)

**Question**: Which CNCF or cloud native projects does your project complement or integrate with?

**Answer**:
DevOps AI Toolkit integrates with and enhances CNCF projects through universal discovery and capability-driven operations. The system works with any operators and resources that exist in your cluster. Common examples include:

**Core Integration - Kubernetes**:
- Primary interface for cluster management
- Discovers and leverages all Kubernetes resource types (native and custom)
- Generates manifests for any discovered resources (Deployments, StatefulSets, Services, operator CRs, etc.)

**GitOps & Continuous Delivery**:
- **Argo CD**: Recommends ArgoCD Applications when detected in cluster
- **Flux**: Can generate Flux-compatible manifests
- Supports GitOps workflows through manifest generation

**Infrastructure Operators (Examples)**:
- **Crossplane**: Discovers Crossplane providers and generates XRs/XRDs when available
- **AWS Controllers for Kubernetes (ACK)**: Leverages ACK operators when available
- **ClusterAPI**: Discovers and uses ClusterAPI resources when available
- **Any infrastructure operators**: Works universally with whatever operators exist in the cluster

**Policy & Security**:
- **Kyverno**: Integrates policy validation into recommendations
- **OPA/Gatekeeper**: Can validate generated manifests against policies
- **Falco**: Integrates security context into remediation recommendations

**Observability**:
- **Prometheus**: Uses metrics for remediation root cause analysis
- **Jaeger/Tempo**: Integrates distributed tracing for debugging

**Service Mesh**:
- **Istio/Linkerd**: Generates service mesh configurations when detected

**Storage & Databases**:
- **Operator Framework**: Discovers and uses database operators (PostgreSQL, MySQL, etc.)
- Recommends StatefulSets with proper PVC configurations

**Build & Registry**:
- **Harbor**: References container registries in deployment recommendations
- **Buildpacks**: Can recommend Cloud Native Buildpacks for image creation

**Key Differentiator**: DevOps AI Toolkit acts as a **universal discovery and automation layer** that works with any CNCF projects and operators through capability-driven discovery. The examples above represent common integrations, but the system adapts to whatever exists in your cluster.

---

### 3.5 Cloud Native Overlap (Competing Projects)

**Question**: Are there any CNCF or cloud native projects that overlap with yours? How do you differentiate?

**Answer**:
**Primary Overlap Area**: AI-powered Kubernetes operations

**Similar Projects**:

**1. K8sGPT (CNCF Sandbox, Dec 2023)**
- **Focus**: Troubleshooting and diagnosis - scans clusters for issues and explains them in plain English
- **Overlap**: Both use AI with Kubernetes
- **Differentiation**:
  - K8sGPT: Single-purpose troubleshooting tool (diagnose existing problems)
  - DevOps AI Toolkit: Comprehensive DevOps automation platform (provisioning, remediation, governance, project setup)
  - K8sGPT: Works with current cluster state to diagnose issues
  - DevOps AI Toolkit: Discovers capabilities (any operators/resources), matches intent, provisions infrastructure anywhere
  - K8sGPT: Explains what's wrong
  - DevOps AI Toolkit: Provides end-to-end automation from provisioning to remediation to governance
  - **Complementary**: Can use both - K8sGPT for diagnosis, DevOps AI Toolkit for comprehensive DevOps automation

**2. HolmesGPT (CNCF Sandbox, Sept 2025)**
- **Focus**: AI troubleshooting with broader data sources (Prometheus, logs)
- **Overlap**: AI-powered root cause analysis
- **Differentiation**:
  - HolmesGPT: Investigation from alerts/incidents
  - DevOps AI Toolkit: Semantic capability discovery + deployment recommendations + remediation
  - **Complementary**: Can integrate HolmesGPT for alert analysis, DevOps AI Toolkit for deployment

**3. Kagent (CNCF Sandbox, May 2025)**
- **Focus**: General-purpose agentic AI framework for Kubernetes
- **Overlap**: AI agents for Kubernetes automation
- **Differentiation**:
  - Kagent: Framework for building custom AI agents
  - DevOps AI Toolkit: Purpose-built solution for platform engineering workflows
  - **Complementary**: Kagent provides framework, we provide specific platform engineering tools

**4. Kubernetes Dashboard (CNCF Graduated)**
- **Focus**: Web-based UI for Kubernetes cluster management
- **Overlap**: Both help discover cluster resources
- **Differentiation**:
  - Kubernetes Dashboard: Manual UI navigation and visualization
  - DevOps AI Toolkit: AI-powered semantic discovery and conversational interface with intent-based provisioning
  - **Complementary**: Dashboard for visual inspection, DevOps AI Toolkit for AI-driven automation

**5. Helm (CNCF Graduated)**
- **Focus**: Package manager for Kubernetes with pre-built charts
- **Overlap**: Both simplify Kubernetes deployments
- **Differentiation**:
  - Helm: Pre-built package manager with standardized charts
  - DevOps AI Toolkit: AI-generated manifests tailored to your cluster's actual discovered capabilities
  - Helm: Users must find and choose appropriate charts
  - DevOps AI Toolkit: Discovers what operators/CRDs exist and generates appropriate manifests dynamically
  - **Complementary**: Helm for packaging applications, DevOps AI Toolkit for capability-driven provisioning

**Key Differentiators That Make DevOps AI Toolkit Unique**:
1. **Semantic Capability Discovery**: Only project using vector search to understand what any cluster resources can do
2. **Universal Compatibility**: Works with any operators on any infrastructure (not prescriptive about specific operators or clouds)
3. **Comprehensive Platform**: Covers full DevOps lifecycle (provisioning, remediation, governance, project setup) vs. single-purpose tools
4. **MCP Protocol Integration**: Native integration with any MCP-compatible AI agents for conversational workflows
5. **Capability-Driven**: Discovers and adapts to whatever exists in your cluster dynamically
6. **Organizational Intelligence**: Codifies institutional knowledge as patterns and policies for consistent operations

**Ecosystem Positioning**: DevOps AI Toolkit is **complementary** to single-purpose tools (K8sGPT for troubleshooting, Helm for packaging) while providing a **comprehensive AI-powered DevOps automation platform** that works universally with any infrastructure operators and any MCP-compatible agents.

---

### 3.6 Similar Projects (Non-CNCF)

**Question**: Are there similar projects outside CNCF? How do you compare?

**Answer**:
**Similar Projects & Comparisons**:

**1. kubectl-ai / Kube-Copilot**
- **Similarity**: AI-assisted kubectl commands
- **Difference**:
  - Limited to generating kubectl commands from natural language
  - DevOps AI Toolkit discovers capabilities, understands operators/CRDs, generates complete manifests
  - We provide organizational governance (patterns/policies) on top of AI

**2. Pulumi/Terraform with AI Assistants**
- **Similarity**: Infrastructure as Code with AI code generation
- **Difference**:
  - IaC tools: Define infrastructure in code
  - DevOps AI Toolkit: Kubernetes-native, leverages existing cluster capabilities, semantic discovery
  - We work with what's already in the cluster rather than defining everything from scratch

**3. Commercial AI DevOps Platforms (Harness AI, GitLab Duo, GitHub Copilot for Azure)**
- **Similarity**: AI for DevOps automation
- **Difference**:
  - Commercial platforms: Closed source, vendor lock-in, SaaS-only
  - DevOps AI Toolkit: 100% open source, self-hosted, MIT licensed, neutral governance
  - Focuses on Kubernetes capability discovery vs. broad DevOps automation

**Unique Value Proposition**:
- **Only open source project** combining semantic capability discovery + vector search + MCP integration for Kubernetes platform engineering
- **Kubernetes-native**: Works with cluster as it exists, not imposing new abstractions
- **AI-powered intent translation**: Converts "what I want" to "how to deploy it with what's available"
- **Governance-aware**: Organizational patterns/policies influence recommendations

**Target Audience Alignment**:
Unlike general-purpose IaC or AI code assistants, DevOps AI Toolkit is purpose-built for platform engineers and DevOps teams working with complex Kubernetes environments who need AI to help bridge the capability discovery gap.

---

### 3.7 Landscape Listing Status

**Question**: Is your project currently listed on the Cloud Native Landscape?

**Answer**:
**Not currently listed.**

We plan to apply for Cloud Native Landscape listing upon Sandbox acceptance, as CNCF projects receive prioritized placement. We recommend being listed under:

**Primary Category**: **Provisioning > Automation & Configuration**
- **Rationale**: DevOps AI Toolkit's core functionality aligns with infrastructure orchestration and deployment automation, which is the focus of this category. The project automates infrastructure provisioning, configuration management, and operational workflows through AI-powered intelligence.

**Secondary Category (if dual listing permitted)**: **CNAI (Cloud Native AI)**
- **Rationale**: As an AI-powered automation toolkit, the project also fits the emerging Cloud Native AI category, demonstrating innovative application of AI technologies to cloud native operations.

**Why Landscape Listing Matters**:
Landscape visibility helps potential adopters discover the project when researching automation solutions and AI-powered Kubernetes tools, reinforcing our position as a cloud native community member while increasing project discoverability across multiple relevant categories.

---

## Section 4: Legal & Compliance

### 4.1 Trademark Donation Agreement

**Question**: Are you willing to donate any project trademarks to CNCF (if applicable)?

**Answer**:
**Yes, willing to transfer any applicable trademarks to CNCF.**

**Current Trademark Status**:
- "DevOps AI Toolkit" is not currently registered as a trademark
- Preliminary trademark search conducted (October 2025) shows no obvious conflicts
- No trademark registration exists for the project name
- Note: A comprehensive trademark clearance search may be recommended before formal registration

**Transfer Agreement**:
If trademarks are registered in the future or if CNCF requests trademark registration, we will follow CNCF trademark transfer procedures per the CNCF Charter and IP Policy.

**Name Flexibility**:
If trademark conflicts arise during the acceptance process, we're open to discussing alternative names to ensure smooth CNCF integration.

---

### 4.2 IP Policy Compliance

**Question**: Does your project comply with CNCF IP Policy? Are all contributions properly licensed?

**Answer**:
**Yes, full compliance with CNCF IP Policy.**

**License Compliance** (verified via `npm audit` and `license-checker`, October 2025):
- **Project License**: MIT License (CNCF-approved, permissive)
- **Primary Dependencies** (378 total packages):
  - MIT: 296 packages (78%) - CNCF allowlist
  - Apache-2.0: 32 packages (8%) - CNCF allowlist
  - ISC: 30 packages (8%) - CNCF allowlist
  - BSD-2-Clause: 10 packages (3%) - CNCF allowlist
  - BSD-3-Clause: 6 packages (2%) - CNCF allowlist
  - Python-2.0: 1 package (0.3%) - CNCF allowlist
  - BlueOak-1.0.0: 3 packages (0.8%) - OSI-approved permissive (not on CNCF allowlist)
  - Unlicense: 1 package (0.3%) - Public domain dedication (not on CNCF allowlist)
- **No GPL or copyleft licenses** in dependency tree
- **No licensing conflicts** detected by npm audit (0 vulnerabilities)

**Contribution Licensing**:
- All contributions are made under MIT license
- Pull Request template includes Developer Certificate of Origin (DCO) sign-off requirement
- Contributors retain copyright, but grant MIT license to use

**Copyright Ownership**:
- Currently: Viktor Farcic (individual contributor)
- Post-acceptance: Open to transferring copyright to CNCF or Linux Foundation as required

**IP Policy Verification**:
- No patents filed or claimed
- No contributor license agreement (CLA) required (DCO-based)
- All code written specifically for this project (no proprietary code included)
- Third-party components clearly identified in package.json with licenses

---

### 4.3 License Exception Needs

**Question**: Do you need any exceptions to the CNCF license policy?

**Answer**:
**Minimal exceptions may be needed for 4 transitive dependencies (1% of total).**

**Non-Allowlist Dependencies** (all permissive, transitive):
1. **BlueOak-1.0.0** (3 packages: jackspeak@4.1.1, package-json-from-dist@1.0.1, path-scurry@2.0.0)
   - Status: OSI-approved permissive license (approved by Open Source Initiative in Jan 2024)
   - Nature: Similar to MIT, explicitly addresses patents
   - Risk: Low - permissive license, widely considered FOSS-compatible

2. **Unlicense** (1 package: stream-buffers@3.0.3)
   - Status: Public domain dedication
   - Nature: Maximum permissiveness (no restrictions)
   - Risk: Low - effectively public domain

**Mitigation Strategy**:
If CNCF requests license alignment, we can identify and replace these 4 transitive dependencies with functionally equivalent packages using CNCF allowlist licenses. Given these are common utility libraries (path handling, argument parsing, stream buffers), allowlist-licensed alternatives are readily available in the npm ecosystem.

**Note**: 97% of dependencies (374 of 378 packages) are on the CNCF allowlist. No GPL, AGPL, or copyleft licenses present.

---

### 4.4 Signatory Information

**Question**: Who will sign legal documents on behalf of the project?

**Answer**:
**Viktor Farcic**
- **Email**: viktor@farcic.com
- **Role**: Project Creator & Lead Maintainer
- **Authority**: As individual copyright holder, authorized to sign all legal documents including trademark transfers, IP agreements, and CNCF membership agreements

**Post-Acceptance Governance**:
As the project matures in Sandbox, we plan to establish a steering committee with multiple maintainers from diverse organizations. At that point, signatory authority would be transferred to the committee or designated CNCF representative per standard CNCF governance models.

---

## Section 5: Additional Information

### 5.1 Domain Technical Review (TAG Engagement)

**Question**: Have you engaged with any CNCF Technical Advisory Groups (TAGs)? Which TAG would be most appropriate to review your application?

**Answer**:
**No formal TAG engagement yet.**

**Primary Recommendation: Platform Working Group**

DevOps AI Toolkit is fundamentally a platform engineering tool that helps teams build internal developer platforms through AI-powered automation. The CNCF Platform Working Group is the most natural fit for review, as the project directly addresses platform engineering challenges: abstracting infrastructure complexity, enabling self-service workflows, codifying organizational patterns, and improving developer experience.

**Alternative TAG Assignments** (if Platform WG is unavailable or TOC prefers TAG review):

Given the project's cross-domain nature, it could fit multiple TAGs depending on review focus:
- **TAG Infrastructure** - Capability discovery and infrastructure provisioning
- **TAG Developer Experience** - Project setup, governance automation, developer workflows
- **TAG Operational Resilience** - AI-powered issue remediation and troubleshooting
- **TAG Security and Compliance** - Policy management and governance enforcement
- **Cloud Native AI Working Group (TAG Runtime)** - AI/LLM-powered automation across all workflows

**Flexibility**:
We're open to TOC assigning any TAG or working group based on their strategic priorities and full application context. The project's cross-cutting nature means it can provide value to multiple technical communities.

**Post-Submission Engagement**:
We're committed to actively participating in assigned TAG/working group meetings, presenting project demos, and incorporating feedback into roadmap priorities.

---

### 5.2 CNCF Contacts

**Question**: Do you have any existing contacts within CNCF (TOC members, ambassadors, project maintainers)?

**Answer**:
**Yes, several CNCF community members with whom I have professional relationships**:

**CNCF TOC & TAB Members**:
- **Ricardo Rocha** - CERN Platform Infrastructure Lead, CNCF TOC member, Chair of End User Technical Advisory Board (TAB), Lead of Research User Group, Co-chair of TAG Runtime, previously Co-Chair of KubeCon + CloudNativeCon

**CNCF Ambassadors**:
- **Abby Bangser** - CNCF Ambassador, co-lead of CNCF Platforms Working Group, Syntasso founding principal engineer
- **Whitney Lee** - CNCF Ambassador, Datadog
- **Saiyam Pathak** - CNCF Ambassador, TAG Operational Resilience Chair (elected 2025), TAG Environmental Sustainability Lead, Kubesimplify founder
- **William Rizzo** - CNCF Ambassador, Mirantis Strategy Lead, TAG nominee for Infrastructure and Workloads Foundation
- **Saim Safdar** - CNCF Ambassador, TAG Developer Experience Chair nominee, Platform Working Group contributor, Cloud Native Islamabad organizer

**TAG Leadership & Nominees**:
- **Mauricio Salatino** - TAG Developer Experience Chair nominee, former Knative Steering Committee member, Diagrid engineer
- **Lian Li** - Former TAG App-Delivery Tech Lead and Co-Chair, Freelance Platform Engineer

**Project Maintainers & Community Contributors**:
- **Dan Garfield** - Argo project maintainer, Chief Open Source Officer at Codefresh/Octopus Deploy
- **Orlin Vasilev** - CNCF community contributor
- **Faisal Afzal** - Cloud native practitioner
- **Graziano Casto** - Platform engineering community member
- **Vlad Mocanu** - DevOps community contributor

**Nature of Relationships**:
These contacts are through professional DevOps community engagement (conferences, meetups, online communities). While I haven't formally discussed this CNCF application with them, they represent potential reviewers or advisors familiar with the platform engineering, developer experience, and operational resilience problem spaces that DevOps AI Toolkit addresses.

---

### 5.3 Additional Information

**Question**: Any additional information you'd like to share with the TOC?

**Answer**:

**Project Maturity & Readiness**:
- **Active Development**: 442 commits in 6 months, regular releases (currently v0.118.0)
- **Production Quality**: Comprehensive integration test suite, CI/CD automation, semantic versioning
- **Documentation**: 12+ detailed guides covering all features, quick start, troubleshooting
- **Community Infrastructure**: Issue/PR templates, automated labeling, stale bot, OpenSSF Scorecard

**Timing & Market Context**:
- **AI DevOps Surge**: Rapid growth in AI-powered DevOps tools; positioning early in CNCF establishes leadership
- **Platform Engineering Movement**: Strong industry momentum toward platform engineering practices; project directly addresses this trend
- **MCP Ecosystem Growth**: Model Context Protocol adoption accelerating; being early CNCF project with MCP integration creates differentiation

**Commitment to CNCF Principles**:
- **Neutral Governance**: Committed to evolving toward multi-organization maintainer base
- **Community First**: Will prioritize community needs over individual/employer interests
- **Ecosystem Collaboration**: Eager to integrate deeply with other CNCF projects (Argo, Crossplane, Kyverno, etc.)
- **Transparency**: Public roadmap, open development, responsive to feedback

**Sandbox as Growth Vehicle**:
We view Sandbox not as an endpoint but as a **foundation for community building**:
- Sandbox visibility will help attract contributors and maintainers
- TAG engagement will guide architecture and integration decisions
- CNCF credibility will lower adoption barriers for enterprise teams
- Goal: Progress to Incubating as community and governance mature

**Challenges We're Transparent About**:
- **Single Maintainer Currently**: Actively working to recruit contributors; Sandbox acceptance will accelerate this
- **Limited Production Evidence**: Early stage with growing adoption; will document adopters as they emerge
- **Rapid AI Evolution**: Committed to evolving with AI/LLM ecosystem while maintaining stability

**Why CNCF Should Accept DevOps AI Toolkit**:
1. **Fills Real Gap**: Addresses underserved "platform engineering enablement" category
2. **Cloud Native DNA**: Built on Kubernetes, integrates with CNCF projects, follows cloud native principles
3. **Innovative Technology**: First to combine semantic discovery + vector search + MCP for Kubernetes
4. **Strong Foundation**: 6 months of active development, comprehensive docs, solid architecture
5. **Growth Trajectory**: Community interest indicators (stars, forks, downloads) show upward momentum
6. **Committed Maintainer**: Track record of open source contribution, DevOps community presence (YouTube channel: DevOps Toolkit, published author)

We're excited about the opportunity to contribute to the CNCF community and help advance cloud native platform engineering practices.

---

### 5.4 Supplementary Details

**Question**: Any supplementary materials or links that support your application?

**Answer**:

**Video Demonstrations**:
- **Primary Demo**: "DevOps AI Toolkit: AI-Powered Application Deployment"
  https://youtu.be/8Yzn-9qQpQI
  (Comprehensive walkthrough of capability discovery and deployment workflow)

**Documentation Assets**:
- **Quick Start Guide**: https://github.com/vfarcic/dot-ai/blob/main/docs/quick-start.md
- **MCP Setup Guide**: https://github.com/vfarcic/dot-ai/blob/main/docs/mcp-setup.md
- **Tools Overview**: https://github.com/vfarcic/dot-ai/blob/main/docs/mcp-tools-overview.md
- **Deployment Guide**: https://github.com/vfarcic/dot-ai/blob/main/docs/mcp-recommendation-guide.md
- **Remediation Guide**: https://github.com/vfarcic/dot-ai/blob/main/docs/mcp-remediate-guide.md

**Technical Architecture**:
- **GitHub Repository**: https://github.com/vfarcic/dot-ai
- **npm Package**: https://www.npmjs.com/package/@vfarcic/dot-ai
- **Release Notes**: https://github.com/vfarcic/dot-ai/releases

**Community Metrics** (as of October 2025):
- 151 GitHub stars
- 31 forks
- 8 watchers
- 442 commits (6 months)
- 0.118.0 version (semantic versioning, frequent releases)
- npm downloads: Growing trend since launch

**Creator Background**:
- **Viktor Farcic**
- **YouTube Channel**: DevOps Toolkit (DevOps education, 50K+ subscribers)
- **Published Author**: Multiple books on Kubernetes and DevOps
- **Roles**: CNCF Ambassador, GitHub Star, Google Developer Expert, CDF Ambassador
- **Current**: Developer Advocate at Upbound (Crossplane, CNCF Graduated project)
- **Community Presence**: Regular speaker at KubeCon, DevOps conferences

**Security & Quality**:
- **OpenSSF Scorecard**: Automated security monitoring enabled
- **Dependency Updates**: Renovate bot for automated dependency management
- **CI/CD**: GitHub Actions for automated testing and releases
- **Code Quality**: TypeScript with strict mode, comprehensive linting, integration tests

**Integration Examples**:
- Model Context Protocol (MCP) server implementation
- Kubernetes API client integration
- Vercel AI SDK for multi-provider AI support (Claude, GPT, Gemini, Mistral, DeepSeek, XAI)
- Qdrant vector database for semantic search
- Support for Crossplane, Argo CD, Kyverno integration

---

## Application Submission Checklist

Before submitting this application, verify:

- [x] All 30 fields completed with accurate information
- [x] All URLs tested and accessible
- [x] Governance documents exist and linked correctly
- [x] Trademark status confirmed (no conflicts)
- [x] License compliance verified (MIT + compatible dependencies)
- [x] Contact information current (viktor@farcic.com)
- [x] Project metrics up to date (stars, forks, commits)
- [x] Differentiation from similar projects clearly articulated
- [x] TOC/TAG reviewer context provided
- [x] Application tone: professional, honest, enthusiastic

---

## Next Steps After Submission

1. **Monitor Application Issue**: Track cncf/sandbox GitHub issue for TOC/TAG comments
2. **Respond Promptly**: Answer any TAG review questions within 48 hours
3. **TAG Engagement**: Attend relevant TAG meetings if invited to present
4. **Community Updates**: Keep community informed via GitHub Discussions
5. **Be Responsive**: Address any feedback or concerns raised during review
6. **Prepare Demo**: Be ready to provide live demo if requested by TOC

---

**Application Prepared By**: Viktor Farcic (viktor@farcic.com)
**Date**: January 2025
**Document Version**: 1.0
