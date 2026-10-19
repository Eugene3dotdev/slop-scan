# Rolling benchmark history: Known AI repos vs older solid OSS repos

Latest update: 2026-10-19
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

- `0.4.0` @ `f92bdd8` — 18 latest repo snapshots

## Latest cohort medians

| Cohort | Repo count | Median current blended | Median score/file | Median findings/file |
|---|---:|---:|---:|---:|
| explicit-ai | 9 | **4.47** | 1.24 | 0.33 |
| mature-oss | 9 | **1.00** | 0.19 | 0.07 |

## AI cohort latest standings

| Repo | Points | Trend (pinned) | Latest ref | Current blended | Latest pinned | Highest pinned | Δ prev (pinned) | Δ first (pinned) | Score/file | Findings/file |
|---|---:|---|---|---:|---:|---:|---:|---:|---:|---:|
| [redwoodjs/agent-ci](https://github.com/redwoodjs/agent-ci) | 31 | ██▁▁▁▁▁▁ | `main@c8597bb` | **5.63** | **9.01** | **9.62** | 0.00 | +5.10 | 1.33 | 0.40 |
| [jiayun/DevWorkbench](https://github.com/jiayun/DevWorkbench) | 31 | ▅▅▅▅▅▅▅▅ | `main@27f0d1a` | **5.62** | **8.99** | **8.99** | 0.00 | +5.59 | 1.26 | 0.47 |
| [garrytan/gstack](https://github.com/garrytan/gstack) | 31 | ██▇▃▂▃▂▁ | `main@6a4ab69` | **5.08** | **8.12** | **11.92** | -0.16 | +1.75 | 1.24 | 0.37 |
| [openclaw/openclaw](https://github.com/openclaw/openclaw) | 31 | ▁▃▄▇▇█▇▆ | `main@ae0ff9c` | **4.76** | **7.60** | **7.82** | -0.12 | +4.67 | 1.32 | 0.34 |
| [emdash-cms/emdash](https://github.com/emdash-cms/emdash) | 29 | ▁▂▃▆▇██▇ | `main@b82016d` | **4.18** | **6.68** | **6.72** | -0.02 | +4.50 | 1.25 | 0.32 |
| [cloudflare/vinext](https://github.com/cloudflare/vinext) | 31 | ▅▄█▇▄▅▃▁ | `main@183c2e6` | **2.28** | **3.64** | **4.11** | -0.07 | +1.65 | 0.45 | 0.13 |
| [modem-dev/hunk](https://github.com/modem-dev/hunk) | 31 | ▁▅▇▆▆▆▅█ | `main@5fb9926` | **2.24** | **3.58** | **3.59** | +0.11 | +2.78 | 0.54 | 0.19 |
| [FullAgent/fulling](https://github.com/FullAgent/fulling) | 31 | ▅▅▅▅▅▅▅▅ | `main@f48efce` | **1.65** | **2.64** | **10.28** | 0.00 | +0.48 | 0.20 | 0.05 |
| [robinebers/openusage](https://github.com/robinebers/openusage) | 31 | n/a | `main@26132ff` | **n/a** | **n/a** | **6.56** | n/a | n/a | n/a | n/a |

## Mature OSS cohort latest standings

| Repo | Points | Trend (pinned) | Latest ref | Current blended | Latest pinned | Highest pinned | Δ prev (pinned) | Δ first (pinned) | Score/file | Findings/file |
|---|---:|---|---|---:|---:|---:|---:|---:|---:|---:|
| [mikaelbr/node-notifier](https://github.com/mikaelbr/node-notifier) | 31 | ▁▁▁▁▁▁██ | `master@b50f939` | **1.68** | **2.68** | **2.68** | 0.00 | +2.27 | 0.26 | 0.13 |
| [withastro/astro](https://github.com/withastro/astro) | 31 | ▂▄▁▃▃▂█▆ | `main@48ec171` | **1.55** | **2.48** | **2.49** | -0.02 | +0.93 | 0.20 | 0.07 |
| [umami-software/umami](https://github.com/umami-software/umami) | 31 | ███▁▁▁▁▁ | `master@ec0ff50` | **1.41** | **2.26** | **2.35** | 0.00 | +1.21 | 0.25 | 0.07 |
| [vitejs/vite](https://github.com/vitejs/vite) | 31 | ▃▁▃▃▂▄▇█ | `main@467f7ac` | **1.34** | **2.14** | **2.14** | +0.01 | +0.62 | 0.16 | 0.05 |
| [payloadcms/payload](https://github.com/payloadcms/payload) | 31 | ▁▂▃▅▇▆██ | `main@d5b01b4` | **1.00** | **1.60** | **1.60** | 0.00 | +0.28 | 0.14 | 0.04 |
| [egoist/tsup](https://github.com/egoist/tsup) | 31 | ▁▁▁▁▁▁▁█ | `main@198479b` | **0.95** | **1.52** | **1.52** | +0.00 | +0.60 | 0.15 | 0.06 |
| [pmndrs/zustand](https://github.com/pmndrs/zustand) | 31 | ▅▅▅▅▅▅▅▅ | `main@d7a5583` | **0.83** | **1.33** | **1.38** | 0.00 | -0.05 | 0.19 | 0.08 |
| [sindresorhus/execa](https://github.com/sindresorhus/execa) | 31 | ▁▁▁▁▁▁▆█ | `main@e7e0664` | **0.82** | **1.31** | **1.31** | +0.11 | +0.42 | 0.12 | 0.03 |
| [vercel/hyper](https://github.com/vercel/hyper) | 31 | ▅▅▅▅▅▅▅▅ | `canary@30ec0a2` | **0.56** | **0.90** | **0.90** | 0.00 | +0.49 | 0.63 | 0.15 |

## Table legend

- `Current blended` = latest repo score vs the current mature-OSS medians from the same rolling run.
- `Latest pinned` = latest repo score vs the frozen pinned mature-OSS baseline snapshot.
- `Highest pinned` = highest stored repo score on that same pinned baseline.
- `Δ prev (pinned)` = latest pinned - previous week's pinned score.
- `Δ first (pinned)` = latest pinned - first stored pinned score for that repo.

## Biggest increases vs previous week

- [sindresorhus/execa](https://github.com/sindresorhus/execa) — +0.11 vs previous week (pinned blended)
- [modem-dev/hunk](https://github.com/modem-dev/hunk) — +0.11 vs previous week (pinned blended)
- [vitejs/vite](https://github.com/vitejs/vite) — +0.01 vs previous week (pinned blended)
- [egoist/tsup](https://github.com/egoist/tsup) — +0.00 vs previous week (pinned blended)

## Biggest decreases vs previous week

- [garrytan/gstack](https://github.com/garrytan/gstack) — -0.16 vs previous week (pinned blended)
- [openclaw/openclaw](https://github.com/openclaw/openclaw) — -0.12 vs previous week (pinned blended)
- [cloudflare/vinext](https://github.com/cloudflare/vinext) — -0.07 vs previous week (pinned blended)
- [emdash-cms/emdash](https://github.com/emdash-cms/emdash) — -0.02 vs previous week (pinned blended)
- [withastro/astro](https://github.com/withastro/astro) — -0.02 vs previous week (pinned blended)

## Notes

- `Trend (pinned)` is a mini sparkline of the repo's stored pinned-blended values across recent weekly points.
- Each repo stores one JSONL datapoint per UTC week; reruns in the same week replace that week's datapoint instead of appending duplicates.
- Older backfills can have fewer points for newer repos because the history job skips weeks before a repo had any commit on its current default branch.
- The existing pinned benchmark report remains the reproducible source of truth for exact SHA-based benchmark claims.
