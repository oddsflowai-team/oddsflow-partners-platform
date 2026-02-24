# Technology — The Intelligence Engine

## End-to-End Pipeline

OddsFlow Partners operates a four-stage intelligence pipeline that transforms raw
bookmaker odds into actionable, auditable signals. Every stage is designed for
sub-second latency, full transparency, and rigorous statistical validation.

```
Data Ingestion → Fair-Value Engine → Signal Generation → Signal Delivery
```

---

## Stage 1: Data Ingestion

The pipeline begins with real-time odds collection from 50+ licensed bookmakers
across all major sports — football, basketball, baseball, hockey, tennis, MMA,
and more. Odds are ingested via direct API integrations and normalized into a
unified schema regardless of source format.

Key characteristics:

- **50+ bookmakers** monitored continuously
- **All major sports** and hundreds of leagues worldwide
- **Sub-second latency** from bookmaker update to pipeline entry
- **Normalized schema** — moneyline, spread, and totals standardized across
  regional formats (American, decimal, fractional)
- **Historical archive** — every odds movement is stored for backtesting and
  model calibration

---

## Stage 2: Fair-Value Engine

Raw bookmaker odds contain embedded margins (the "vig" or "juice") that distort
true probabilities. The Fair-Value Engine removes these margins using the Shin
de-vig methodology, then synthesizes probabilities from all sources into a single
ensemble fair-value estimate.

### Why Shin De-Vig

There are simpler methods for removing bookmaker margins — basic normalization,
multiplicative removal, power method. OddsFlow uses the Shin method because it
is the only approach that correctly models how bookmakers actually build their
margins.

The Shin model, based on the academic work of Hyun Song Shin, assumes that a
fraction of bettors are "insiders" with superior information. The bookmaker sets
margins asymmetrically — applying more margin to outcomes where insider activity
is likely and less to outcomes where it is not. Simpler methods assume margins are
applied uniformly, which produces systematically biased probability estimates.

The Shin method solves for the insider-trader parameter (z) that best explains
the observed odds, then uses that parameter to back out the true underlying
probabilities. This captures the margin asymmetry that other methods miss.

### Ensemble Approach

No single bookmaker has perfect information. OddsFlow aggregates de-vigged
probabilities from all 50+ sources into an ensemble estimate using weighted
averaging with dynamic calibration.

Weights are assigned based on each bookmaker's historical accuracy and market
influence. Sharp books (those known for setting efficient lines) receive higher
weights. Books that consistently lag the market or show systematic biases receive
lower weights. Weights are recalibrated on a rolling basis as bookmaker
performance evolves.

### Calibration and Validation

Fair-value estimates are validated continuously using multiple metrics:

- **Brier scores** — Measures the mean squared error between predicted
  probabilities and binary outcomes. Lower is better. OddsFlow's current
  aggregate Brier score is 0.187.
- **Log-loss** — Penalizes confident incorrect predictions more heavily than
  Brier scores, providing a complementary accuracy measure.
- **Reliability diagrams** — Visual calibration checks plotting predicted
  probability buckets against observed outcome frequencies. A perfectly
  calibrated model produces a 45-degree line.
- **Daily transparency reports** — Published calibration metrics broken down by
  sport, league, and bet type. Available to all partners and the public.

---

## Stage 3: Signal Generation

With fair-value probabilities established, statistical models compare each
bookmaker's current odds against the ensemble fair value. When discrepancies
exceed configurable thresholds, the system generates structured signals.

Signal generation also includes anomaly detection — identifying unusual patterns
such as sudden coordinated line movements across multiple books, odds that diverge
sharply from the consensus, or volume spikes that suggest informed money entering
the market.

---

## Stage 4: Signal Delivery

Signals reach consumers through multiple channels, each designed for different
use cases:

- **REST API** — Request-response interface for on-demand queries. Retrieve
  current fair values, active signals, historical performance, and agent
  reputation scores.
- **WebSocket** — Real-time streaming for latency-sensitive consumers. Receive
  signals the moment they are generated, with no polling overhead.
- **Dashboard** — Visual interface for human analysts. Charts, filters, and
  drill-downs for exploring signals, odds movements, and model performance.
- **Full audit trail** — Every signal includes a complete provenance chain:
  which bookmaker odds triggered it, what the fair value was at the time, which
  model generated it, and what confidence score was assigned.

