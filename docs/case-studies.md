# Case Studies — Verified Results

This document presents OddsFlow Partners' track record, performance data, and
three anonymized case studies from real partner engagements. All statistics cited
are drawn from PDF-verified records with pre-match timestamps and post-match
settlement confirmation.

---

## Track Record Summary

### Overall Performance

| Metric | Value |
|---|---|
| **Overall verified win rate** | 56.8% |
| **Total tracked matches** | 10,000+ |
| **PDF-verified records** | 228+ |
| **Global bookmakers monitored** | 50+ |
| **Signal types** | 3 (HDP Sniper, Active Trader, Shield) |

### Performance by Signal Type

| Signal | Win Rate | Tracked Signals | Focus |
|---|---|---|---|
| **HDP Sniper** | 58.3% | 1,847 | Asian handicap line deviations |
| **Active Trader** | 55.1% | 3,241 | Coordinated market movements |
| **Shield** | 61.2% | 982 | Counter-consensus risk identification |

These win rates are measured across all tracked signals, not a cherry-picked
subset. Each signal is documented with pre-match conditions, fair-value context,
and post-match settlement outcome.

---

## Verification Methodology

OddsFlow Partners uses a four-step verification process designed to eliminate
survivorship bias and ensure that all published results are auditable.

### 1. Pre-Match PDF Generation

Before a match begins, OddsFlow generates a PDF document containing the signal
details: the identified anomaly, the fair-value benchmark at time of detection,
the bookmaker odds in question, the signal type and confidence level, and all
relevant market context. This PDF is generated automatically by the system — not
manually selected after the fact.

### 2. Immutable Timestamping

Each pre-match PDF receives a cryptographic timestamp that proves it existed
before the match started. This timestamp cannot be altered retroactively. The
combination of pre-match content and immutable timestamp ensures that the record
was created before the outcome was known.

### 3. Post-Match Settlement

After the match concludes, the system records the actual outcome and compares it
against the pre-match signal. Each signal is marked as correct or incorrect based
on the settlement result. There is no subjective judgment — settlement is binary
and determined by the match result.

### 4. Public Audit Trail

Verified records are accumulated into the public track record. The complete
dataset — including both correct and incorrect signals — is available for review.
This ensures full transparency: no selective reporting, no survivorship bias, no
omission of losing signals.

---

## Case Study 1: European Sportsbook Operator

### Client Profile

- **Type:** Multi-brand sportsbook operator
- **Scale:** 200,000+ registered users across 12 markets
- **Region:** Europe
- **Sports coverage:** Football, basketball, tennis, and 15+ secondary sports

### Challenge

The operator's risk team suspected that their Asian handicap pricing in lower-tier
European football leagues was slower to update than their major league pricing.
Manual spot checks were inconclusive — the team lacked the tooling to
systematically measure staleness across all markets at all times.

### Analysis

OddsFlow conducted a full Audit of the operator's pricing across all sports and
market types. The analysis covered a rolling 30-day window of live odds data
compared against the Shin-derived fair-value benchmark.

**Key findings:**

- **14.3% of Asian handicap lines** in Ligue 2 and Serie B were stale by 3+
  minutes at any given time during live play
- The estimated annual financial exposure from these stale lines was
  **EUR 180,000**, based on historical sharp-bettor exploitation rates for
  similar staleness windows
- **Three specific feed sources** were identified as the primary contributors to
  the latency, with one feed consistently updating 45-90 seconds behind the
  other two on lower-tier fixtures
- Major league pricing (Premier League, La Liga, Serie A top tier) showed no
  significant staleness — the issue was isolated to second-tier competitions

### Outcome

The operator used the OddsFlow report to renegotiate SLAs with two of the three
identified feed providers and switched the third. After implementing changes:

- **87% reduction in stale lines** within 60 days
- Stale-line percentage in Ligue 2 and Serie B dropped from 14.3% to under 2%
- Estimated annual exposure reduced from EUR 180,000 to under EUR 25,000
- **Composite quality score improved from 72 to 91**

The operator subsequently moved to the Monitor plan for ongoing surveillance and
is evaluating agent deployment for automated stale-line detection and response.

---

## Case Study 2: Asian Odds Feed Provider

### Client Profile

- **Type:** Mid-size odds feed provider
- **Scale:** 15+ sportsbook clients
- **Region:** Southeast Asia
- **Coverage:** Football, basketball, tennis, esports, and virtual sports

### Challenge

Two of the provider's largest clients had raised quality concerns and were
evaluating alternative feed providers. The clients cited "data quality issues"
but could not provide specific metrics. The provider needed an objective,
third-party assessment to understand the actual quality level and either fix
real issues or defend their product with evidence.

### Analysis

OddsFlow conducted a comprehensive feed quality benchmark across all sports and
market types in the provider's output. The analysis compared the provider's odds
against the Shin-derived fair-value benchmark from 50+ bookmakers.

**Key findings:**

- **Overall accuracy: 93.7%** — above the industry average and competitive with
  larger providers in the region
- Football and basketball feeds scored 95%+ on accuracy and latency
- **Tennis totals accuracy: 86.1%** — a significant weakness, particularly in
  WTA and lower-tier ATP tournaments where the provider's models updated slowly
  after set breaks
