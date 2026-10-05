# Rolling benchmark history: Known AI repos vs older solid OSS repos

Latest update: 2026-10-05
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

- `0.4.0` @ `afcdf09` — 18 latest repo snapshots

## Latest cohort medians

| Cohort | Repo count | Median current blended | Median score/file | Median findings/file |
|---|---:|---:|---:|---:|
| explicit-ai | 9 | **4.79** | 1.26 | 0.34 |
| mature-oss | 9 | **1.00** | 0.16 | 0.06 |

## AI cohort latest standings

| Repo | Points | Trend (pinned) | Latest ref | Current blended | Latest pinned | Highest pinned | Δ prev (pinned) | Δ first (pinned) | Score/file | Findings/file |
|---|---:|---|---|---:|---:|---:|---:|---:|---:|---:|
| [redwoodjs/agent-ci](https://github.com/redwoodjs/agent-ci) | 29 | ████▁▁▁▁ | `main@c8597bb` | **5.93** | **9.01** | **9.62** | 0.00 | +5.10 | 1.33 | 0.40 |
| [jiayun/DevWorkbench](https://github.com/jiayun/DevWorkbench) | 29 | ▅▅▅▅▅▅▅▅ | `main@27f0d1a` | **5.92** | **8.99** | **8.99** | 0.00 | +5.59 | 1.26 | 0.47 |
| [garrytan/gstack](https://github.com/garrytan/gstack) | 29 | ██▇▇▆▂▁▂ | `main@857466f` | **5.69** | **8.63** | **11.92** | +0.34 | +2.26 | 1.34 | 0.38 |
| [openclaw/openclaw](https://github.com/openclaw/openclaw) | 29 | ▁▁▃▄▅▇██ | `main@7879c7f` | **5.15** | **7.82** | **7.82** | +0.05 | +4.89 | 1.37 | 0.35 |
| [emdash-cms/emdash](https://github.com/emdash-cms/emdash) | 27 | ▁▂▂▃▄▆▇█ | `main@0a17191` | **4.43** | **6.72** | **6.72** | +0.05 | +4.55 | 1.27 | 0.32 |
| [cloudflare/vinext](https://github.com/cloudflare/vinext) | 29 | ▇▄▁▁█▅▁▁ | `main@448b5f3` | **2.49** | **3.78** | **4.11** | +0.01 | +1.79 | 0.48 | 0.14 |
| [modem-dev/hunk](https://github.com/modem-dev/hunk) | 29 | ▂▁▅▇████ | `main@1b7ceb5` | **2.30** | **3.48** | **3.59** | 0.00 | +2.68 | 0.54 | 0.19 |
| [FullAgent/fulling](https://github.com/FullAgent/fulling) | 29 | ▅▅▅▅▅▅▅▅ | `main@f48efce` | **1.74** | **2.64** | **10.28** | 0.00 | +0.48 | 0.20 | 0.05 |
| [robinebers/openusage](https://github.com/robinebers/openusage) | 29 | n/a | `main@256a9f1` | **n/a** | **n/a** | **6.56** | n/a | n/a | n/a | n/a |

## Mature OSS cohort latest standings

| Repo | Points | Trend (pinned) | Latest ref | Current blended | Latest pinned | Highest pinned | Δ prev (pinned) | Δ first (pinned) | Score/file | Findings/file |
|---|---:|---|---|---:|---:|---:|---:|---:|---:|---:|
| [withastro/astro](https://github.com/withastro/astro) | 29 | ▁▅▄█▃▆▇▅ | `main@7f78504` | **1.61** | **2.44** | **2.46** | -0.01 | +0.89 | 0.20 | 0.07 |
| [umami-software/umami](https://github.com/umami-software/umami) | 29 | ▁████▆▆▆ | `master@ec0ff50` | **1.49** | **2.26** | **2.35** | 0.00 | +1.21 | 0.25 | 0.07 |
| [vitejs/vite](https://github.com/vitejs/vite) | 29 | █▅▅▁▅▅▂▇ | `main@1003321` | **1.38** | **2.09** | **2.11** | +0.02 | +0.58 | 0.16 | 0.05 |
| [payloadcms/payload](https://github.com/payloadcms/payload) | 29 | ▁▁▃▄▄▆█▇ | `main@288b133` | **1.03** | **1.56** | **1.58** | -0.02 | +0.24 | 0.14 | 0.04 |
| [egoist/tsup](https://github.com/egoist/tsup) | 29 | ▅▅▅▅▅▅▅▅ | `main@b6bcae8` | **1.00** | **1.52** | **1.52** | 0.00 | +0.60 | 0.15 | 0.06 |
| [pmndrs/zustand](https://github.com/pmndrs/zustand) | 29 | ▅▅▅▅▅▅▅▅ | `main@d7a5583` | **0.88** | **1.33** | **1.38** | 0.00 | -0.05 | 0.19 | 0.08 |
| [sindresorhus/execa](https://github.com/sindresorhus/execa) | 29 | ▅▅▅▅▅▅▅▅ | `main@8017b27` | **0.65** | **0.98** | **1.10** | 0.00 | +0.09 | 0.09 | 0.02 |
| [mikaelbr/node-notifier](https://github.com/mikaelbr/node-notifier) | 29 | ▅▅▅▅▅▅▅▅ | `master@b36c237` | **0.62** | **0.95** | **0.95** | 0.00 | +0.53 | 0.08 | 0.04 |
| [vercel/hyper](https://github.com/vercel/hyper) | 29 | ▅▅▅▅▅▅▅▅ | `canary@30ec0a2` | **0.59** | **0.90** | **0.90** | 0.00 | +0.49 | 0.63 | 0.15 |

## Table legend

- `Current blended` = latest repo score vs the current mature-OSS medians from the same rolling run.
- `Latest pinned` = latest repo score vs the frozen pinned mature-OSS baseline snapshot.
- `Highest pinned` = highest stored repo score on that same pinned baseline.
- `Δ prev (pinned)` = latest pinned - previous week's pinned score.
- `Δ first (pinned)` = latest pinned - first stored pinned score for that repo.

## Biggest increases vs previous week

- [garrytan/gstack](https://github.com/garrytan/gstack) — +0.34 vs previous week (pinned blended)
- [emdash-cms/emdash](https://github.com/emdash-cms/emdash) — +0.05 vs previous week (pinned blended)
- [openclaw/openclaw](https://github.com/openclaw/openclaw) — +0.05 vs previous week (pinned blended)
- [vitejs/vite](https://github.com/vitejs/vite) — +0.02 vs previous week (pinned blended)
- [cloudflare/vinext](https://github.com/cloudflare/vinext) — +0.01 vs previous week (pinned blended)

## Biggest decreases vs previous week

- [payloadcms/payload](https://github.com/payloadcms/payload) — -0.02 vs previous week (pinned blended)
- [withastro/astro](https://github.com/withastro/astro) — -0.01 vs previous week (pinned blended)
- [modem-dev/hunk](https://github.com/modem-dev/hunk) — 0.00 vs previous week (pinned blended)

## Notes

- `Trend (pinned)` is a mini sparkline of the repo's stored pinned-blended values across recent weekly points.
- Each repo stores one JSONL datapoint per UTC week; reruns in the same week replace that week's datapoint instead of appending duplicates.
- Older backfills can have fewer points for newer repos because the history job skips weeks before a repo had any commit on its current default branch.
- The existing pinned benchmark report remains the reproducible source of truth for exact SHA-based benchmark claims.
