# Rolling benchmark history: Known AI repos vs older solid OSS repos

Latest update: 2026-09-28
History dir: `benchmarks/history/known-ai-vs-solid-oss/`
Pinned baseline snapshot: `benchmarks/results/known-ai-vs-solid-oss.json` (2026-04-26)
Pinned baseline analyzer version: 0.3.0

## Goal

Compare a cohort of known AI-generated JavaScript/TypeScript repos against well-regarded OSS repos, with the mature-OSS cohort pinned to the latest default-branch commit on or before 2025-01-01, using exact commit SHAs and normalized analyzer metrics. This rolling history tracks the same repos at the default-branch revision that existed at each recorded run time so the benchmark can show movement over time.

## Refresh

```bash
bun run benchmark:history
```

To backfill earlier weekly points honestly, rerun the history job with a past timestamp so each repo resolves the default-branch commit that existed at that time:

```bash
bun run benchmark:history --recorded-at 2026-04-06T12:00:00Z
```

## Latest analyzer revisions

- `0.4.0` @ `86515a2` — 18 latest repo snapshots

## Latest cohort medians

| Cohort | Repo count | Median current blended | Median score/file | Median findings/file |
|---|---:|---:|---:|---:|
| explicit-ai | 9 | **4.76** | 1.25 | 0.34 |
| mature-oss | 9 | **1.00** | 0.16 | 0.06 |

## AI cohort latest standings

