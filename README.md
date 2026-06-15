# Hi, I'm Matthew 👋

**Security / GRC engineer (11+ yrs) moving deeper into DevOps & Cloud.**
Primary technical contact for SOX, PCI-DSS, and FISMA audits; remediated 450+ SOX
findings; CIS/NIST CSF hardening; AWS + Kubernetes + Terraform on the build side.
CISSP and AZ-500 in progress.

I don't think a wall of certs proves much on its own. What proves something is
that you **broke something, fixed something, and built something** — and can show
how you thought through it. So instead of a list of acronyms, here are two
projects I built and can walk you through line by line.

---

## 🔧 Projects

### [CloudRiskIQ](https://github.com/yellowlotuscg/cloudriskiq) — security posture + compliance, as code
Ingests security findings from AWS, Azure, endpoints, and GitHub; normalizes them;
**risk-scores** each one by context (not just raw severity); maps every finding to
**NIST CSF / CIS / PCI-DSS / SOX / FISMA** controls; and generates an audit-ready
evidence pack. FastAPI + Next.js + a Python CLI. Runs offline on synthetic data.

> **Broke:** in real audits, "severity" isn't "risk," and control-mapped evidence
> was assembled by hand. **Fixed:** a transparent risk-scoring engine + an
> automated control mapper. **Built:** a working full-stack app with 24 tests.

→ [Read the writeup](https://github.com/yellowlotuscg/cloudriskiq/blob/main/docs/broke-fixed-built.md)

### [self-healing-k8s-pipeline](https://github.com/yellowlotuscg/self-healing-k8s-pipeline) — the EKS incident, made runnable
A self-healing Kubernetes CI/CD + observability demo that reproduces a real EKS
incident I worked — a pod-scheduling stampede that cascaded into node failures —
on a free local `kind` cluster, then ships the fixes as code. `make break`
reproduces it; `make heal` recovers it.

> **Broke:** no resource requests + a liveness probe doing readiness's job → the
> scheduler overpacked nodes → memory pressure → cascading evictions →
> CrashLoopBackOff. **Fixed:** right-sized requests/limits, tuned probes, a PDB,
> topology spread, and a Jenkins-on-k8s rebuild with EFS-backed storage.
> **Built:** the manifests, Terraform, Ansible, CI/CD, Prometheus/Grafana alerts,
> and a full post-mortem.

→ [Read the post-mortem](https://github.com/yellowlotuscg/self-healing-k8s-pipeline/blob/main/docs/INCIDENT-POSTMORTEM.md)

---

## 🧰 What I work with

**Security / GRC:** SOX · PCI-DSS · FISMA · NIST CSF · NIST 800-53 · CIS Controls ·
Zero Trust · IAM / RBAC / MFA · Entra ID · Qualys vuln management

**DevOps / Cloud:** AWS (EKS, IAM, Lambda, CloudWatch, DynamoDB, SNS/SQS, ALB, S3) ·
Kubernetes · Terraform · Ansible · Jenkins · GitHub Actions

**Languages & tooling:** Python (FastAPI) · Bash · PowerShell ·
Datadog · Prometheus · Grafana · Git

---

## 📫 Reach me

- 🌐 Portfolio: **https://yellowlotuscg.github.io/portfolio/**
- 📧 yellowlotuscg@gmail.com
