# GitHub Actions runner prices (2026): per-minute rates for every hosted runner

Per-minute list prices for GitHub-hosted runners and the hosted services that replace them, at matched 2, 4 and 8 vCPU Linux x64 sizes. **Last checked 2026-11-07.** Every price was read from the provider's own pricing page on that date. Machine-readable copies: [`data/prices.json`](data/prices.json) and [`data/prices.csv`](data/prices.csv).


## Price per minute, Linux x64

| Runner | Hosting | 2 vCPU | 4 vCPU | 8 vCPU | vs GitHub at 2 vCPU |
|---|---|---|---|---|---|
| Sengi Basic | hosted | $0.001 | $0.002 | $0.004 | 83% less |
| Sengi Premium | hosted | $0.003 | $0.006 | $0.012 | 50% less |
| GitHub-hosted | hosted | $0.006 | $0.012 | $0.022 | — |
| Blacksmith | hosted | $0.004 | $0.008 | $0.016 | 33% less |
| WarpBuild | hosted | $0.004 | $0.008 | $0.016 | 33% less |
| Namespace | hosted | $0.006 | $0.012 | $0.024 | same |
| Depot | hosted | $0.006 | $0.012 | $0.024 | same |
| RunsOn | your own AWS account | $0.0009 | $0.0013 | $0.0021 | 85% less |
| Latchkey | hosted | $0.0025 | $0.005 | $0.01 | 58% less |
| StarSling | hosted | $0.004 | $0.008 | $0.016 | 33% less |
| Avrea | hosted | $0.004 | $0.008 | $0.016 | 33% less |
| compiler.dev | hosted | $0.002 | $0.004 | $0.008 | 67% less |
| BuildJet | shut down 2026-03-31 | — | — | — | — |

RunsOn runs in your own AWS account: its figure is spot compute plus its licence, not a hosted price. BuildJet stopped running jobs on 2026-03-31.

## What a month costs

List price before free or included usage.

| Runner | 3,000 min at 2 vCPU | 20,000 min at 4 vCPU | 100,000 min at 8 vCPU |
|---|---|---|---|
| Sengi Basic | $3 | $40 | $400 |
| Sengi Premium | $9 | $120 | $1,200 |
| GitHub-hosted | $18 | $240 | $2,200 |
| Blacksmith | $12 | $160 | $1,600 |
| WarpBuild | $12 | $160 | $1,600 |
| Namespace | $18 | $240 | $2,400 |
| Depot | $18 | $240 | $2,400 |
| RunsOn | $3 | $26 | $210 |
| Latchkey | $8 | $100 | $1,000 |
| StarSling | $12 | $160 | $1,600 |
| Avrea | $12 | $160 | $1,600 |
| compiler.dev | $6 | $80 | $800 |

## Runners priced another way

| Runner | Published prices per minute | Note |
|---|---|---|
| CRACI | 2 vCPU $0.004 | one published size (2 vCPU, 6 GB) |
| tempus.build | 2 vCPU $0.004, 4 vCPU $0.008 | no 8 vCPU price published |
| FlameWill | 2 vCPU $0.0009, 4 vCPU $0.0018, 8 vCPU $0.0048 | arm64 only, priced by memory (8, 16 and 32 GB) |
| Bitrise Build Hub | 4 vCPU $0.0125 |  |
| Cirrus Runners | not published per minute |  |
| Actuated | not published per minute |  |


## GitHub's included usage

GitHub plans include a dollar amount of Actions usage each month: $12 on Free, $18 on Pro and Team, $300 on Enterprise Cloud. Larger runners on Team and Enterprise Cloud draw on it at their own rate. Standard runners are free for public repositories.


## Method

- Linux x64 list prices at matched vCPU counts, in USD per minute, without volume discounts or commitments.
- Prices are read from each provider's public pricing page on the date above and re-checked when a provider changes them.