- **Esports totals accuracy: 86.4%** — similar weakness, with CS2 and Dota 2
  map totals showing inconsistent updates during live play
- All other metrics (latency, coverage, consistency, market depth) were at or
  above benchmark levels

### Outcome

The provider used the OddsFlow certification report in two ways:

1. **Client retention:** Shared the full report with the two at-risk clients,
   demonstrating that overall quality was above average and that the perceived
   issues were isolated to specific markets. Both clients renewed their
   contracts.
2. **Targeted improvement:** Invested in improving tennis and esports totals
   models specifically, using the OddsFlow benchmark as the success metric.
   Within 90 days, tennis totals accuracy improved from 86.1% to 92.8%.
3. **New client acquisition:** Used the certification in sales materials,
   winning three new sportsbook clients who cited the independent quality
   verification as a factor in their decision.

**Composite score: 88 at initial assessment, upgraded to Certified status after
targeted improvements.**

---

## Case Study 3: North American Digital Sportsbook

### Client Profile

- **Type:** Digital-first sportsbook operator
- **Scale:** Licensed in 3 US states, launched within the prior 18 months
- **Region:** North America
- **Sports focus:** NFL, NBA, MLB, NHL, and college sports

### Challenge

As a new entrant, the operator needed to understand how their pricing compared
to established competitors. Their internal team had built pricing models for the
four major US sports but lacked an independent benchmark. Anecdotally, they
believed their NFL and NBA pricing was competitive but were less confident about
MLB, NHL, and their expanding player props offering.

### Analysis

OddsFlow conducted an Audit across all of the operator's active sports and
market types, comparing their odds against the Shin-derived fair-value benchmark
and against the pricing of established US operators.

**Key findings:**

- **NFL and NBA:** Competitive pricing with deviation from fair value within
  normal ranges. No significant stale-line issues detected. The operator's
  models were performing well for these marquee sports.
- **MLB:** A consistent **+1.5% overround bias** was detected across run-line
  and totals markets. The operator was pricing MLB markets wider than consensus,
  which reduced competitiveness for price-sensitive bettors and indicated a
  model calibration issue.
- **NHL:** Similar overround bias on puck-line markets, though less pronounced
  than MLB (approximately +0.8% above consensus).
- **Player props:** The anomaly rate for player props was **3x the rate** of
  their standard markets. Specific issues included slow updates on in-game props
  and wider-than-market pricing on statistical props (assists, rebounds, hits).
  The player props model was identified as the highest-priority area for
  improvement.

### Outcome

The operator used the OddsFlow findings to prioritize model improvements:

1. **MLB recalibration:** Adjusted run-line and totals models to reduce overround
   bias, bringing pricing in line with market consensus within two weeks.
2. **Player props overhaul:** Invested in upgrading the player props pricing
   pipeline, focusing on update frequency and margin calibration. Anomaly rate
   decreased by 60% within 30 days.
3. **NHL adjustment:** Minor model tweaks to reduce puck-line overround. Changes
   implemented in the same cycle as MLB fixes.

**Composite quality score improved from 68 to 84 within 30 days of implementing
changes.**

The operator subsequently moved to the Integrate plan for ongoing API-based
monitoring and is evaluating the deployment of an Odds Monitoring agent for
automated anomaly detection across all markets.

---

## Credibility & Transparency

OddsFlow Partners is committed to transparent, verifiable reporting. The
following principles govern how results are documented and published.

### Pre-Match Timestamps

Every signal is documented before the match begins. Pre-match PDFs with
cryptographic timestamps prove that the analysis existed prior to the outcome
being known. This is the fundamental mechanism that prevents after-the-fact
selection of winning signals.

### Open Methodology

The Shin de-vig methodology, fair-value computation approach, and signal
classification criteria are documented publicly. The methodology is available on
the OddsFlow Partners GitHub repository for independent review and scrutiny. We
believe that transparent methods produce more trustworthy results than
proprietary black boxes.

### Downloadable Records

PDF-verified records are available for download and independent review. The
dataset includes both correct and incorrect signals — providing the complete
picture rather than a curated highlight reel.

### No Survivorship Bias

All signals generated by the system are included in the track record, regardless
of outcome. There is no selective removal of losing signals, no retroactive
adjustment of thresholds, and no post-hoc filtering. The 56.8% composite win
rate, the 58.3% HDP Sniper rate, the 55.1% Active Trader rate, and the 61.2%
Shield rate reflect the full, unfiltered dataset.

### Continuous Verification

The track record is not a one-time report — it is continuously updated as new
signals are generated and settled. Performance metrics reflect the most current
data available, including recent signals that may differ from historical
averages.

---

## Contact

To discuss how OddsFlow Partners can help your organization, or to request
access to detailed performance data:

- **Website:** [https://www.oddsflow-partners.com](https://www.oddsflow-partners.com)
- **Email:** support@oddsflow-partners.com
- **Telegram:** @oddsflowteam

---

*OddsFlow Partners — Verified odds intelligence for the sports betting industry.*
