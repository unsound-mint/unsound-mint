### Hi, I'm Denis 👋

Backend and full-stack engineer and Computer Science student at **Nazarbayev University** (class of 2027), based in Astana, Kazakhstan (UTC+5). I build production systems end to end, from the database schema to deployment and monitoring, and I run two of them in production today.

Looking for **backend (Go), DevOps/SRE and full-stack (TypeScript/Next.js)** roles and internships, remote or in Astana.

#### In production

- **[Happy End](case-studies/happyend.md)**: e-commerce platform with ~7,000 monthly users, which I develop on my own. I moved it from 1C-Bitrix to Next.js + PostgreSQL + a PHP API, with Halyk Bank online payments, analytics in BigQuery and 3,700+ automated tests.
- **[City news platform](case-studies/city-portals.md)**: a multi-tenant platform for two city portals that I built alone. Go API, PostgreSQL with row-level security and hybrid search, Kaspi Pay webhooks, CI/CD with automatic rollback, Prometheus/Grafana/OpenTelemetry.

#### Projects

| | |
|---|---|
| [**payhook**](https://github.com/unsound-mint/payhook) | Payments and webhooks service in Go: idempotent API, signed webhooks, transactional outbox to NATS JetStream, retries with dead letters. Helm chart tested on kind in CI; zero failed requests during a rolling restart under load. |
| [**payhook-infra**](https://github.com/unsound-mint/payhook-infra) | Terraform for payhook on AWS: VPC, ALB + Auto Scaling, RDS, Secrets Manager, CloudWatch alarms, GitHub Actions deploys through OIDC, `terraform test`, tflint, Trivy. |
| [**MusicRoomBot**](https://github.com/unsound-mint/MusicRoomBot) | Telegram booking bot used by NU's Music Room. Async Python, PostgreSQL constraints against double booking, Alembic, CI. |
| [**water-meter-anomaly-detection**](https://github.com/unsound-mint/water-meter-anomaly-detection) | Anomaly detection in water-meter consumption data. |
| [**nuclear-morphometry**](https://github.com/unsound-mint/nuclear-morphometry) | GPU pipeline for 2D/3D analysis of cell nuclei from confocal microscopy (Cellpose-SAM, PyTorch, Polars). |

#### Stack

**Go** · **TypeScript / Next.js / React** · PHP · Python · PostgreSQL · Redis · NATS · Docker · Kubernetes (Helm) · Terraform · AWS · GitHub Actions · Prometheus · Grafana · OpenTelemetry · Cloudflare · Linux

I also do research at NU: high-performance Julia pipelines for large 3D astronomical datasets on the university HPC cluster.

#### Contact

[LinkedIn](https://www.linkedin.com/in/denisxandreyev/) · denisxandreyev@gmail.com · English C1, Russian native
