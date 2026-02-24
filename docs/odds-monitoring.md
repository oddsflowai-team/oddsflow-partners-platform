# Odds Monitoring — Real-Time Surveillance & Anomaly Detection

This document describes the odds monitoring capabilities of the OddsFlow Partners
platform, including real-time surveillance, fair-value computation, anomaly
detection, signal generation, and integration options.

---

## What Odds Monitoring Is

Odds monitoring is the continuous collection, normalization, and analysis of
betting odds across multiple bookmakers. Its purpose is to identify when an
individual bookmaker's odds deviate from fair value — whether due to stale
lines, mispricing, or suspicious market movements.

For sportsbooks, odds monitoring protects margins by catching pricing errors
before they are exploited. For feed providers, it provides an objective measure
of feed quality and accuracy.

---

## Why It Matters

Bookmaker odds are set independently and updated at different speeds. At any
given moment, some bookmakers will be mispriced relative to the true market.
These mispricings create risk:

- **For sportsbooks:** Stale or mispriced lines attract sharp bettors and
  arbitrageurs, eroding margins.
- **For feed providers:** Inaccurate or delayed feeds reduce client confidence
  and create downstream pricing errors.
- **For the market:** Undetected anomalies can indicate suspicious activity
  that warrants investigation.

Continuous monitoring surfaces these issues in real time, before they cause
material financial impact.

---

## How OddsFlow Monitors Odds

OddsFlow Partners ingests odds from 50+ global bookmakers across multiple
sports and market types. The monitoring pipeline operates as follows:

1. **Ingestion** — Raw odds are collected from bookmaker APIs and partner data
   connections. Data arrives continuously at sub-second intervals.
2. **Normalization** — Odds are converted to a common format (decimal odds and
   implied probabilities) and aligned by event, market type, and selection.
3. **Fair-value computation** — The Shin de-vig methodology strips bookmaker
   margins to compute true implied probabilities for each selection.
4. **Comparison** — Each bookmaker's odds are compared against fair value.
   Deviations are measured in standard deviations and implied probability gaps.
5. **Anomaly detection** — Statistical models evaluate whether deviations are
   within normal range or represent actionable anomalies.
6. **Signal generation** — Anomalies that meet predefined thresholds are
   classified by type, severity, and confidence.
7. **Delivery** — Signals and data are delivered via REST API, WebSocket
   streams, and the monitoring dashboard.

---

## Fair-Value Engine

### Shin De-Vig Methodology

The platform uses the Shin model to remove bookmaker overround (vig) from raw
odds. The Shin method accounts for the fact that bookmaker margins are not
applied uniformly across all outcomes — favorites carry less margin than
longshots. This produces more accurate implied probabilities than simpler
methods such as proportional margin removal.

The fair-value engine:

- Aggregates odds from all monitored bookmakers for each event and market
- Applies the Shin de-vig model to compute margin-free implied probabilities
- Weights bookmaker inputs based on historical accuracy and sharpness
- Updates fair values continuously as new odds data arrives
- Provides a neutral benchmark for measuring individual book pricing

The Shin model was developed specifically to address the favorite-longshot bias
in bookmaker pricing, making it more suitable for fair-value estimation in
sports betting markets than proportional de-vig approaches.

---

## Anomaly Detection

The anomaly detection layer sits on top of the fair-value engine. It uses
statistical models to determine whether a bookmaker's odds deviate from fair
value by more than expected.

### Stale Lines

A bookmaker's odds have not updated in response to market movements. The
platform tracks each bookmaker's last price update relative to fair-value
movement and flags lines that fail to respond within an expected window. Stale
lines are a primary target for arbitrage bettors and represent direct margin
erosion.

### Mispricing

A bookmaker's odds differ from fair value beyond normal margin variation.
Statistical comparison of implied probabilities against the Shin-derived fair
value flags deviations that exceed configurable thresholds.

### Suspicious Movements

