# Haihan Jiang

Production / SRE / infrastructure engineer focused on reliable systems, Kubernetes/cloud operations, observability, and automation that is safe to run in production.

I like work where the result is reviewable: smaller diffs, clear failure modes, tests or gates that prove behavior, and evidence a future on-call engineer can trust.

Best fit: SRE, Production Engineering, Infrastructure, Platform, Cloud/DevOps, and backend infrastructure roles close to real operations.

## Fast Proof

- Verified upstream PRs merged in Google and Google Cloud Platform maintained repositories.
- Recent upstream work across `gVisor`, `syzkaller`, `KHI`, `go-containerregistry`, `google/benchmark`, `stellar-engine`, and `vertex-ai-creative-studio`.
- Built a GKE AI inference reliability lab with OpenTelemetry traces, Kubernetes manifests, incident replay, and SLO-style evidence gates.
- Production context includes Meta monetization data infrastructure and SHEIN gateway infrastructure work.
- Experience around production gateways, Kubernetes/AKS-style platforms, Kafka, ZooKeeper, Elasticsearch, Terraform, runbooks, dashboards, and operational automation.

## Contributor Signals

<p align="left">
  <a href="https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3Agoogle"><img alt="Google upstream contributor" src="https://img.shields.io/badge/Google-upstream%20contributor-4285F4?style=flat-square&logo=google&logoColor=white"></a>
  <a href="https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3AGoogleCloudPlatform"><img alt="Google Cloud upstream contributor" src="https://img.shields.io/badge/Google%20Cloud-upstream%20contributor-1A73E8?style=flat-square&logo=googlecloud&logoColor=white"></a>
  <a href="https://github.com/google/gvisor/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="gVisor contributor" src="https://img.shields.io/badge/gVisor-merged%20PRs-34A853?style=flat-square"></a>
  <a href="https://github.com/google/syzkaller/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="syzkaller contributor" src="https://img.shields.io/badge/syzkaller-merged%20PRs-FBBC04?style=flat-square"></a>
  <a href="https://github.com/GoogleCloudPlatform/khi/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="KHI contributor" src="https://img.shields.io/badge/KHI-merged%20PRs-1A73E8?style=flat-square"></a>
  <a href="https://github.com/google/go-containerregistry/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="go-containerregistry contributor" src="https://img.shields.io/badge/go--containerregistry-merged%20PR-00ADD8?style=flat-square&logo=go&logoColor=white"></a>
  <a href="https://github.com/google/benchmark/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang"><img alt="Google Benchmark contributor" src="https://img.shields.io/badge/google%2Fbenchmark-merged%20PRs-5F6368?style=flat-square&logo=cplusplus&logoColor=white"></a>
</p>

Projects where my upstream PRs have been merged: `google/gvisor`, `google/syzkaller`, `GoogleCloudPlatform/khi`, `google/go-containerregistry`, `google/benchmark`, `google/stellar-engine`, and `GoogleCloudPlatform/vertex-ai-creative-studio`.

## Selected Upstream Work

| Area | Evidence |
| --- | --- |
| Container/runtime reliability | [`google/gvisor#13276`](https://github.com/google/gvisor/pull/13276) - set swap for precreated cgroups |
| Kernel fuzzing / report parsing | [`google/syzkaller#7420`](https://github.com/google/syzkaller/pull/7420), [`google/syzkaller#7376`](https://github.com/google/syzkaller/pull/7376) |
| Kubernetes troubleshooting | [`GoogleCloudPlatform/khi#708`](https://github.com/GoogleCloudPlatform/khi/pull/708), [`GoogleCloudPlatform/khi#692`](https://github.com/GoogleCloudPlatform/khi/pull/692) |
| Container image tooling | [`google/go-containerregistry#2318`](https://github.com/google/go-containerregistry/pull/2318) |
| C++ build/test infrastructure | [`google/benchmark#2198`](https://github.com/google/benchmark/pull/2198), [`#2199`](https://github.com/google/benchmark/pull/2199), [`#2204`](https://github.com/google/benchmark/pull/2204) |
| Safer cloud defaults | [`google/stellar-engine#68`](https://github.com/google/stellar-engine/pull/68), [`GoogleCloudPlatform/vertex-ai-creative-studio#1445`](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/pull/1445) |

Live searches:
[`org:google merged PRs`](https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3Agoogle) /
[`org:GoogleCloudPlatform merged PRs`](https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3AGoogleCloudPlatform)

## Featured Builds

### [GKE AI Inference Reliability Lab](https://github.com/Haihan-Jiang/gke-ai-workload-observability-recipes)

A runnable infrastructure lab for AI inference reliability:

- OpenTelemetry trace collection and Kubernetes resource context
- incident replay for baseline traffic, cache-miss latency, dependency timeout, and rollout regression
- SLO-style reliability gate with published evidence reports
- GKE-shaped manifests for collector RBAC, PVC-backed queue storage, and sample workloads

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

_Merged PR status was verified from GitHub on 2026-06-14. I keep merged work separate from review-in-progress work._
