[![CI/CD](https://github.com/Buildeployship/go-cicd-observability/actions/workflows/ci.yml/badge.svg)](https://github.com/Buildeployship/go-cicd-observability/actions)
[![GitLab CI/CD](https://img.shields.io/badge/GitLab%20CI%2FCD-6%20stages-FC6D26?logo=gitlab&logoColor=white)](.gitlab-ci.yml)
[![Terraform](https://img.shields.io/badge/Terraform-1.14+-7B42BC?logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Docker](https://img.shields.io/badge/Docker-multi--stage-2496ED?logo=docker&logoColor=white)](Dockerfile)
[![AWS](https://img.shields.io/badge/AWS-ECS%20Fargate-FF9900?logo=amazonwebservices&logoColor=white)](terraform/)

# Jordan Taylor

DevOps & Platform Engineer

## ABOUT

DevOps & Platform Engineer building hardened CI/CD, observability, and delivery infrastructure across on-premise and cloud environments. Observability built on the Grafana LGTM stack — Loki, Grafana, Tempo, and Mimir. Every component is automated, version-controlled, pipelined through GitLab CI/CD, and shipped publicly on GitHub.

## Architecture

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

## PROJECTS

### [go-cicd-observability](https://github.com/Buildeployship/go-cicd-observability)
**Description**:
A Go webhook relay through multi-stage GitLab CI/CD with Grafana's Loki-Grafana-Tempo-Mimir (LGTM) observability stack, service mesh, and live AWS deployment. Instrumented end-to-end with OpenTelemetry for trace, metric, and log correlation.
<br>

**Technologies**:
Go · GitLab CI/CD · Terraform · AWS ECS Fargate · Nomad · OTel
<br>


### [cicd-observability-stack](https://github.com/Buildeployship/cicd-observability-stack)
**Description**:
Infrastructure-as-code and documentation for a on-premise GitLab CI/CD pipeline, LGTM observability stack, Nomad orchestration, and Tailscale networking on Arch Linux.
<br>

**Technologies**:
GitLab CE · Docker Compose · LGTM · Nomad · Consul · Tailscale
<br>

## SKILLS & EXPERTISE

**Domains:** Networking, Security, Secrets management, Incident response, Infrastructure as Code

**Automation:** CI/CD tooling (GitLab CI, GitHub Actions), Git, Terraform, Ansible, Bash, Go

**Delivery:** Docker, Nomad, Linux, AWS (IAM, EC2, ECS, ECR, S3, ALB/ELB), Consul, Tailscale, Cloudflare

**Observability:** CloudWatch, Loki, Grafana, Tempo, Mimir, Node exporter, Otel-collector, Alertmanager, Prometheus, OpenTelemetry

## COMPETENCIES

<ul>
  <li> Multi-Environment Deployment
  <li> Platform Reliability Engineering
  <li> CI/CD Pipeline Design & Automation
  <li> Developer Tooling & Experience
  <li> Infrastructure as Code
  <li> Containerization & Orchestration
  <li> GitOps & Version Control Workflows
  <li> Infrastructure Architecture & Networking
  <li> Configuration Management
  <li> Observability & Monitoring
  <li> Security & Secrets Management
  <li> Disaster Recovery & Backup Strategy
  <li> Linux Systems Administration
</ul>

## CONTACT
- [LinkedIn](https://www.linkedin.com/in/buildeployship/)
