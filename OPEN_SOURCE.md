# Open Source Contributions

[Haihan Jiang](https://github.com/Haihan-Jiang) | Production / SRE / Infrastructure

Merged upstream work across Linux runtimes, Kubernetes diagnostics, container tooling, cloud configuration, and developer infrastructure. Each contribution below links directly to its upstream pull request.

Verified against GitHub on **2026-09-07**. The linked final diffs are the source for implementation details.

[Profile](README.md) | [Structured contribution data](open-source-contributions.json)

## Selected Engineering Details

- **gVisor:** Apply OCI swap limits to pre-created cgroup v2 paths without overwriting caller-owned memory limits. Netstat compatibility uses matching zero-filled value rows for counters that gVisor does not track.
- **KHI:** Recognize truncated audit entries in GKE and Kubernetes logs, clear stale manifest reconstruction state, and handle condition continuity. The final implementation invalidates the previous manifest on truncation.
- **go-containerregistry:** Validate archive paths independently of the host OS; reject Windows-style traversal and drive prefixes, and filter unsafe relative link targets.
- **Composer local dev:** Create dependency files as the runtime Airflow user; propagate a configurable startup timeout through start/restart commands and readiness waits.
- **SecOps SOAR MCP:** Skip cleanup when initialization did not create a client and close only sessions that already exist.
- **syzkaller:** Improve Linux crash classification, automated email handling, and root-cause visibility for long build failures.

## google/gvisor

Linux runtime and cgroups.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-06-11 | runsc/cgroup: set swap for precreated cgroups | [#13276](https://github.com/google/gvisor/pull/13276) |
| 2026-06-11 | proc: include values in /proc/net/netstat | [#13275](https://github.com/google/gvisor/pull/13275) |

## GoogleCloudPlatform/khi

Kubernetes diagnostics.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-09-03 | Handle truncated Kubernetes audit logs | [#697](https://github.com/GoogleCloudPlatform/khi/pull/697) |
| 2026-06-11 | Handle slog attributes in KHI log formatter | [#708](https://github.com/GoogleCloudPlatform/khi/pull/708) |
| 2026-06-03 | fix: confirm refresh when backend disconnects | [#692](https://github.com/GoogleCloudPlatform/khi/pull/692) |

## google/go-containerregistry

Container image tooling.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-07-25 | Document tag and digest reference semantics | [#2325](https://github.com/google/go-containerregistry/pull/2325) |
| 2026-07-24 | Reject unsafe Windows archive paths in Extract | [#2330](https://github.com/google/go-containerregistry/pull/2330) |
| 2026-06-02 | fix(crane): avoid creating export tar on pull failure | [#2318](https://github.com/google/go-containerregistry/pull/2318) |

## GoogleCloudPlatform/composer-local-dev

Airflow development environments.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-09-03 | fix: write Airflow dependency file as runtime user | [#135](https://github.com/GoogleCloudPlatform/composer-local-dev/pull/135) |
| 2026-09-03 | Add configurable start timeout | [#136](https://github.com/GoogleCloudPlatform/composer-local-dev/pull/136) |

## google/syzkaller

Kernel fuzzing and diagnostics.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-06-15 | Improve AI job error reporting | [#7388](https://github.com/google/syzkaller/pull/7388) |
| 2026-06-03 | dashboard/app: avoid syzbot email reply loops | [#7420](https://github.com/google/syzkaller/pull/7420) |
| 2026-06-01 | pkg/report: parse int3 oops reports | [#7376](https://github.com/google/syzkaller/pull/7376) |

## google/mcp-security

Security automation and MCP.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-08-29 | fix: correct case details response key | [#257](https://github.com/google/mcp-security/pull/257) |
| 2026-08-29 | fix: make SOAR cleanup idempotent | [#258](https://github.com/google/mcp-security/pull/258) |
| 2026-08-29 | fix: avoid creating SOAR session on close | [#260](https://github.com/google/mcp-security/pull/260) |
| 2026-08-29 | fix: declare SOAR dotenv dependency | [#259](https://github.com/google/mcp-security/pull/259) |
| 2026-08-29 | fix: align SOAR setup entrypoint | [#261](https://github.com/google/mcp-security/pull/261) |

## GoogleCloudPlatform/kubernetes-engine-samples

GKE deployment and autoscaling samples.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-07-30 | Add safe-to-evict annotations to DRA installers | [#2081](https://github.com/GoogleCloudPlatform/kubernetes-engine-samples/pull/2081) |
| 2026-06-30 | Fix Model Armor sample path | [#2082](https://github.com/GoogleCloudPlatform/kubernetes-engine-samples/pull/2082) |
| 2026-06-30 | Fix T5 model serving doc links | [#2083](https://github.com/GoogleCloudPlatform/kubernetes-engine-samples/pull/2083) |

## google/benchmark

C++ benchmarking and build tooling.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-05-27 | Skip perf counter tests when counters are unavailable | [#2204](https://github.com/google/benchmark/pull/2204) |
| 2026-05-27 | Clarify DoNotOptimize const-ref warning | [#2201](https://github.com/google/benchmark/pull/2201) |
| 2026-05-26 | Skip errored runs when computing repetition statistics | [#2199](https://github.com/google/benchmark/pull/2199) |
| 2026-05-26 | Document CMake embedding guidance | [#2203](https://github.com/google/benchmark/pull/2203) |
| 2026-05-26 | Document static library benchmark registration | [#2200](https://github.com/google/benchmark/pull/2200) |
| 2026-05-26 | Clarify benchmark_main CMake target usage | [#2205](https://github.com/google/benchmark/pull/2205) |
| 2026-05-25 | Fix pkg-config paths for absolute install dirs | [#2198](https://github.com/google/benchmark/pull/2198) |

## google/stellar-engine

Cloud bootstrap and IAM.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-08-10 | Centralize deployment prerequisites | [#88](https://github.com/google/stellar-engine/pull/88) |
| 2026-07-07 | Clean up path to authorization markdown artifacts | [#89](https://github.com/google/stellar-engine/pull/89) |
| 2026-06-22 | Align DDG bootstrap region example | [#90](https://github.com/google/stellar-engine/pull/90) |
| 2026-06-22 | Align naming convention docs with DDG prefix | [#87](https://github.com/google/stellar-engine/pull/87) |
| 2026-05-26 | Deprivilege bootstrap default service accounts | [#68](https://github.com/google/stellar-engine/pull/68) |

## google/adk-go

Agent integration documentation.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-08-21 | docs: Explain adka2a handler wiring | [#893](https://github.com/google/adk-go/pull/893) |

## GoogleCloudPlatform/vertex-ai-creative-studio

AI tooling and cloud configuration.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-06-26 | Fix Pixie transitions for short clips | [#1444](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/pull/1444) |
| 2026-06-26 | Default character consistency image selection | [#1439](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/pull/1439) |
| 2026-06-26 | Document Gemini CLI cloud auth | [#1440](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/pull/1440) |
| 2026-05-30 | Expose Veo location in Terraform | [#1445](https://github.com/GoogleCloudPlatform/vertex-ai-creative-studio/pull/1445) |

## GoogleCloudPlatform/opentelemetry-operator-sample

Observability deployment documentation.

| Merged (UTC) | Contribution | Pull Request |
| --- | --- | --- |
| 2026-06-29 | Document Artifact Registry Docker auth setup | [#135](https://github.com/GoogleCloudPlatform/opentelemetry-operator-sample/pull/135) |

## Verification

This snapshot contains public, non-fork upstream repositories where GitHub reports Haihan-Jiang as the PR author and records a completed merge with a merge timestamp. It includes implementation, testing, configuration, and documentation contributions.

The structured file records the verification time, repository, PR title, URL, merge date, and available merge commit IDs. Tests mentioned in upstream discussions are historical validation; this contribution inventory does not represent a fresh execution of those test suites.

Live searches: [Google](https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3Agoogle) / [Google Cloud Platform](https://github.com/pulls?q=is%3Apr+is%3Amerged+author%3AHaihan-Jiang+org%3AGoogleCloudPlatform).
