# Haihan Jiang

Production / SRE / infrastructure engineer focused on reliable systems, Kubernetes/cloud operations, observability, and automation that is safe to run in production.

Upstream contributor to **gVisor**, **KHI**, **go-containerregistry**, **syzkaller**, **Composer local dev**, and **Google SecOps MCP**. My merged work covers Linux runtime behavior, Kubernetes diagnostics, container archive safety, and service lifecycle reliability.

## Contributor Signals

<p align="left">
  <a href="https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3Agoogle"><img alt="Google upstream contributor" src="https://img.shields.io/badge/Google-upstream%20contributor-4285F4?style=flat-square&logo=google&logoColor=white"></a>
  <a href="https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3AGoogleCloudPlatform"><img alt="Google Cloud upstream contributor" src="https://img.shields.io/badge/Google%20Cloud-upstream%20contributor-1A73E8?style=flat-square&logo=googlecloud&logoColor=white"></a>
  <a href="https://github.com/google/gvisor/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="gVisor contributor" src="https://img.shields.io/badge/gVisor-contributor-34A853?style=flat-square"></a>
  <a href="https://github.com/GoogleCloudPlatform/khi/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="KHI contributor" src="https://img.shields.io/badge/KHI-contributor-1A73E8?style=flat-square"></a>
  <a href="https://github.com/google/go-containerregistry/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="go-containerregistry contributor" src="https://img.shields.io/badge/go--containerregistry-contributor-00ADD8?style=flat-square&logo=go&logoColor=white"></a>
  <a href="https://github.com/GoogleCloudPlatform/composer-local-dev/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="Composer local dev contributor" src="https://img.shields.io/badge/Composer%20local%20dev-contributor-137333?style=flat-square"></a>
  <a href="https://github.com/google/syzkaller/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="syzkaller contributor" src="https://img.shields.io/badge/syzkaller-contributor-9C6500?style=flat-square"></a>
  <a href="https://github.com/google/mcp-security/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="SecOps MCP contributor" src="https://img.shields.io/badge/SecOps%20MCP-contributor-5F6368?style=flat-square"></a>
  <a href="https://github.com/google/benchmark/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="Google Benchmark contributor" src="https://img.shields.io/badge/Google%20Benchmark-contributor-00599C?style=flat-square&logo=cplusplus&logoColor=white"></a>
</p>

## Selected Upstream Work

| Project | Technical Contribution | Merged Evidence |
| --- | --- | --- |
| **gVisor** | Honor OCI swap limits in pre-created cgroup v2 paths while preserving caller-owned limits; emit Linux-compatible netstat name/value rows. | [#13276](https://github.com/google/gvisor/pull/13276), [#13275](https://github.com/google/gvisor/pull/13275) |
| **KHI** | Detect truncated Kubernetes audit logs, invalidate stale manifest state, and preserve condition-timeline continuity with regression tests. | [#697](https://github.com/GoogleCloudPlatform/khi/pull/697) |
| **go-containerregistry** | Harden flattened archive export against Windows-style traversal and drive-prefixed paths, with regression coverage for entries and relative links. | [#2330](https://github.com/google/go-containerregistry/pull/2330) |
| **Composer local dev** | Fix Airflow dependency-file ownership under the runtime user; add configurable startup timeouts across the CLI and readiness checks. | [#135](https://github.com/GoogleCloudPlatform/composer-local-dev/pull/135), [#136](https://github.com/GoogleCloudPlatform/composer-local-dev/pull/136) |
| **syzkaller** | Parse Linux int3 crash reports, prevent syzbot reply loops, and surface build root causes in AI job errors. | [#7376](https://github.com/google/syzkaller/pull/7376), [#7420](https://github.com/google/syzkaller/pull/7420), [#7388](https://github.com/google/syzkaller/pull/7388) |
| **SecOps SOAR MCP** | Guard cleanup after failed initialization and avoid creating HTTP sessions during shutdown. | [#258](https://github.com/google/mcp-security/pull/258), [#260](https://github.com/google/mcp-security/pull/260) |
| **GKE samples** | Mark NVIDIA DRA installer pods safe to evict so installer DaemonSets do not block autoscaler scale-down. | [#2081](https://github.com/GoogleCloudPlatform/kubernetes-engine-samples/pull/2081) |
| **Google Benchmark** | Exclude errored repetitions from statistics and skip hardware-counter tests when counters are unavailable. | [#2199](https://github.com/google/benchmark/pull/2199), [#2204](https://github.com/google/benchmark/pull/2204) |
| **Stellar Engine** | Remove default-service-account project IAM grants in Terraform bootstrap projects. | [#68](https://github.com/google/stellar-engine/pull/68) |

[Full contribution record](OPEN_SOURCE.md) includes additional merged work in ADK Go, Vertex AI Creative Studio, and the OpenTelemetry Operator sample.

Live upstream searches: [Google](https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3Agoogle) / [Google Cloud Platform](https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3AGoogleCloudPlatform).

## Production Context

- Production context includes Meta monetization data infrastructure and SHEIN gateway infrastructure work.
- Experience around production gateways, Kubernetes/AKS-style platforms, Kafka, ZooKeeper, Elasticsearch, Terraform, runbooks, dashboards, and operational automation.

## Featured Builds

### [GKE Workload Reliability Lab](https://github.com/Haihan-Jiang/gke-ai-workload-observability-recipes)

A runnable Kubernetes reliability lab for production-style workloads:

- OpenTelemetry trace collection and Kubernetes resource context
- incident replay for baseline traffic, cache-miss latency, dependency timeout, and rollout regression
- SLO-style reliability gate with published evidence reports
- GKE-shaped manifests for collector RBAC, PVC-backed queue storage, NetworkPolicy, PDBs, and sample workloads
- CI validation that regenerates evidence, checks JSON/YAML, runs tests, and enforces a Kubernetes production manifest review

### [Release Evidence Gate](https://github.com/Haihan-Jiang/release-evidence-gate)

An offline release go/no-go gate for production-adjacent rollouts:

- evaluates baseline and canary windows from committed rollout evidence
- checks error rate, p95 latency, burn rate, rollback events, pager alerts, change freeze state, and required approvals
- writes JSON for automation and Markdown for release records
- dependency-free Python package with unit tests and GitHub Actions CI

## What I Optimize For

- Production changes that can be rolled out, observed, and rolled back.
- Automation with explicit inputs, validation, state, side effects, and retry boundaries.
- Reliability evidence: runbooks, dashboards, audit trails, tests, and incident reports.
- Practical open-source changes that reduce ambiguity for maintainers and users.

## Stack

`Python` `Go` `C++` `Java` `SQL` `Bash` `Linux` `Kubernetes` `AKS` `GKE` `OpenTelemetry` `Terraform` `Ansible` `Nginx/APISIX` `Kafka` `ZooKeeper` `Elasticsearch` `CMake` `pkg-config` `GitHub Actions`

## Contact

- GitHub: [Haihan-Jiang](https://github.com/Haihan-Jiang)
- Engineering profile: [haihan-jiang.github.io](https://haihan-jiang.github.io/)
- LinkedIn: [haihan-jiang](https://www.linkedin.com/in/haihan-jiang/)
- Email: [haihanj99@gmail.com](mailto:haihanj99@gmail.com)

_Upstream merge status verified on 2026-09-07. [Contribution evidence](OPEN_SOURCE.md)._
