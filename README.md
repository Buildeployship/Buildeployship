# Jordan Taylor

[![GitLab CI/CD](https://img.shields.io/badge/GitLab%20CI%2FCD-6%20stages-FC6D26?logo=gitlab&logoColor=white)](.gitlab-ci.yml)
[![GitHub Actions](https://github.com/Buildeployship/go-cicd-observability/actions/workflows/ci.yml/badge.svg)](https://github.com/Buildeployship/go-cicd-observability/actions)
[![Docker](https://img.shields.io/badge/Docker-multi--stage-2496ED?logo=docker&logoColor=white)](Dockerfile)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![Terraform](https://img.shields.io/badge/Terraform-1.14+-7B42BC?logo=terraform&logoColor=white)](https://www.terraform.io/)
[![AWS](https://img.shields.io/badge/AWS-ECS%20·%20Fargate%20·%20ECR%20·%20EC2%20·%20S3%20·%20IAM%20·%20VPC%20·%20ALB%2FELB%20·%20Secrets%20Manager%20·%20CloudWatch-FF9900?logo=amazonwebservices&logoColor=white)](aws/)
[![HashiCorp Vault](https://img.shields.io/badge/HashiCorp%20Vault-FFEC6E?logo=vault&logoColor=black)](https://developer.hashicorp.com/vault)
[![Bash](https://img.shields.io/badge/Bash-4EAA25?logo=gnubash&logoColor=white)](https://www.gnu.org/software/bash/)
[![Go](https://img.shields.io/badge/Go-00ADD8?logo=go&logoColor=white)](https://go.dev/)
[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)](https://git-scm.com/)
[![Linux](https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black)](https://www.kernel.org/)
[![Tailscale](https://img.shields.io/badge/Tailscale-242424?logo=tailscale&logoColor=white)](https://tailscale.com/)
[![Grafana LGTM](https://img.shields.io/badge/Grafana-LGTM%20Stack-F46800?logo=grafana&logoColor=white)](https://grafana.com/oss/)
![PMP](https://img.shields.io/badge/PMP-In%20Progress-informational?style=flat&logo=trello&logoColor=white)

## CONTACT

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/buildeployship/)

## SUMMARY

DevOps engineer with hands-on infrastructure and security engineering across on-premises and cloud environments. Automates delivery through multi-stage CI/CD pipelines and infrastructure as code, shipping containerized services instrumented for observability across metrics, logs, and traces.

## PROJECTS

### [go-cicd-observability](https://github.com/Buildeployship/go-cicd-observability)
Go webhook relay delivered through a multi-stage pipeline to on-premises and AWS targets.

`Go` `GitLab CI/CD` `Terraform` `AWS ECS Fargate` `Nomad` `OTel`

### [cicd-observability-stack](https://github.com/Buildeployship/cicd-observability-stack)
On-premises CI/CD and observability platform, with full architecture and operating documentation.

`GitLab CI/CD` `Docker Compose` `LGTM` `Nomad` `Consul` `Tailscale`

**Architecture:**
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

## TECHNICAL SKILLS

**Automation:** GitLab CI/CD, GitHub Actions, Git, Terraform, Ansible, Bash, Python

**Delivery:** Linux, Docker, Kubernetes (Helm, ArgoCD, EKS), AWS (IAM, EC2, ECS, ECR, S3, ALB/ELB, VPC, Fargate), Consul, Nomad, Tailscale

**Observability:** OpenTelemetry, AWS CloudWatch, Grafana LGTM stack (Loki, Grafana, Tempo, Mimir)

**Security:** HashiCorp Vault, AWS Secrets Manager, SOPS, Trivy, Consul Connect (mTLS)