| Repo | Points | Trend (pinned) | Latest ref | Current blended | Latest pinned | Highest pinned | Δ prev (pinned) | Δ first (pinned) | Score/file | Findings/file |
|---|---:|---|---|---:|---:|---:|---:|---:|---:|---:|
| [redwoodjs/agent-ci](https://github.com/redwoodjs/agent-ci) | 28 | █████▁▁▁ | `main@c8597bb` | **5.93** | **9.01** | **9.62** | 0.00 | +5.10 | 1.33 | 0.40 |
| [jiayun/DevWorkbench](https://github.com/jiayun/DevWorkbench) | 28 | ▅▅▅▅▅▅▅▅ | `main@27f0d1a` | **5.92** | **8.99** | **8.99** | 0.00 | +5.59 | 1.26 | 0.47 |
| [garrytan/gstack](https://github.com/garrytan/gstack) | 28 | █▇▆▆▆▅▂▁ | `main@01593aa` | **5.46** | **8.29** | **11.92** | -0.38 | +1.92 | 1.25 | 0.35 |
| [openclaw/openclaw](https://github.com/openclaw/openclaw) | 28 | ▂▁▁▃▄▅██ | `main@dfd4cc8` | **5.12** | **7.77** | **7.77** | +0.05 | +4.84 | 1.39 | 0.36 |
| [emdash-cms/emdash](https://github.com/emdash-cms/emdash) | 26 | ▂▁▃▂▄▄▇█ | `main@698a0f8` | **4.39** | **6.67** | **6.67** | +0.04 | +4.49 | 1.26 | 0.32 |
| [cloudflare/vinext](https://github.com/cloudflare/vinext) | 28 | ▇▇▄▁▁█▅▁ | `main@074e64f` | **2.49** | **3.77** | **4.11** | -0.08 | +1.79 | 0.48 | 0.14 |
| [modem-dev/hunk](https://github.com/modem-dev/hunk) | 28 | ▁▂▁▅▇███ | `main@6c95708` | **2.30** | **3.49** | **3.59** | -0.03 | +2.68 | 0.55 | 0.19 |
| [FullAgent/fulling](https://github.com/FullAgent/fulling) | 28 | ▅▅▅▅▅▅▅▅ | `main@f48efce` | **1.74** | **2.64** | **10.28** | 0.00 | +0.48 | 0.20 | 0.05 |
| [robinebers/openusage](https://github.com/robinebers/openusage) | 28 | n/a | `main@4ce7887` | **n/a** | **n/a** | **6.56** | n/a | n/a | n/a | n/a |

## Mature OSS cohort latest standings

| Repo | Points | Trend (pinned) | Latest ref | Current blended | Latest pinned | Highest pinned | Δ prev (pinned) | Δ first (pinned) | Score/file | Findings/file |
|---|---:|---|---|---:|---:|---:|---:|---:|---:|---:|
| [withastro/astro](https://github.com/withastro/astro) | 28 | ▁▇█▇█▇██ | `main@404014a` | **1.61** | **2.45** | **2.46** | +0.00 | +0.90 | 0.20 | 0.07 |
| [umami-software/umami](https://github.com/umami-software/umami) | 28 | ▁▆████▇▇ | `master@ec0ff50` | **1.49** | **2.26** | **2.35** | 0.00 | +1.21 | 0.25 | 0.07 |
| [vitejs/vite](https://github.com/vitejs/vite) | 28 | ██▄▄▁▄▅▂ | `main@afaf48b` | **1.36** | **2.07** | **2.11** | -0.01 | +0.55 | 0.16 | 0.05 |
| [payloadcms/payload](https://github.com/payloadcms/payload) | 28 | ▁▁▁▃▄▅▆█ | `main@124b55a` | **1.04** | **1.58** | **1.58** | +0.07 | +0.26 | 0.14 | 0.04 |
| [egoist/tsup](https://github.com/egoist/tsup) | 28 | ▅▅▅▅▅▅▅▅ | `main@b6bcae8` | **1.00** | **1.52** | **1.52** | 0.00 | +0.60 | 0.15 | 0.06 |
| [pmndrs/zustand](https://github.com/pmndrs/zustand) | 28 | █▁▁▁▁▁▁▁ | `main@b57db4f` | **0.88** | **1.33** | **1.38** | 0.00 | -0.05 | 0.19 | 0.08 |
| [sindresorhus/execa](https://github.com/sindresorhus/execa) | 28 | ▅▅▅▅▅▅▅▅ | `main@8017b27` | **0.65** | **0.98** | **1.10** | 0.00 | +0.09 | 0.09 | 0.02 |
| [mikaelbr/node-notifier](https://github.com/mikaelbr/node-notifier) | 28 | ▅▅▅▅▅▅▅▅ | `master@b36c237` | **0.62** | **0.95** | **0.95** | 0.00 | +0.53 | 0.08 | 0.04 |
| [vercel/hyper](https://github.com/vercel/hyper) | 28 | ▅▅▅▅▅▅▅▅ | `canary@30ec0a2` | **0.59** | **0.90** | **0.90** | 0.00 | +0.49 | 0.63 | 0.15 |

## Table legend

- `Current blended` = latest repo score vs the current mature-OSS medians from the same rolling run.
- `Latest pinned` = latest repo score vs the frozen pinned mature-OSS baseline snapshot.
- `Highest pinned` = highest stored repo score on that same pinned baseline.
- `Δ prev (pinned)` = latest pinned - previous week's pinned score.
- `Δ first (pinned)` = latest pinned - first stored pinned score for that repo.

## Biggest increases vs previous week

- [payloadcms/payload](https://github.com/payloadcms/payload) — +0.07 vs previous week (pinned blended)
- [openclaw/openclaw](https://github.com/openclaw/openclaw) — +0.05 vs previous week (pinned blended)
- [emdash-cms/emdash](https://github.com/emdash-cms/emdash) — +0.04 vs previous week (pinned blended)
- [withastro/astro](https://github.com/withastro/astro) — +0.00 vs previous week (pinned blended)

## Biggest decreases vs previous week

- [garrytan/gstack](https://github.com/garrytan/gstack) — -0.38 vs previous week (pinned blended)
- [cloudflare/vinext](https://github.com/cloudflare/vinext) — -0.08 vs previous week (pinned blended)
- [modem-dev/hunk](https://github.com/modem-dev/hunk) — -0.03 vs previous week (pinned blended)
- [vitejs/vite](https://github.com/vitejs/vite) — -0.01 vs previous week (pinned blended)

## Notes

- `Trend (pinned)` is a mini sparkline of the repo's stored pinned-blended values across recent weekly points.
- Each repo stores one JSONL datapoint per UTC week; reruns in the same week replace that week's datapoint instead of appending duplicates.
- Older backfills can have fewer points for newer repos because the history job skips weeks before a repo had any commit on its current default branch.
- The existing pinned benchmark report remains the reproducible source of truth for exact SHA-based benchmark claims.
