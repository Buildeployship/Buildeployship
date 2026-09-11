# Jordan Taylor

[![GitHub Actions](https://github.com/Buildeployship/go-cicd-observability/actions/workflows/ci.yml/badge.svg)](https://github.com/Buildeployship/go-cicd-observability/actions)
[![GitLab CI/CD](https://img.shields.io/badge/GitLab%20CI%2FCD-6%20stages-FC6D26?logo=gitlab&logoColor=white)](.gitlab-ci.yml)
[![Terraform](https://img.shields.io/badge/Terraform-1.14+-7B42BC?logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Docker](https://img.shields.io/badge/Docker-multi--stage-2496ED?logo=docker&logoColor=white)](Dockerfile)
[![AWS](https://img.shields.io/badge/AWS-ECS%20Fargate-FF9900?logo=amazonwebservices&logoColor=white)](terraform/)
![PMP](https://img.shields.io/badge/PMP-In%20Progress-informational?style=flat&logo=trello&logoColor=white)

## CONTACT

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/buildeployship/)

## SUMMARY

Technical Project Manager with hands-on infrastructure and security engineering background. In DevOps I apply systems and security engineering to Automation, Delivery, and Observability.

I design, build, and operate across on-premises and cloud environment infrastructure. DevOps projects are scoped, tracked, secured, version-controlled, pipelined through GitLab CI/CD, and shipped publicly on GitHub.

In project management I've led crews, subcontractors, and vendors across concurrent sites, driving alignment across dependencies while owning schedules, compliance, and cost reporting to ownership.

Technical project delivery, with focus on security and compliance. Contract, contract-to-hire, or full-time.

## DEVOPS PROJECTS

### [go-cicd-observability](https://github.com/Buildeployship/go-cicd-observability)
**Description**:
A Go webhook relay app through multi-stage GitLab CI/CD with Grafana's Loki-Grafana-Tempo-Mimir (LGTM) observability stack, Consul Connect mutual-TLS service mesh, and AWS deployment. Instrumented end-to-end with OpenTelemetry for trace, metric, and log correlation.
<br>

**Technologies**:
Go · GitLab CI/CD · Terraform · AWS ECS Fargate · Nomad · OTel
<br>

### [cicd-observability-stack](https://github.com/Buildeployship/cicd-observability-stack)
**Description**:
Infrastructure-as-code and documentation for an on-premises GitLab CI/CD pipeline, Grafana's Loki-Grafana-Tempo-Mimir (LGTM) observability stack, Nomad orchestration, and Tailscale networking on Linux.
<br>

**Technologies**:
GitLab CE · Docker Compose · LGTM · Nomad · Consul · Tailscale
<br>

**Architecture**:

```
┌─────────────────────────────────────────────────────────────────────┐
│ cicd-observability-stack                                            │
│                                                                     │
│  ┌─────────────┐     ┌──────────────────┐     ┌─────────────────┐   │
│  │  GitLab CE  │───▶│  GitLab Runner   │───▶│  Loki · Grafana │   │
│  │  Registry   │     │  Docker executor │     │  Tempo · Mimir  │   │
│  └─────────────┘     └──────────────────┘     │  Alloy · OTel   │   │
│                                               └────────┬────────┘   │
└────────────────────────────────────────────────────────│────────────┘
                                                         │ observes
┌────────────────────────────────────────────────────────│────────────┐
│ go-cicd-observability                                  │            │
│                                                        ▼            │
│  ┌─────────────┐     ┌──────────────────┐     ┌─────────────────┐   │
│  │ Go webhook  │───▶│   GitLab CI/CD   │───▶│ Nomad · Consul  │   │
│  │ relay · OTel│     │   6 stages       │  ╔══│ mTLS  · homelab │   │
│  └─────────────┘     └──────────────────┘  ║  └─────────────────┘   │
│                                            ║                        │
│                                            ╚══▶┌─────────────────┐ │
│                                                 │ AWS ECS Fargate │ │
│                                                 │ Terraform · ALB │ │
│                                                 └─────────────────┘ │
└─────────────────────────────────────────────────────────────────────┘
```

## TECHNICAL SKILLS & EXPERTISE

**Technical:** Linux, Docker, Kubernetes (K8s, Helm, ArgoCD, EKS), AWS (IAM, EC2, ECS, ECR, S3, ALB/ELB, VPC, Fargate), AWS Secrets Manager, Tailscale, Cloudflare, HashiCorp Vault, Trivy, GitLab CI/CD, GitHub Actions, Git, Terraform, Bash, AWS CloudWatch, Grafana LGTM stack (Loki, Grafana, Tempo, Mimir)

**Delivery Methodologies & Frameworks:** Agile (Scrum, Kanban), Waterfall, Hybrid, DevSecOps, Risk Management, Scope & Budget Management, Root Cause Analysis (RCA), Critical Path Method (CPM), Lean Six Sigma (DMAIC), OKRs, ITIL, RAID logs, RACI

**Tooling:** Jira, Azure DevOps, ServiceNow, Confluence, SharePoint, Microsoft 365, Slack, Lucidchart, Figma, ClickUp, Linear, Asana, Trello, Monday.com, Notion, Google Workspace, MS Teams, draw.io