---

## Model Performance

OddsFlow's models are validated against a large, independently verifiable dataset.

| Metric                | Value           |
| --------------------- | --------------- |
| Overall Win Rate      | 56.8%           |
| Sample Size           | 10,000+ bets    |
| PDF-Verified Records  | 228+            |
| Aggregate Brier Score | 0.187           |
| Bookmakers Monitored  | 50+             |

PDF-verified records refer to bet settlement confirmations exported directly from
sportsbook accounts — not self-reported results. These documents are available for
audit upon request.

---

## De-Vig Pipeline

The complete de-vig pipeline operates in six steps, running continuously for every
market across every sport.

```
1. Collect       Ingest raw odds from 50+ bookmakers in real time
      |
      v
2. Shin De-Vig   Apply Shin method per bookmaker to strip margins
      |
      v
3. Weight         Assign accuracy and influence weights to each source
      |
      v
4. Synthesize     Ensemble weighted average into single fair-value estimate
      |
      v
5. Compare        Measure each book's current odds against fair value
      |
      v
6. Signal         Generate scores, confidence levels, and structured signals
```

Each step is instrumented with latency tracking, error rates, and data quality
checks. If any source produces anomalous data (stale odds, malformed responses,
extreme outliers), it is automatically flagged and down-weighted until the issue
resolves.

---

## Three Signal Types

OddsFlow generates three distinct signal types, each targeting a different
market inefficiency.

### HDP Sniper

Detects Asian handicap deviations where one or more bookmakers have mispriced
the spread relative to the ensemble fair value. Asian handicap markets are
particularly susceptible to inefficiency because they require precise calibration
of the handicap line — small errors in line-setting create exploitable value.

| Metric       | Value           |
| ------------ | --------------- |
| Win Rate     | 58.3%           |
| Total Signals| 1,847           |
| Avg Edge     | 3.2%            |

### Active Trader

Identifies coordinated multi-book movements where several sportsbooks shift their
lines in the same direction within a short time window. These movements typically
indicate informed money entering the market and often precede further line
movement in the same direction.

| Metric       | Value           |
| ------------ | --------------- |
| Win Rate     | 55.1%           |
| Total Signals| 3,241           |
| Avg Edge     | 2.1%            |

### Shield

Generates counter-consensus risk alerts when the market consensus appears to be
wrong. Shield fires when OddsFlow's fair-value models strongly disagree with the
direction the market is moving — suggesting that the crowd is chasing a narrative
rather than following the data.

| Metric       | Value           |
| ------------ | --------------- |
| Win Rate     | 61.2%           |
| Total Signals| 982             |
| Avg Edge     | 4.7%            |

---

## Open Source

OddsFlow Partners is committed to transparency and open research. Core datasets,
model code, and research notebooks are published under the MIT license across
multiple platforms.

### GitHub

Repository: [github.com/oddsflowai-team](https://github.com/oddsflowai-team)

Source code for de-vig models, signal generation pipelines, backtesting
frameworks, and A2A protocol reference implementations. All repositories are
MIT licensed.

### Kaggle

Profile: [kaggle.com/oddsflow](https://www.kaggle.com/oddsflow)

Public datasets including historical odds snapshots, fair-value estimates, signal
archives, and model performance benchmarks. Updated regularly for the research
community.

### HuggingFace

Organization: [huggingface.co/Oddsflowai-team/oddsflow-transparency](https://huggingface.co/Oddsflowai-team/oddsflow-transparency)

Transparency reports, model documentation, and research publications for sports
betting AI research.

---

## Learn More

- [Agent Reputation Network](./agent-reputation.md) — Trust layer for AI agents
- [SportBot](./sportbot.md) — Autonomous betting agent built on this stack
- Website: [www.oddsflow-partners.com](https://www.oddsflow-partners.com)
- GitHub: [github.com/oddsflowai-team](https://github.com/oddsflowai-team)
- X: [@Oddsflow_Nat](https://x.com/Oddsflow_Nat)
- YouTube: [OddsflowAIPrediction](https://www.youtube.com/@OddsflowAIPrediction)
- Instagram: [oddsflow.ai](https://www.instagram.com/oddsflow.ai)
- Medium: [@oddsflow.ai](https://medium.com/@oddsflow.ai)
- Substack: [oddsflowai.substack.com](https://oddsflowai.substack.com)
