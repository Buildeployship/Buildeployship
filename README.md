[![CI/CD](https://github.com/Buildeployship/go-cicd-observability/actions/workflows/ci.yml/badge.svg)](https://github.com/Buildeployship/go-cicd-observability/actions)
[![GitLab CI/CD](https://img.shields.io/badge/GitLab%20CI%2FCD-6%20stages-FC6D26?logo=gitlab&logoColor=white)](.gitlab-ci.yml)
[![Terraform](https://img.shields.io/badge/Terraform-1.14+-7B42BC?logo=terraform&logoColor=white)](https://www.terraform.io/)
[![Docker](https://img.shields.io/badge/Docker-multi--stage-2496ED?logo=docker&logoColor=white)](Dockerfile)
[![AWS](https://img.shields.io/badge/AWS-ECS%20Fargate-FF9900?logo=amazonwebservices&logoColor=white)](terraform/)

# Jordan Taylor

## ABOUT

DevOps Engineer with hands-on experience designing, building, and operating infrastructure across on-premise and cloud environments. I work across the full stack — Linux systems, networking, continuous integration and continuous delivery (CI/CD) pipelines, monitoring & observability and delivery infrastructure with a security-first approach throughout.

My on-premise infrastructure runs: GitLab CE, the Grafana LGTM stack (Loki, Grafana, Tempo, Mimir), Nomad orchestration, and AWS-integrated pipelines. Every component is automated, version-controlled, pipelined through GitLab CI/CD, and shipped publicly on GitHub.

## SKILLS & EXPERTISE

**Domains & Methodologies:** Infrastructure as Code (IaC), CI/CD, GitOps, Configuration Management, Distributed Systems, Storage, Container Orchestration, Networking, On-premise Infrastructure, Security Hardening, High Availability (HA), Fault Tolerance, Disaster Recovery (DR), Service Discovery, Load Balancing, Horizontal Scaling, SLO/SLI Definition, Reliability Engineering, Observability-Driven Development, Automation of Toil

**Security:** IAM/Least-Privilege Policy Design, Container/Image Scanning, CIS (Center for Internet Security) Benchmarks, Secrets Management

**Automation:** GitLab CI, GitHub Actions, Git, Terraform, Bash, SOPS, AWS Secrets Manager, Trivy

**Delivery:** Docker, Nomad, Linux, AWS (IAM, EC2, S3, ECS, ECR, ALB/ELB, Fargate), Consul Connect mutual-TLS service mesh, Tailscale, Cloudflare, Render, HashiCorp Vault

**Observability:** CloudWatch, LGTM stack (Loki, Grafana, Tempo, Mimir), Node exporter, Alertmanager, Prometheus, OpenTelemetry, Otel-Collector

## COMPETENCIES

<ul>
  <li> Infrastructure
    <ul>
      <li> Storage Architecture & Data Management
      <li> Network Segmentation & Traffic Control
      <li> High Availability & Fault Tolerance
      <li> Infrastructure Architecture & Networking
      <li> Linux Systems Administration
    </ul>
  <li> Platform & orchestration
    <ul>
      <li> Multi-Environment Deployment
      <li> Containerization & Orchestration
      <li> Service Mesh & Internal DNS
      <li> Configuration Management
      <li> Infrastructure as Code
    </ul>
  <li> Delivery & automation
    <ul>
      <li> CI/CD Pipeline Design & Automation
      <li> GitOps & Version Control Workflows
      <li> Developer Tooling & Process Engineering
    </ul>
  <li> Operations
    <ul>
      <li> Platform Reliability Engineering
      <li> Observability & Monitoring
      <li> Capacity Planning & Resource Optimization
      <li> Threat Detection & Incident Response
      <li> Secrets Management & Credential Rotation
      <li> Disaster Recovery & Backup Strategy
    </ul>
</ul>

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

## CONTACT
- [LinkedIn](https://www.linkedin.com/in/buildeployship/)
- [X](https://x.com/buildeployship)