Odds move in patterns inconsistent with normal market behavior — sudden large
movements at a single bookmaker, movements preceding public information, or
coordinated shifts across a small subset of books that diverge from the broader
market. Time-series analysis across all monitored bookmakers flags deviations
outside normal statistical bounds.

---

## Signal Types

When anomalies are detected, they are classified into one of three signal types.

### HDP Sniper

- **Target:** Asian handicap line deviations
- **Verified win rate:** 58.3%
- **Description:** Identifies mispricing in Asian handicap markets by comparing
  individual bookmaker lines against the Shin-derived fair value. Asian handicap
  markets are particularly susceptible to stale lines due to the granularity of
  half-goal and quarter-goal adjustments.

### Active Trader

- **Target:** Coordinated market movements
- **Verified win rate:** 55.1%
- **Description:** Detects coordinated odds movements across multiple bookmakers
  that indicate informed money entering the market. Signals are generated when
  cross-bookmaker correlation patterns exceed expected levels.

### Shield

- **Target:** Counter-consensus risk positions
- **Verified win rate:** 61.2%
- **Description:** Identifies situations where a bookmaker's position diverges
  materially from market consensus, indicating elevated risk exposure. Designed
  for defensive risk management — alerting sportsbooks to concentrated liability
  positions.

---

## Alert System

Each alert includes:

- **Signal type** — HDP Sniper, Active Trader, or Shield
- **Severity score** — Numeric rating based on deviation magnitude
- **Confidence interval** — Statistical confidence in the anomaly detection
- **Affected bookmaker(s)** — Which bookmaker(s) show the anomaly
- **Event details** — Sport, league, teams, market type, and kickoff time
- **Fair-value context** — Current fair value, bookmaker odds, and deviation size
- **Timestamp** — When the anomaly was detected

Severity scoring accounts for deviation magnitude, anomaly duration, number of
affected bookmakers, historical frequency, and estimated financial exposure.

### Delivery Channels

- **WebSocket** — Real-time push delivery, sub-100ms latency
- **REST API** — Polling-based access, sub-200ms response time
- **Dashboard** — Visual interface with filtering, sorting, and drill-down

---

## Historical Analysis

The platform maintains a historical database of odds movements and anomalies.

- **Pattern detection** — Identify recurring anomaly patterns for specific
  bookmakers, leagues, or market types over time
- **Bookmaker profiling** — Build accuracy and latency profiles for individual
  bookmakers based on historical performance
- **Trend analysis** — Track changes in feed quality or pricing accuracy across
  weeks and months
- **Backtesting** — Test detection thresholds and signal parameters against
  historical data

---

## Integration

### REST API

- Request-response access to current odds, fair values, signals, and history
- Sub-200ms response time, JSON format, API key authentication

### WebSocket

- Streaming real-time odds updates and alert notifications
- Sub-100ms delivery latency with automatic reconnection
- Filtered subscriptions by sport, league, bookmaker, or signal type

### Dashboard

- Browser-based monitoring with real-time odds comparison
- Alert feed, historical analysis tools, and bookmaker quality scorecards

---

## Use Cases

### For Sportsbooks

- **Line management** — Detect stale lines before exploitation by arbitrage
  and sharp action
- **Risk surveillance** — Monitor for suspicious movement patterns
- **Pricing validation** — Benchmark internal models against the fair-value engine
- **Automated response** — Connect alerts to line adjustment workflows via API

### For Feed Providers

- **Quality measurement** — Objective scoring of feed accuracy, latency, and
  coverage
- **Certification** — Independent third-party feed quality certification
- **Competitive benchmarking** — Compare feed performance to the broader market
- **Issue detection** — Early warning when feed quality degrades

---

## Contact

- **Website:** [https://www.oddsflow-partners.com](https://www.oddsflow-partners.com)
- **Email:** support@oddsflow-partners.com
- **Telegram:** @oddsflowteam
