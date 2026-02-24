# OddsFlow Partners Platform

[![Website](https://img.shields.io/badge/Website-oddsflow--partners.com-0A66C2?style=for-the-badge&logo=google-chrome&logoColor=white)](https://www.oddsflow-partners.com)
[![License: CC BY 4.0](https://img.shields.io/badge/Docs_License-CC_BY_4.0-lightgrey?style=for-the-badge)](https://creativecommons.org/licenses/by/4.0/)

---

**OddsFlow Partners** is an AI-powered odds intelligence and agentic AI infrastructure platform built for sportsbooks and odds feed providers. The platform delivers real-time odds monitoring across 50+ bookmakers, anomaly detection, feed quality auditing, custom AI agent development, an Agent-to-Agent (A2A) communication protocol, and an Agent Reputation Network that establishes trust between autonomous systems operating in the sports betting ecosystem.

> **Website:** [https://www.oddsflow-partners.com](https://www.oddsflow-partners.com)

### Who is this for?

- **Sportsbook operators** who need to protect margins, detect stale lines, and deploy autonomous risk management agents
- **Odds feed providers** who want independent quality certification, competitive benchmarking, and agent-ready data infrastructure
- **Trading desks** seeking AI-powered signal generation with verified win rates and transparent methodology
- **Technology teams** building agentic AI systems for the sports betting industry

---

## Table of Contents

- [Getting Started](#getting-started)
- [Key Stats](#key-stats)
- [The Three Pillars](#the-three-pillars)
  - [Odds Intelligence](#1-odds-intelligence)
  - [Agentic AI Infrastructure](#2-agentic-ai-infrastructure)
  - [Agent Reputation Network](#3-agent-reputation-network)
- [For Sportsbooks](#for-sportsbooks)
- [For Feed Providers](#for-feed-providers)
- [Agentic AI](#agentic-ai)
  - [Custom Agent Types](#custom-agent-types)
  - [Agent-to-Agent (A2A) Protocol](#agent-to-agent-a2a-protocol)
  - [SportBot](#sportbot)
- [Technology](#technology)
  - [Data Pipeline Architecture](#data-pipeline-architecture)
  - [Shin De-Vig Methodology](#shin-de-vig-methodology)
  - [Signal Types](#signal-types)
  - [Open Source](#open-source)
- [Security & Compliance](#security--compliance)
- [Pricing](#pricing)
  - [Platform Tiers](#platform-tiers)
  - [Agent Add-Ons](#agent-add-ons)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Ecosystem](#ecosystem)
- [Links & Contact](#links--contact)
- [Documentation Index](#documentation-index)
- [License](#license)

---

## Getting Started

The fastest path to value depends on your role:

**For Sportsbooks:**
1. Start with a **free Audit** -- a no-commitment assessment of your current line quality and market positioning
2. Review the audit report to identify margin leakage and pricing anomalies
3. Upgrade to **Monitor** ($499/mo) for continuous real-time tracking across up to 5 sports
4. Deploy your first AI agent with a 4-week **Agent POC** ($5,000 one-time)
5. Scale to **Integrate** ($2,499/mo) for full API access and all signal types

**For Feed Providers:**
1. Start with a **free Audit** -- an independent quality assessment of your feed against fair-value benchmarks
2. Use the audit results to identify accuracy gaps and freshness bottlenecks
3. Upgrade to **Monitor** ($499/mo) for continuous quality tracking and automated reporting
4. Earn **OddsFlow Quality Certification** with PDF reports and a live embeddable badge
5. Deploy a **Data Verification Agent** to automate quality assurance in production

**For Agent Builders:**
1. Review the [Agent-to-Agent Protocol documentation](./docs/agent-protocol.md)
2. Explore open-source examples on [GitHub](https://github.com/oddsflow-ai)
3. Contact us for a discovery session to scope your custom agent requirements
4. Receive a working POC in 4 weeks; move to production in 8 weeks

> Contact [support@oddsflow-partners.com](mailto:support@oddsflow-partners.com) or reach us on Telegram [@oddsflowteam](https://t.me/oddsflowteam) to get started.

---

## Key Stats

| Metric | Value |
|---|---|
| **Bookmaker Sources** | 50+ global |
| **API Latency** | Sub-200ms (REST), Sub-100ms (WebSocket) |
| **Verified Win Rate** | 56.8% across 10,000+ matches |
| **PDF-Verified Records** | 228+ pre-match timestamped |
| **Brier Score** | 0.187 |
| **Signal Types** | HDP Sniper (58.3%), Active Trader (55.1%), Shield (61.2%) |

All win rates are independently verifiable through timestamped PDF records generated before match kick-off. The Brier Score of 0.187 indicates well-calibrated probabilistic forecasting that outperforms the majority of publicly benchmarked models in the sports prediction domain.

---

## The Three Pillars

OddsFlow Partners is built on three interconnected pillars that together deliver a complete intelligence and automation layer for the sports betting industry.

### 1. Odds Intelligence

AI-powered odds monitoring, anomaly detection, and quality scoring aggregated from 50+ global bookmakers. The intelligence layer transforms raw odds data into actionable insights through:

- **Real-Time Monitoring**: Continuous tracking of odds movements across all major bookmakers with sub-second update detection.
- **Anomaly Detection**: Machine learning models identify pricing anomalies, stale lines, and market inefficiencies the moment they appear.
- **Quality Scoring**: Every odds update is scored for accuracy, freshness, and reliability against fair-value benchmarks.
- **Shin De-Vig Methodology**: Proprietary implementation of the Shin model strips bookmaker margins to reveal true implied probabilities, solving for the insider-trader parameter to produce the most accurate fair-value estimates.
- **Ensemble ML Models**: Multiple model architectures (gradient boosting, neural networks, Bayesian approaches) are combined through ensemble weighted averaging to maximize prediction accuracy and calibration.

The Odds Intelligence layer serves as the foundation for all downstream products, feeding cleaned and enriched data into signal generation, agent decision-making, and feed quality auditing systems.

### 2. Agentic AI Infrastructure

Custom AI agent development with six specialized agent types purpose-built for the sports betting industry. The infrastructure enables both sportsbooks and feed providers to deploy autonomous agents that operate continuously without human intervention:

- **Six Agent Types**: Odds Monitoring Agent, Risk Assessment Agent, Trading Assistant Agent, Compliance Agent, Data Verification Agent, and A2A Gateway Agent.
- **Agent-to-Agent Protocol**: A structured communication protocol enabling machine-to-machine exchange between agents, with mutual verification, reputation-based trust scoring, and full audit trails.
- **Rapid Deployment**: Proof of concept delivered in 4 weeks; full production deployment in 8 weeks.
- **Custom Development**: Every agent is tailored to the partner's specific data feeds, risk parameters, regulatory requirements, and operational workflows.

The Agentic AI Infrastructure is designed for enterprises that need autonomous systems operating around the clock, making decisions at machine speed while maintaining full compliance and auditability.

### 3. Agent Reputation Network

A trust layer for AI agents operating across the sports betting ecosystem. The Agent Reputation Network provides a standardized framework for evaluating and scoring the reliability of autonomous agents, ensuring that partners can trust the agents they interact with.

**Five Evaluation Dimensions:**

| Dimension | Weight | Description |
|---|---|---|
| **Accuracy** | 30% | Correctness of agent outputs, predictions, and recommendations measured against verified outcomes |
| **Consistency** | 25% | Reliability and stability of agent behavior over time, including uptime and response uniformity |
| **Transparency** | 20% | Quality of reasoning explanations, audit trail completeness, and decision traceability |
| **Response Quality** | 15% | Timeliness, format compliance, and completeness of agent communications |
| **Peer Validation** | 10% | Cross-validation scores from other agents in the network, weighted by their own reputation |

**Three Reputation Tiers:**

| Tier | Score Range | Benefits |
|---|---|---|
| **Verified** | 50 - 74 | Basic participation in the network, standard communication privileges |
| **Trusted** | 75 - 89 | Priority routing, expanded data access, reduced verification overhead |
| **Elite** | 90+ | Full network privileges, preferred partner status, direct A2A connections |

Reputation scores are computed continuously and updated in real time as new interaction data flows through the network. Agents that consistently perform well earn higher trust scores, unlocking additional capabilities and reducing friction in inter-agent communications.

---

## For Sportsbooks

OddsFlow Partners provides sportsbooks with a comprehensive intelligence and automation layer that protects margins, detects risk, and enables autonomous operations. Here is what the platform delivers for sportsbook operators:

### Real-Time Line Protection

- **Detect stale lines and pricing anomalies in real time.** The platform continuously compares your live lines against fair-value benchmarks derived from 50+ bookmakers. When a line goes stale or deviates beyond configurable thresholds, alerts fire within milliseconds.
- **Quantify liability exposure from mispriced markets.** Every anomaly is accompanied by an exposure estimate that quantifies the potential financial impact, allowing risk teams to prioritize responses based on dollar exposure rather than arbitrary alert severity.

### Market Intelligence

- **Market efficiency scoring with competitive positioning.** See exactly where your lines rank against the broader market. Efficiency scores reveal whether you are leading, lagging, or in line with consensus pricing across every sport and market type.
- **Risk intelligence with sharp-money flow indicators.** Track where sophisticated bettors are placing their money. Sharp-money flow analysis identifies markets where informed action is concentrated, giving trading desks advance warning of impending line movements.

### Integration Options

OddsFlow Partners supports three integration pathways tailored to different operational needs:

| Integration Type | Latency | Description |
|---|---|---|
| **API Overlay** | Sub-100ms | Lightweight integration that overlays intelligence on top of existing trading systems via REST or WebSocket APIs |
| **White-Label** | Configurable | Fully branded dashboards and alerting systems deployed under the sportsbook's own identity |
| **Custom POC** | 4 weeks | Proof of concept engagement tailored to specific data feeds, sports, and risk parameters |

### Deployable AI Agents for Sportsbooks

Sportsbooks can deploy the following AI agents through the OddsFlow Agentic AI Infrastructure:

1. **Odds Monitoring Agent**: Continuously tracks odds movements across 50+ bookmakers, detects anomalies, and alerts trading desks to stale lines and pricing outliers in real time.
2. **Risk Assessment Agent**: Evaluates liability exposure across active markets, flags mispriced lines based on fair-value deviation, and recommends position adjustments.
3. **Trading Assistant Agent**: Provides automated trading recommendations based on market consensus, sharp-money signals, and ensemble model outputs. Supports semi-automated and fully autonomous trading modes.
4. **Compliance Agent**: Monitors trading activity for regulatory compliance, generates audit reports, and ensures that all automated decisions meet jurisdictional requirements.

Each agent is custom-configured to the sportsbook's specific operational environment and can communicate with other agents via the A2A protocol.

---

## For Feed Providers

OddsFlow Partners enables odds feed providers to measure, certify, and improve their data quality through independent, quantitative benchmarking. The platform serves as both a quality assurance tool and a competitive differentiator for feed providers.

### Feed Quality Measurement

- **Measure feed quality against fair-value benchmarks.** Every odds update in your feed is compared against OddsFlow's fair-value engine, which aggregates and de-vigs data from 50+ bookmakers. The result is an objective, quantitative assessment of your feed's accuracy.
- **Per-update accuracy and freshness scores.** Each individual odds update receives an accuracy score (deviation from fair value) and a freshness score (latency from market movement to feed delivery). These granular metrics roll up into aggregate quality indicators.

### Third-Party Quality Certification

- **Independent quality certification with PDF reports, live badge, and dashboards.** Feed providers can earn OddsFlow Quality Certification, which includes:
  - **PDF Reports**: Detailed, timestamped quality reports suitable for sharing with clients and regulators.
  - **Live Badge**: An embeddable quality badge that displays real-time certification status on the provider's website.
  - **Dashboards**: Interactive dashboards showing historical quality trends, sport-by-sport breakdowns, and competitive comparisons.

### Sample Quality Metrics

A feed provider operating at industry-leading standards would display metrics such as:

| Metric | Score | Description |
|---|---|---|
| **Accuracy** | 94.2% | Percentage of odds updates within acceptable deviation from fair value |
| **Freshness** | A+ | Latency grade based on time-to-reflect market movements |
| **Coverage** | 98.7% | Percentage of available markets included in the feed |
| **Anomaly Rate** | 0.3% | Percentage of updates flagged as anomalous or potentially erroneous |

### Agent-Ready Feed Infrastructure

OddsFlow Partners ensures that feed providers' data is optimized for consumption by AI agents. This includes structured data formatting, real-time streaming compatibility, and metadata enrichment that agents need to make autonomous decisions.

### Deployable AI Agents for Feed Providers

Feed providers can deploy the following AI agents through the OddsFlow Agentic AI Infrastructure:

1. **Data Verification Agent**: Continuously validates incoming odds data against fair-value benchmarks, flags anomalies, and triggers correction workflows automatically.
2. **Quality Monitoring Agent**: Tracks feed quality metrics in real time, generates quality reports, and alerts operations teams when metrics drop below defined thresholds.
3. **Compliance Agent**: Ensures feed data meets regulatory standards across jurisdictions, generates compliance documentation, and maintains audit trails for all data operations.
4. **A2A Gateway Agent**: Serves as the interface between the feed provider's internal systems and external agents in the OddsFlow network, handling authentication, reputation verification, and structured data exchange.

Each agent integrates directly with the feed provider's existing infrastructure and can be deployed incrementally, starting with a single agent and expanding as confidence grows.

---

## Agentic AI

The OddsFlow Agentic AI platform enables partners to build, deploy, and manage autonomous AI agents tailored to the sports betting industry. These agents operate continuously, make decisions at machine speed, and communicate with each other through standardized protocols.

### Custom Agent Types

OddsFlow supports six specialized agent types, each designed for a specific operational domain:

| Agent Type | Primary Function | Typical Deployer |
|---|---|---|
| **Odds Monitoring Agent** | Real-time odds tracking, anomaly detection, stale-line alerts | Sportsbooks |
| **Risk Assessment Agent** | Liability evaluation, exposure quantification, position recommendations | Sportsbooks |
| **Trading Assistant Agent** | Automated trading recommendations, semi-auto and full-auto modes | Sportsbooks |
| **Compliance Agent** | Regulatory monitoring, audit reporting, jurisdictional compliance | Both |
| **Data Verification Agent** | Feed validation, anomaly flagging, correction workflows | Feed Providers |
| **Quality Monitoring Agent** | Quality metric tracking, reporting, threshold alerting | Feed Providers |

All agent types share a common architecture that includes:

- **Configurable decision thresholds** tuned to the partner's risk appetite
- **Full audit logging** of every decision, input, and output
- **Graceful degradation** to human-in-the-loop mode when confidence is low
- **Real-time monitoring dashboards** showing agent health, decision rates, and outcomes

### Agent-to-Agent (A2A) Protocol

The Agent-to-Agent protocol is a structured communication framework that enables machine-to-machine interaction between autonomous agents in the OddsFlow ecosystem. The protocol is built on four core principles:

1. **Structured Exchange**: All inter-agent communication follows a defined schema with typed fields, versioned message formats, and mandatory metadata. This ensures that agents from different partners can communicate without ambiguity.

2. **Mutual Verification**: Before any data exchange occurs, both agents verify each other's identity and authorization level through cryptographic handshakes. This prevents unauthorized agents from accessing sensitive data or issuing commands.

3. **Reputation-Based Trust**: Communication privileges are modulated by each agent's reputation score in the Agent Reputation Network. Higher-reputation agents receive priority routing, expanded data access, and reduced verification overhead.

4. **Audit Trail**: Every inter-agent interaction is logged with full context, including message payloads, timestamps, sender and receiver identities, reputation scores at time of interaction, and outcome tracking. These audit trails are immutable and available for regulatory review.

**Example A2A Message Flow:**

```
Agent A (Sportsbook Risk)          Agent B (Feed Verification)
         |                                    |
         |  1. Identity + Reputation Request  |
         |----------------------------------->|
         |                                    |
         |  2. Verified Identity + Score: 87  |
         |<-----------------------------------|
         |                                    |
         |  3. Odds Verification Query        |
         |     (event_id, market, timestamp)  |
         |----------------------------------->|
         |                                    |
         |  4. Verification Response          |
         |     (status, fair_value, delta)    |
         |<-----------------------------------|
         |                                    |
         |  5. Acknowledgment + Audit Hash    |
         |----------------------------------->|
         |                                    |
```

The A2A protocol enables use cases such as:

- A sportsbook's Risk Assessment Agent querying a feed provider's Data Verification Agent to confirm odds accuracy before adjusting lines
- Multiple Odds Monitoring Agents sharing anomaly alerts across the network to provide earlier warning of market-wide pricing events
- Compliance Agents from different jurisdictions coordinating to ensure cross-border regulatory alignment
- A Trading Assistant Agent requesting real-time fair-value confirmations from multiple Data Verification Agents before executing automated trades

### SportBot

**SportBot** (also known as **ClawSportBot**) is an autonomous betting agent that demonstrates the full capabilities of the OddsFlow Agentic AI platform. SportBot operates independently, making betting decisions based on the OddsFlow Odds Intelligence layer without human intervention.

- **Website**: [https://clawsportbot.io](https://clawsportbot.io)
- **Functionality**: Autonomous pre-match betting across multiple sports and markets
- **Decision Engine**: Powered by OddsFlow ensemble ML models and Shin de-vig fair-value estimates
- **Track Record**: All bets are timestamped and recorded in PDF format before match kick-off, providing a fully verifiable performance record
- **Purpose**: Serves as both a production agent and a reference implementation for partners building their own autonomous agents on the OddsFlow platform

SportBot is a live demonstration that AI agents can operate profitably and transparently in the sports betting domain, with every decision traceable and every outcome verifiable.

### Agent Development Lifecycle

Every custom agent engagement follows a structured development lifecycle:

| Phase | Duration | Deliverables |
|---|---|---|
| **Discovery** | Week 1 | Requirements document, data source mapping, success metrics definition |
| **Design** | Week 2 | Agent architecture, decision logic specification, integration plan |
| **Development** | Weeks 2-3 | Working agent with core logic, unit tests, integration tests |
| **Testing** | Week 3-4 | Backtesting against historical data, shadow-mode deployment alongside human operators |
| **Pilot** | Weeks 4-6 | Live deployment with monitoring, human-in-the-loop oversight, performance measurement |
| **Production** | Weeks 6-8 | Full autonomous deployment, alerting, dashboards, ongoing maintenance |

Partners retain full ownership of their custom agents, including all configuration, decision logic, and training data. OddsFlow provides the infrastructure, tooling, and ongoing support.

---

## Technology

### Data Pipeline Architecture

The OddsFlow data pipeline processes odds data from ingestion to delivery through four stages:

```
Data Ingestion  -->  Fair-Value Engine  -->  Signal Generation  -->  Delivery
     |                     |                       |                    |
  50+ bookmakers     Shin de-vig            ML ensemble models    REST / WebSocket
  Raw odds feeds     Margin stripping       Anomaly detection     Sub-200ms REST
  Market metadata    True probability       Signal scoring        Sub-100ms WS
  Event data         Insider parameter      Confidence levels     Push notifications
```

**Stage 1 -- Data Ingestion**

Raw odds data is collected from 50+ global bookmakers in real time. The ingestion layer normalizes heterogeneous data formats into a unified schema, handles deduplication, and enriches each update with market metadata (sport, league, event, market type, timestamp). Key capabilities of the ingestion layer include:

- **Format Normalization**: Converts American, decimal, fractional, and Asian odds formats into a unified internal representation
- **Deduplication**: Identifies and removes duplicate updates from overlapping data sources
- **Metadata Enrichment**: Attaches sport, league, event, market type, and temporal metadata to every update
- **Source Health Monitoring**: Tracks the availability, latency, and data quality of each bookmaker source in real time

**Stage 2 -- Fair-Value Engine (Shin De-Vig)**

The core pricing engine applies the Shin de-vig methodology to strip bookmaker margins and produce true implied probabilities. This stage is described in detail in the next section.

**Stage 3 -- Signal Generation**

Ensemble machine learning models analyze the de-vigged probabilities and market dynamics to generate trading signals. Each signal includes a type classification, confidence score, expected value estimate, and recommended position size. Three primary signal types are produced (detailed below).

**Stage 4 -- Delivery**

Signals and data are delivered to partners and agents through multiple channels:

- **REST API**: Sub-200ms latency, suitable for polling-based integrations and batch queries
- **WebSocket API**: Sub-100ms latency, suitable for real-time streaming and agent consumption
- **Push Notifications**: Configurable alerts delivered via webhook, email, or Telegram
- **Dashboard**: Interactive web interface for visual monitoring and manual analysis

### Shin De-Vig Methodology

The Shin de-vig methodology is the cornerstone of OddsFlow's fair-value estimation. Named after the academic work of Hyun Song Shin, this approach provides a principled method for removing bookmaker margins from published odds to reveal the true implied probabilities of sporting outcomes.

**How it works:**

1. **Margin Stripping**: Published odds from each bookmaker include an overround (margin) that ensures the bookmaker's profit. The Shin model identifies and removes this overround mathematically rather than through naive proportional scaling.

2. **Insider-Trader Parameter**: The Shin model introduces a parameter (z) that represents the estimated proportion of bets placed by insiders -- bettors with superior information. Solving for this parameter produces probability estimates that account for the information asymmetry inherent in betting markets.

3. **Ensemble Weighted Averaging**: After de-vigging odds from each individual bookmaker, OddsFlow applies ensemble weighted averaging across all 50+ sources. Weights are assigned based on each bookmaker's historical accuracy, market depth, and update frequency. The result is a consensus fair-value estimate that is more accurate than any single bookmaker's line.

The Shin de-vig methodology produces probability estimates with a Brier Score of 0.187, indicating strong calibration. For context, a Brier Score of 0.0 represents perfect prediction and 0.25 represents uninformative prediction. The OddsFlow score of 0.187 demonstrates meaningful predictive skill across a large sample of 10,000+ verified matches.

### Signal Types

OddsFlow generates three primary signal types, each designed for a different trading strategy and risk profile:

#### HDP Sniper

| Attribute | Detail |
|---|---|
| **Win Rate** | 58.3% |
| **Strategy** | Identifies Asian Handicap mispricing by detecting discrepancies between fair-value handicap lines and bookmaker offerings |
| **Trigger** | Fires when the fair-value handicap deviates from published lines by more than a configurable threshold (default: 0.25 goals) |
| **Best For** | Partners seeking high-frequency, moderate-edge trading opportunities in handicap markets |
| **Time Horizon** | Pre-match, typically 1-24 hours before kick-off |

#### Active Trader

| Attribute | Detail |
|---|---|
| **Win Rate** | 55.1% |
| **Strategy** | Follows sharp-money movements and market momentum, identifying markets where informed bettors are driving line changes |
| **Trigger** | Fires when statistically significant line movement is detected across multiple bookmakers within a short time window |
| **Best For** | Partners who want to align with market consensus and capitalize on information cascades |
| **Time Horizon** | Pre-match, typically 0-6 hours before kick-off |

#### Shield

| Attribute | Detail |
|---|---|
| **Win Rate** | 61.2% |
| **Strategy** | Defensive signal designed to protect against adverse outcomes by identifying markets with asymmetric risk profiles |
| **Trigger** | Fires when the model detects a high probability of a one-sided outcome that the market has not fully priced in |
| **Best For** | Risk-averse partners seeking high-confidence, lower-frequency signals with strong expected value |
| **Time Horizon** | Pre-match, typically 6-48 hours before kick-off |

All signals include:

- **Confidence score** (0-100) indicating the model's conviction level
- **Expected value estimate** quantifying the projected edge
- **Recommended stake** based on Kelly criterion position sizing
- **Supporting data** including the specific bookmakers, market movements, and model inputs that generated the signal

### Open Source

OddsFlow is committed to transparency and community contribution. Selected algorithms, datasets, and models are published on open platforms:

| Platform | URL | Content |
|---|---|---|
| **GitHub** | [github.com/oddsflow-ai](https://github.com/oddsflow-ai) | Open source algorithms, Shin de-vig implementations, signal generation code, and integration examples |
| **Kaggle** | [kaggle.com/oddsflowai](https://kaggle.com/oddsflowai) | Historical odds datasets, prediction competition notebooks, and benchmarking datasets |
| **HuggingFace** | [huggingface.co/oddsflow-ai](https://huggingface.co/oddsflow-ai) | Pre-trained model weights for odds prediction, anomaly detection, and market classification |

The open-source materials are intended for research, education, and community benchmarking. Partners who want production-grade implementations with real-time data, SLAs, and support should use the commercial platform.

---

## Security & Compliance

OddsFlow Partners operates in a regulated industry and takes data security and compliance seriously.

### Data Security

- **Encryption in Transit**: All API communications are encrypted using TLS 1.3. WebSocket connections use WSS (WebSocket Secure) exclusively.
- **Encryption at Rest**: All stored data, including odds histories, agent logs, and partner configurations, is encrypted at rest using AES-256.
- **Access Control**: Role-based access control (RBAC) ensures that each partner user can only access data and agents they are authorized to manage.
- **API Authentication**: All API access requires token-based authentication with configurable expiration and rotation policies.

### Compliance Features

- **Audit Trails**: Every agent decision, every inter-agent communication, and every data access event is logged with immutable audit trails.
- **Regulatory Reporting**: Automated report generation for jurisdictional compliance requirements, including responsible gambling obligations.
- **Data Retention**: Configurable data retention policies that comply with local regulations, with automated purging for expired data.
- **Geographic Restrictions**: Configurable geo-fencing to ensure that data and agent operations comply with jurisdictional boundaries.

### Agent Safety

- **Decision Boundaries**: Every agent operates within configurable decision boundaries that prevent unauthorized or excessive actions.
- **Human-in-the-Loop**: All agents support graceful degradation to human oversight when confidence drops below configured thresholds.
- **Kill Switch**: Operators can immediately halt any agent through the management dashboard or API.
- **Rollback**: Agent configurations can be rolled back to any previous version with full state recovery.

---

## Pricing

### Platform Tiers

| Feature | Audit | Monitor | Integrate | Enterprise |
|---|---|---|---|---|
| **Price** | Free | $499/mo | $2,499/mo | Custom |
| | One-time assessment | Continuous monitoring | Full API access | White-label & on-premise |
| **Sports Coverage** | One-time snapshot | Up to 5 sports | Unlimited sports | Unlimited sports |
| **Odds Monitoring** | Point-in-time | Real-time | Real-time | Real-time |
| **Anomaly Detection** | Included in report | Continuous | Continuous | Continuous |
| **Quality Scoring** | Included in report | Continuous | Continuous | Continuous |
| **API Access (REST)** | -- | Read-only | Full access | Full access |
| **API Access (WebSocket)** | -- | -- | Full access | Full access |
| **Trading Signals** | -- | -- | All signal types | All signal types |
| **Custom Dashboards** | -- | -- | Configurable | Fully branded |
| **PDF Reports** | Single report | Monthly | Weekly | On-demand |
| **Live Quality Badge** | -- | -- | Included | Included |
| **Dedicated Support** | Email | Email + Telegram | Priority | 24/7 dedicated |
| **SLA** | -- | 99.5% uptime | 99.9% uptime | 99.99% uptime |
| **On-Premise Deployment** | -- | -- | -- | Available |
| | | | **Most Popular** | |

> **Audit** is designed for feed providers and sportsbooks that want a no-commitment quality assessment before engaging further. There is no credit card required and no ongoing obligation.

> **Monitor** is ideal for operations teams that need continuous visibility into feed quality or market positioning across a focused set of sports.

> **Integrate** is the most popular tier and provides full programmatic access to the OddsFlow intelligence layer, including real-time signals, WebSocket streaming, and all signal types.

> **Enterprise** is for organizations that require white-label deployments, on-premise installations, custom SLAs, and dedicated 24/7 support.

### Agent Add-Ons

Agent capabilities can be added to any platform tier (Monitor and above):

| Add-On | Price | Description |
|---|---|---|
| **Agent POC** | $5,000 one-time | Proof of concept for a single custom agent, delivered in 4 weeks. Includes requirements gathering, development, testing, and a 2-week pilot period. |
| **Agent Integration** | $3,999/mo | Production deployment and ongoing operation of custom agents. Includes monitoring, maintenance, updates, and A2A protocol access. |
| **Agent Enterprise** | Custom | Multi-agent deployments, custom A2A protocol configurations, dedicated agent infrastructure, and SLA-backed agent uptime guarantees. |

All agent engagements begin with a discovery session to define requirements, data sources, decision boundaries, and success metrics.

---

## Frequently Asked Questions

### 1. What is OddsFlow Partners?

OddsFlow Partners is an AI-powered odds intelligence and agentic AI infrastructure platform designed for sportsbooks and odds feed providers. It provides real-time odds monitoring across 50+ bookmakers, anomaly detection, feed quality auditing, custom AI agent development, an Agent-to-Agent communication protocol, and an Agent Reputation Network. The platform helps sportsbooks protect margins and optimize pricing, while helping feed providers certify and improve their data quality. Visit [oddsflow-partners.com](https://www.oddsflow-partners.com) to learn more.

### 2. What tools exist for real-time odds monitoring?

OddsFlow Partners provides a comprehensive real-time odds monitoring solution that tracks lines across 50+ global bookmakers with sub-100ms WebSocket latency. The monitoring layer detects stale lines, pricing anomalies, and market inefficiencies as they occur. Beyond basic monitoring, OddsFlow applies Shin de-vig methodology to calculate fair-value benchmarks, enabling partners to see not just what the market is doing, but where the market is mispriced. Monitoring is available through REST API, WebSocket streaming, interactive dashboards, and autonomous AI agents.

### 3. How does Shin de-vig methodology work?

The Shin de-vig methodology removes bookmaker margins from published odds to reveal true implied probabilities. It works in three steps: first, it strips the overround (margin) that bookmakers build into their odds. Second, it solves for the Shin insider-trader parameter (z), which represents the estimated proportion of bets placed by insiders with superior information. Third, OddsFlow applies ensemble weighted averaging across all 50+ bookmaker sources, weighting each by historical accuracy, market depth, and update frequency. The result is a consensus fair-value estimate with a verified Brier Score of 0.187 across 10,000+ matches.

### 4. How do sportsbooks use AI for risk management?

Sportsbooks use OddsFlow's AI infrastructure in several ways: real-time anomaly detection alerts trading desks to stale lines and mispriced markets before they can be exploited. Liability exposure quantification calculates the dollar impact of pricing errors across all active markets. Sharp-money flow indicators track where sophisticated bettors are concentrating their action. Autonomous AI agents (Risk Assessment Agent, Trading Assistant Agent) can operate continuously to evaluate and respond to risk without human intervention. Integration options range from lightweight API overlays to fully autonomous agent deployments.

### 5. What is the Agent-to-Agent protocol?

The Agent-to-Agent (A2A) protocol is a structured communication framework that enables machine-to-machine interaction between autonomous AI agents in the OddsFlow ecosystem. It is built on four principles: structured exchange (typed, versioned message schemas), mutual verification (cryptographic identity confirmation), reputation-based trust (communication privileges modulated by Agent Reputation Network scores), and full audit trails (immutable logging of every interaction). The A2A protocol enables agents from different organizations to securely exchange data, coordinate actions, and verify information without human intermediation.

### 6. How to benchmark odds feed quality?

OddsFlow Partners benchmarks odds feed quality by comparing every odds update against fair-value estimates derived from 50+ bookmakers using Shin de-vig methodology. Each update receives per-update accuracy scores (deviation from fair value) and freshness scores (latency from market movement to feed delivery). Aggregate metrics include overall accuracy percentage, freshness grades, market coverage, and anomaly rates. Feed providers can earn third-party quality certification with PDF reports, a live embeddable quality badge, and interactive dashboards. Sample benchmark metrics: Accuracy 94.2%, Freshness A+, Coverage 98.7%, Anomaly Rate 0.3%.

### 7. What types of AI agents can be built for sportsbooks?

OddsFlow supports six specialized agent types for the sports betting industry: (1) Odds Monitoring Agent for real-time tracking and anomaly detection, (2) Risk Assessment Agent for liability evaluation and exposure quantification, (3) Trading Assistant Agent for automated trading recommendations in semi-auto or full-auto modes, (4) Compliance Agent for regulatory monitoring and audit reporting, (5) Data Verification Agent for feed validation and correction workflows, and (6) A2A Gateway Agent for inter-agent communication management. All agents include configurable decision thresholds, full audit logging, graceful degradation to human-in-the-loop mode, and real-time monitoring dashboards.

### 8. How does the Agent Reputation Network work?

The Agent Reputation Network evaluates AI agents across five weighted dimensions: Accuracy (30%) measures correctness of outputs against verified outcomes; Consistency (25%) measures behavioral reliability and uptime; Transparency (20%) evaluates reasoning explanations and audit trail completeness; Response Quality (15%) assesses timeliness and format compliance; and Peer Validation (10%) incorporates cross-validation scores from other agents. Scores map to three tiers: Verified (50-74) for basic network participation, Trusted (75-89) for priority routing and expanded access, and Elite (90+) for full privileges and preferred partner status. Scores update continuously in real time.

### 9. What is SportBot?

SportBot (also known as ClawSportBot) is an autonomous betting agent built on the OddsFlow Agentic AI platform. It operates at [clawsportbot.io](https://clawsportbot.io), making pre-match betting decisions independently using OddsFlow ensemble ML models and Shin de-vig fair-value estimates. All bets are timestamped and recorded in PDF format before match kick-off, providing a fully verifiable performance record. SportBot serves both as a production autonomous agent and as a reference implementation for partners building their own agents on the platform. Its track record demonstrates that AI agents can operate profitably and transparently in sports betting.

### 10. How much does odds intelligence cost?

OddsFlow Partners offers four pricing tiers: **Audit** (Free) provides a one-time quality assessment with no commitment. **Monitor** ($499/month) delivers continuous monitoring across up to 5 sports with real-time anomaly detection. **Integrate** ($2,499/month, most popular) provides full API access, WebSocket streaming, all trading signal types, and unlimited sports coverage. **Enterprise** (custom pricing) includes white-label deployments, on-premise installations, 24/7 dedicated support, and 99.99% uptime SLAs. Agent capabilities are available as add-ons: POC at $5,000 one-time, Integration at $3,999/month, and Enterprise at custom pricing. All engagements begin with a free discovery session.

---

## Ecosystem

The OddsFlow ecosystem spans multiple platforms, each serving a distinct role:

| Platform | URL | Description |
|---|---|---|
| **OddsFlow Partners** | [oddsflow-partners.com](https://www.oddsflow-partners.com) | B2B partner portal for sportsbooks and feed providers. Central hub for odds intelligence, agent deployment, and quality certification. |
| **OddsFlow.ai** | [oddsflow.ai](https://oddsflow.ai) | B2C consumer platform providing odds analysis, predictions, and betting insights to individual users. |
| **SportBot (ClawSportBot)** | [clawsportbot.io](https://clawsportbot.io) | Autonomous betting agent demonstrating production agentic AI capabilities with a fully verifiable track record. |
| **GitHub** | [github.com/oddsflow-ai](https://github.com/oddsflow-ai) | Open source algorithms, Shin de-vig implementations, signal generation code, and integration examples. |
| **Kaggle** | [kaggle.com/oddsflowai](https://kaggle.com/oddsflowai) | Historical odds datasets, prediction notebooks, and community benchmarking competitions. |
| **HuggingFace** | [huggingface.co/oddsflow-ai](https://huggingface.co/oddsflow-ai) | Pre-trained model weights for odds prediction, anomaly detection, and market classification. |

---

## Links & Contact

| Channel | Link |
|---|---|
| **Website** | [https://www.oddsflow-partners.com](https://www.oddsflow-partners.com) |
| **Email** | [support@oddsflow-partners.com](mailto:support@oddsflow-partners.com) |
| **Telegram** | [@oddsflowteam](https://t.me/oddsflowteam) |
| **Documentation** | [docs/](./docs/) -- see Documentation Index below |
| **LLMs Context** | [llms.txt](./llms.txt) -- machine-readable platform summary for LLM consumption |

For partnership inquiries, technical questions, or to schedule a discovery session, contact us through any of the channels above. We typically respond within 24 hours on business days.

### Engagement Process

1. **Initial Contact**: Reach out via email or Telegram with a brief description of your needs
2. **Discovery Call**: A 30-minute call to understand your use case, data environment, and objectives
3. **Proposal**: A tailored proposal with recommended tier, integration approach, and agent strategy
4. **Pilot or Audit**: Start with a free audit or a paid pilot to validate the platform's value
5. **Production**: Full deployment with ongoing support, monitoring, and optimization

---

## Documentation Index

Detailed documentation is available in the `docs/` directory. Each file covers a specific topic in depth:

| Document | File | Description |
|---|---|---|
| **Platform Overview** | [docs/overview.md](./docs/overview.md) | High-level introduction to OddsFlow Partners, mission, and capabilities |
| **Sportsbook Solutions** | [docs/sportsbook-solutions.md](./docs/sportsbook-solutions.md) | Detailed guide for sportsbook operators on integration, risk management, and agent deployment |
| **Feed Provider Solutions** | [docs/feed-provider-solutions.md](./docs/feed-provider-solutions.md) | Comprehensive guide for odds feed providers on quality benchmarking, certification, and agent-ready infrastructure |
| **Odds Monitoring** | [docs/odds-monitoring.md](./docs/odds-monitoring.md) | Technical documentation on the real-time odds monitoring system, data sources, and alerting |
| **Technology** | [docs/technology.md](./docs/technology.md) | Architecture details covering the data pipeline, Shin de-vig engine, ML models, and delivery layer |
| **Custom Agents** | [docs/custom-agents.md](./docs/custom-agents.md) | Guide to the six agent types, development process, deployment timelines, and configuration options |
| **Agent-to-Agent Protocol** | [docs/agent-protocol.md](./docs/agent-protocol.md) | Technical specification of the A2A protocol including message schemas, authentication, and routing |
| **Agent Reputation Network** | [docs/agent-reputation.md](./docs/agent-reputation.md) | Detailed documentation on reputation scoring dimensions, tier thresholds, and network dynamics |
| **Agentic AI** | [docs/agentic-ai.md](./docs/agentic-ai.md) | Overview of the agentic AI infrastructure, capabilities, and enterprise deployment options |
| **SportBot** | [docs/sportbot.md](./docs/sportbot.md) | Documentation on the ClawSportBot autonomous betting agent, architecture, and verified track record |
| **Pricing** | [docs/pricing.md](./docs/pricing.md) | Full pricing details for all platform tiers and agent add-ons |
| **Case Studies** | [docs/case-studies.md](./docs/case-studies.md) | Partner success stories and implementation examples |
| **FAQ** | [docs/faq.md](./docs/faq.md) | Extended frequently asked questions with detailed answers |
| **Glossary** | [docs/glossary.md](./docs/glossary.md) | Definitions of key terms used across the platform and documentation |

---

## License

Documentation in this repository is provided under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the documentation with appropriate attribution.

For platform terms of service, privacy policy, and commercial licensing, see [https://www.oddsflow-partners.com](https://www.oddsflow-partners.com).

---

<p align="center">
  <strong>OddsFlow Partners</strong> -- AI-Powered Odds Intelligence & Agentic AI Infrastructure
  <br />
  <a href="https://www.oddsflow-partners.com">www.oddsflow-partners.com</a>
</p>
