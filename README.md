# DevOps AI Toolkit

<div align="center">

![DevOps AI Toolkit Logo](assets/images/logo.png)

[![npm version](https://badge.fury.io/js/%40vfarcic%2Fdot-ai.svg)](https://www.npmjs.com/package/@vfarcic/dot-ai)
[![npm downloads](https://img.shields.io/npm/dm/@vfarcic/dot-ai.svg)](https://www.npmjs.com/package/@vfarcic/dot-ai)
[![GitHub release](https://img.shields.io/github/release/vfarcic/dot-ai.svg)](https://github.com/vfarcic/dot-ai/releases/latest)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Project Status](https://img.shields.io/badge/status-beta-orange)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/vfarcic/dot-ai/badge)](https://scorecard.dev/viewer/?uri=github.com/vfarcic/dot-ai)
[![GitHub stars](https://img.shields.io/github/stars/vfarcic/dot-ai.svg?style=social&label=Star)](https://github.com/vfarcic/dot-ai)

</div>

**AI-powered DevOps automation: infrastructure provisioning, issue remediation, governance management, and project setup through natural language.**

📚 [Quick Start](./docs/quick-start.md) | 🔧 [MCP Setup](./docs/mcp-setup.md) | 🛠️ [Features & Tools](./docs/mcp-tools-overview.md)

---

## What is DevOps AI Toolkit?

DevOps AI Toolkit brings AI-powered intelligence to infrastructure provisioning, platform engineering, and development workflows through natural language interaction. Built on the Model Context Protocol (MCP), it provides:

**Infrastructure Provisioning**: Discovers what your cluster can provision (resources inside the cluster and infrastructure outside through any operators) and generates appropriate manifests based on your intent.

**Capability, Pattern, and Policy Management**: Semantically understands what cluster resources do, codifies organizational best practices as reusable patterns, and enforces governance through policies.

**Issue Remediation**: AI-powered root cause analysis with multi-step investigation and executable remediation commands.

**Project Setup**: Generates governance, legal, and security files (LICENSE, CODE_OF_CONDUCT, CONTRIBUTING, SECURITY, GitHub workflows, etc.) for repository standardization.

**Shared Prompts**: Curated prompts accessible as native slash commands in your AI coding assistant.

Works with any infrastructure operators (Crossplane, AWS Controllers, ClusterAPI, database operators, custom operators) and any MCP-compatible AI agent.

## Mission

DevOps AI Toolkit democratizes infrastructure provisioning and platform engineering by making capability-driven operations accessible through AI. We eliminate the expertise barrier that prevents teams from leveraging their cluster's full potential. Whether provisioning cloud resources through operators, deploying applications with native Kubernetes resources, or managing infrastructure across any environment, teams describe what they need in plain English instead of learning operator-specific schemas or memorizing resource types.

## Who Should Use This?

**DevOps AI Toolkit is for teams who want to**:
- Provision infrastructure through Kubernetes operators without learning CRD schemas
- Deploy applications using cluster capabilities discovered automatically
- Manage resources inside the cluster (Deployments, Services) and outside (databases, VMs, storage on any infrastructure)
- Quickly diagnose and fix cluster and infrastructure issues
- Standardize resource provisioning with organizational patterns and policies
- Bootstrap repositories with governance and security files
- Access curated development prompts through native slash commands

## Scope

### In Scope
- Capability-driven resource provisioning (discovers and leverages whatever exists in your cluster)
- Infrastructure provisioning inside cluster (native resources) and outside cluster (via any operators)
- Universal compatibility with any infrastructure operators and any MCP-compatible AI agents
- Intelligent issue remediation and root cause analysis
- Organizational pattern and policy management with semantic search
- Multi-provider AI model support (Claude, GPT, Gemini, Mistral, DeepSeek, XAI)
- Project setup with governance, legal, and security files

### Out of Scope
- Kubernetes cluster provisioning/management (delegates to existing tools)
- CI/CD pipeline execution (provides recommendations only)
- Application runtime monitoring (integrates with existing observability tools)

## Key Features

### 🔍 Capability-Driven Infrastructure Provisioning
Discovers what your cluster can provision: native Kubernetes resources (Deployments, Services, StatefulSets) and infrastructure through any operators (databases, VMs, storage, networks). Works with any operators and any infrastructure (cloud, on-prem, edge). AI understands what each capability actually does, providing intelligent recommendations based on your cluster's actual capabilities.
📖 [Deployment Guide](./docs/mcp-recommendation-guide.md) | [Capability Management](./docs/mcp-capability-management-guide.md)

### 🛠️ Issue Remediation
AI-powered root cause analysis with multi-step investigation, executable remediation commands, and safety mechanisms for manual or automatic execution.
📖 [Learn more →](./docs/mcp-remediate-guide.md)

### 🏛️ Pattern & Policy Management
Capture organizational knowledge and governance policies that automatically enhance AI recommendations with best practices and compliance requirements. Uses vector search for intelligent semantic matching.
📖 [Pattern Management](./docs/pattern-management-guide.md) | [Policy Management](./docs/policy-management-guide.md)

### 📦 Project Setup & Governance
Generate 25+ governance, legal, and automation files (LICENSE, CODE_OF_CONDUCT, CONTRIBUTING, SECURITY, GitHub workflows, Renovate, OpenSSF Scorecard) for repository standardization.
📖 [Learn more →](./docs/mcp-project-setup-guide.md)

### 💬 Shared Prompts Library
Access curated prompts as native slash commands (`/dot-ai:prompt-name`) in your coding agent for consistent workflows across projects.
📖 [Learn more →](./docs/mcp-prompts-guide.md)

### ⚡ Universal AI Integration
Works with any MCP-compatible AI agent via Model Context Protocol. Supports multiple AI providers (Claude, GPT, Gemini, Mistral, DeepSeek, XAI) for flexibility and cost optimization.
📖 [AI Model Configuration](./docs/mcp-setup.md#ai-model-configuration)

## See It In Action

[![DevOps AI Toolkit: AI-Powered Application Deployment](https://img.youtube.com/vi/8Yzn-9qQpQI/maxresdefault.jpg)](https://youtu.be/8Yzn-9qQpQI)

This video explains the platform engineering problem and demonstrates the Kubernetes deployment recommendation workflow from intent to running applications.

## Quick Start

Get started in 3 steps:
1. Configure MCP server (Docker or npm)
2. Connect your AI coding assistant (Claude Code, Cursor, VS Code)
3. Start using conversational workflows

## Documentation

### Getting Started
- **[Quick Start Guide](docs/quick-start.md)** - Get started in minutes
- **[MCP Setup Guide](docs/mcp-setup.md)** - Complete configuration instructions
- **[Tools Overview](docs/mcp-tools-overview.md)** - All available tools and features

### Feature Guides
- **[Resource Provisioning](docs/mcp-recommendation-guide.md)** - AI-powered deployment recommendations
- **[Capability Management](docs/mcp-capability-management-guide.md)** - Semantic resource discovery
- **[Issue Remediation](docs/mcp-remediate-guide.md)** - AI-powered troubleshooting
- **[Pattern Management](docs/pattern-management-guide.md)** - Organizational deployment patterns
- **[Policy Management](docs/policy-management-guide.md)** - Governance and compliance
- **[Project Setup](docs/mcp-project-setup-guide.md)** - Repository governance automation

## Support

- **[Support Guide](SUPPORT.md)** - How to get help and where to ask questions
- **GitHub Issues**: [Bug reports and feature requests](https://github.com/vfarcic/dot-ai/issues)
- **GitHub Discussions**: [Community Q&A and discussions](https://github.com/vfarcic/dot-ai/discussions)
- **Troubleshooting**: See [Troubleshooting Guide](./docs/mcp-setup.md#troubleshooting) for common problems

## Contributing & Governance

We welcome contributions from the community! Please review:

- **[Contributing Guidelines](CONTRIBUTING.md)** - How to contribute code, docs, and ideas
- **[Code of Conduct](CODE_OF_CONDUCT.md)** - Community standards and expectations
- **[Security Policy](SECURITY.md)** - How to report security vulnerabilities
- **[Governance](docs/GOVERNANCE.md)** - Project governance and decision-making
- **[Maintainers](docs/MAINTAINERS.md)** - Current project maintainers
- **[Roadmap](docs/ROADMAP.md)** - Project direction and priorities

## License

MIT License - see [LICENSE](LICENSE) file for details.

## Acknowledgments

DevOps AI Toolkit is built on:
- [Model Context Protocol](https://modelcontextprotocol.io/) for AI integration framework
- [Vercel AI SDK](https://sdk.vercel.ai/) for unified AI provider interface
- [Kubernetes](https://kubernetes.io/) for the cloud native foundation
- [CNCF](https://www.cncf.io/) for the cloud native ecosystem

---

**DevOps AI Toolkit** - Making cloud native operations accessible through AI-powered intelligence.
