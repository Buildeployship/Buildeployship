# Jordan Taylor

I'm a systems thinker, and I enjoy building, deploying, and monitoring infrastructure.

I build delivery platforms end to end: the pipeline, the infrastructure it deploys to, and the telemetry that shows whether it's working. I automate delivery through multi-stage CI/CD pipelines and infrastructure as code, running an on-premises GitLab CI/CD platform with its own registry and runners that ships containerized services to both Nomad on-premises and AWS ECS Fargate, provisioned with Terraform. Services are instrumented with OpenTelemetry across metrics, logs, and traces on a Grafana LGTM stack; secrets are managed with HashiCorp Vault and SOPS, images are scanned with Trivy, and service-to-service traffic runs over Consul Connect mTLS. I'm security and documentation-minded: every build ships with architecture and operating documentation.

## Contact
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/buildeployship/)

## [Explore my homelab](https://github.com/Buildeployship/homelab)
The architecture, design decisions, and a guided path through every project.

## Technical Skills

**Automation:** GitLab CI/CD, GitHub Actions, Git, Terraform, Bash

**Delivery:** Linux, Docker, AWS (IAM, EC2, ECS, ECR, S3, ALB/ELB, VPC, Fargate), Consul, Nomad, Tailscale

**Observability:** OpenTelemetry, AWS CloudWatch, Grafana LGTM stack (Loki, Grafana, Tempo, Mimir)

**Security:** HashiCorp Vault, AWS Secrets Manager, SOPS, Trivy, Consul Connect (mTLS)
