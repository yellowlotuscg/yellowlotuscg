# Matthew Coggins | Yellow Lotus Consulting Group

I work across DevOps, cloud operations, security, and business automation. Through Yellow Lotus Consulting Group, I help small businesses implement useful systems and understand how to run them. My experience includes a Cart.com client contract delivered through Yellow Lotus, not separate direct employment.

I am interested in DevOps and CloudOps roles where reliable infrastructure, clear incident response, and practical automation matter.

## Public repositories

These are the main public examples. Each one is a demo, a lab, or a reconstruction. Read the project's scope and limits before treating it as production work.

- [CloudRiskIQ](https://github.com/yellowlotuscg/cloudriskiq) organizes sample security findings, explains risk scores, and exports evidence for human review. It does not certify compliance.
- [Self-healing Kubernetes pipeline](https://github.com/yellowlotuscg/self-healing-k8s-pipeline) is a local recreation of reliability problems, with deployment configuration, incident analysis, and a runbook. It is not a copy of a client's production environment.
- [CloudWatch observability lab](https://github.com/yellowlotuscg/cloudwatch-observability-lab) is a Terraform lab for CloudWatch alarms, dashboards, log insights, and SNS alerting around a sample app that emits metrics. The repository does not claim a live AWS deployment.
- [Prometheus and Grafana homelab](https://github.com/yellowlotuscg/prometheus-grafana-homelab-stack) is a Docker Compose stack with Prometheus, Grafana, Node Exporter, and Alertmanager, plus alert rules, dashboards, and a runbook.
- [Agent workflow control plane](https://github.com/yellowlotuscg/agentic-workflow-control-plane) is a small example of checkpoints, recovery states, and human approval before an external action.

Other public examples:

- [Deployment starter](https://github.com/yellowlotuscg/small-business-deployment-starter) is a local inventory API, with recovery procedures, staff training, and AWS, GCP, and Azure reference paths. The cloud paths are not live deployments.
- [Datadog observability proof](https://github.com/yellowlotuscg/datadog-observability-proof) is synthetic dashboard and monitor configuration with local consistency tests.
- [Lead workflow demo](https://github.com/yellowlotuscg/lead-operations-control-plane) covers sample enquiries, prioritization, and draft follow-ups, with an approval step before consequential action.
- [AI training framework](https://github.com/yellowlotuscg/ai-adoption-operating-system) includes safe-use materials, a facilitator guide, a source-checking lab, an assessment, and a supervised-pilot handoff. The [workshop and pilot package](https://github.com/yellowlotuscg/ai-adoption-operating-system#workshop-and-supervised-pilot-package) says what is included and what still needs review. No measured client training results are claimed.
- [LogRhythm detection proof](https://github.com/yellowlotuscg/logrhythm-detection-proof) is a synthetic authentication-event investigation and tested detection logic. It is not an exported vendor rule.
- [CTERA operations proof](https://github.com/yellowlotuscg/ctera-operations-proof) covers synthetic fleet and backup checks, with the adapter boundary written down.

## Pattern case studies

Each of these takes one enterprise design pattern and builds it from scratch on synthetic data, with infrastructure as code that is validated in CI but not deployed. Every repository runs offline and has secret scanning in CI.

- [Blue-green edge deploy](https://github.com/yellowlotuscg/blue-green-edge-deploy) (Blue-Green Deployment): a static site on CloudFront and S3 with smoke-test-gated promotion, one-command rollback, and an edge auth gate for admin routes. Terraform.
- [Idempotent inbox triage](https://github.com/yellowlotuscg/idempotent-inbox-triage) (Idempotency Keys, Transactional Outbox): an explainable email rules engine on SES, EventBridge, and Lambda, with fault-injection tests for duplicate deliveries and crashes. Terraform.
- [Feature flag release gates](https://github.com/yellowlotuscg/feature-flag-release-gates) (Feature Flags, quality gates): a .NET 8 API on Azure Container Apps with App Configuration flags, a kill switch, policy-as-code merge checks, and an approval audit report. Bicep.
- [Bulkhead agent router](https://github.com/yellowlotuscg/bulkhead-agent-router) (Bulkhead, Circuit Breaker): a multi-tenant task router for worker agents on Azure Service Bus and Functions, with a chaos test showing one tenant's failures do not reach another. Bicep.
- [Event-sourced knowledge hub](https://github.com/yellowlotuscg/event-sourced-knowledge-hub) (Event Sourcing): an append-only document store on DynamoDB Streams and Lambda with optimistic concurrency, deterministic replay, and ingest-time secret scanning. TypeScript, Terraform.
- [CQRS faceted search](https://github.com/yellowlotuscg/cqrs-faceted-search) (CQRS): separate write and search models for an equipment-manual catalog, with provenance on every hit and index rebuilds that do not block writes. Python, React, Bicep.
- [Claim-check handoff ledger](https://github.com/yellowlotuscg/claim-check-handoff-ledger) (Claim Check): schema-validated handoff records for long-running work, with content-addressed context storage and stale-reference detection. TypeScript, Bicep.

## For small businesses

I offer implementation help with automation, business workflows, and practical AI tools. Optional training can accompany a deployment so staff can use the tools, check their outputs, protect business information, and know when to ask for human review. A useful place to start is the [deployment starter](https://github.com/yellowlotuscg/small-business-deployment-starter).

## How to read this work

Public code here is not evidence of a production deployment, client savings, or a certification. Client source code, credentials, private records, and production infrastructure stay out of these repositories. The public examples use synthetic or deliberately sanitized inputs. I review AI-assisted work against the code and the evidence, and I keep the tooling attribution.

## Contact

[Yellow Lotus Consulting](https://yellowlotuscg.com) takes consulting enquiries. The [public proof index](https://yellowlotuscg.com/proof-of-concepts/) lists more examples.

This profile repository is under the [MIT License](LICENSE).
