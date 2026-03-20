# 🛡️ GigShield — AI-Powered Parametric Income Insurance for E-Commerce Delivery Partners

**DEVTrails 2026 | Guidewire University Hackathon**
*Protecting the last mile. Automatically.*

---
## LIVE DEMO
https://gigshield-devtrails-2026.vercel.app/
## 📌 Table of Contents

1. [The Problem](#the-problem)
2. [Our Solution](#our-solution)
3. [Persona & Scenarios](#persona--scenarios)
4. [Application Workflow](#application-workflow)
5. [Weekly Premium Model](#weekly-premium-model)
6. [Parametric Triggers](#parametric-triggers)
7. [Adversarial Defense & Anti-Spoofing Strategy](#adversarial-defense--anti-spoofing-strategy)
8. [AI/ML Integration Plan](#aiml-integration-plan)
9. [Fraud Detection](#fraud-detection)
10. [Platform Choice](#platform-choice)
11. [Tech Stack](#tech-stack)
12. [Development Plan](#development-plan)
13. [Team](#team)

---

## The Problem

India's e-commerce delivery partners — working for Amazon Flex, Flipkart Ekart, Meesho, Delhivery — are the invisible engine of the country's ₹5 lakh crore e-commerce sector. These workers operate on a gig basis: no fixed salary, no safety net, no paid leave.

When external disruptions hit — a flash flood in Bengaluru, a sudden curfew in a sensitive zone, or a severe AQI alert in Delhi — delivery partners lose 20–30% of their monthly income overnight. They can't work. The packages don't move. And nobody compensates them.

**GigShield exists to fix that.**

> ⚠️ **Coverage Scope:** GigShield insures **INCOME LOSS ONLY**. We do not cover health, life, accidents, or vehicle repairs. This is a pure parametric income protection product.

---

## Our Solution

GigShield is an AI-enabled parametric insurance platform that:

- Automatically monitors real-time disruption triggers (weather, pollution, curfews)
- Pays out lost income instantly when a trigger threshold is crossed — **no claim filing required**
- Uses ML to calculate a personalised weekly premium based on the worker's zone, delivery history, and local risk profile
- Detects fraud intelligently using GPS validation, claim pattern analysis, ring detection, and anomaly detection

---

## Persona & Scenarios

**Our Persona: E-Commerce Delivery Partner**

- **Platforms:** Amazon Flex, Flipkart Ekart, Meesho, Delhivery
- **Profile:** Typically male, 22–38 years old, owns a two-wheeler, earns ₹600–₹1,200/day, operates in Tier 1–2 Indian cities, week-to-week income with zero employer safety net

---

### Scenario 1 — Environmental Disruption: Flash Flood (Bengaluru)

Ravi is an Amazon Flex partner in Indiranagar, Bengaluru. On Tuesday morning, the IMD issues a Red Alert for heavy rainfall. By 9 AM, water levels in his delivery zone exceed 150mm. His hub goes offline. He can't work.

**GigShield Response:** Rainfall API detects the Red Alert threshold. GigShield auto-initiates a claim. By 10 AM, Ravi receives ₹350 — his estimated lost half-day income — directly to his UPI ID. Zero forms. Zero waiting.

---

### Scenario 2 — Social Disruption: Unplanned Curfew (Lucknow)

Priya is a Flipkart Ekart partner. A sudden Section 144 curfew is imposed in her zone after a local incident. All movement is restricted from 2 PM to 8 PM.

**GigShield Response:** GigShield's social disruption monitor detects the curfew notification via news API. It cross-references Priya's active delivery zone and calculates 6 hours of lost earnings. Payout is initiated automatically.

---

### Scenario 3 — Environmental Disruption: Severe Pollution (Delhi)

Suresh operates in Delhi during November. AQI in his delivery zone crosses 400 (Severe). The government announces a delivery restriction order for two-wheelers.

**GigShield Response:** AQI API from CPCB/IQAir detects the threshold breach. GigShield cross-checks whether a government advisory is active, validates Suresh's GPS is in the affected zone, and triggers a payout for lost working hours.

---

## Application Workflow

**1. Onboard** — Worker registers on GigShield, links their platform ID (Amazon Flex / Flipkart Ekart), and sets their UPI ID for payouts.

**2. Risk Profile** — AI scores the worker's zone risk based on flood history, AQI trends, and curfew frequency, combined with their personal delivery history.

**3. Weekly Policy** — Worker selects a coverage tier (Basic / Standard / Pro). The ML model generates a dynamic weekly premium and auto-debits it every Monday.

**4. Active Coverage** — Real-time disruption monitoring runs continuously in the background. The worker sees their live coverage status on their dashboard.

**5. Disruption Hit** — When a parametric trigger threshold is crossed (e.g. rainfall > 64.5mm), a claim is automatically initiated. The worker does nothing.

**6. Fraud Check** — GPS location, delivery activity, ring pattern, and claim behaviour are validated in under 3 seconds by the fraud detection engine.

**7. Payout** — Instant UPI transfer is sent to the worker's registered ID. An SMS and in-app notification confirms the payout.

---

## Weekly Premium Model

GigShield uses a **weekly subscription model** aligned with how gig workers earn and think about money. No annual commitments. No confusing monthly math. Every Monday, coverage renews and premium is auto-debited.

### Coverage Tiers

| Tier | Weekly Premium | Max Weekly Payout | Best For |
|------|---------------|-------------------|----------|
| Basic Shield | ₹29/week | ₹500/week | Occasional workers (<20 hrs/week) |
| Standard Shield | ₹59/week | ₹1,200/week | Regular workers (20–40 hrs/week) |
| Pro Shield | ₹99/week | ₹2,500/week | Full-time partners (40+ hrs/week) |

### How the Premium is Calculated

The base tier price is adjusted each week by our **ML Risk Engine** using the following factors:

| Factor | Effect on Weekly Premium |
|--------|--------------------------|
| Delivery zone flood risk score | +/- ₹5–15/week |
| Historical AQI in zone (Oct–Feb) | +/- ₹3–10/week |
| Worker's active hours per week | Scales coverage tier |
| Zone's curfew frequency index | +/- ₹2–8/week |
| Worker's claim history | Fraud flag adjustment |

**Example:** A Standard Shield worker in a low-risk zone (Pune, Koregaon Park) pays ₹52/week. The same worker in a high-risk zone (Delhi, Najafgarh) pays ₹71/week. Premium recalculates fresh every Monday.

### Actuarial Viability Sketch

To demonstrate the model is financially sound at scale:

| Tier | Weekly Premium | Expected Claim Freq. | Avg. Payout per Claim | Expected Weekly Loss Cost | Margin |
|------|---------------|----------------------|-----------------------|--------------------------|--------|
| Basic | ₹29 | ~8% of weeks | ₹250 | ₹20 | ~31% |
| Standard | ₹59 | ~10% of weeks | ₹600 | ₹60 | ~0% breakeven → cross-subsidised by low-risk members |
| Pro | ₹99 | ~12% of weeks | ₹1,200 | ₹144 | Reinsurance layer kicks in above ₹80/week loss cost |

> **Note:** These figures are based on IMD historical disruption data for Bengaluru, Delhi, and Mumbai (2019–2024). Actual loss ratios will be validated against real claim data in Phase 2 and adjusted dynamically by the ML pricing engine. The model is designed to maintain a combined loss ratio below 85% across the portfolio, with reinsurance covering tail events (e.g., city-wide floods).

---

## Parametric Triggers

These are objective, data-driven thresholds that automatically initiate a claim. **No subjective assessment. No paperwork.**

| # | Trigger | Data Source | Threshold | Payout Basis |
|---|---------|-------------|-----------|--------------|
| 1 | Heavy Rainfall | OpenWeatherMap API | Rainfall > 64.5mm/day (IMD Red Alert) | Per hour unable to work |
| 2 | Flood Zone Alert | IMD / State Flood Authority feeds | Official flood warning in worker's pin code | Flat daily payout |
| 3 | Severe AQI | CPCB / IQAir API | AQI > 400 + govt two-wheeler advisory | Per restricted hour |
| 4 | Curfew / Section 144 | News API (filtered by location) | Active curfew in worker's delivery zone | Per hour of restriction |
| 5 | Extreme Heat | OpenWeatherMap API | Heat index > 47°C + govt advisory | Per hour during advisory |

All triggers are **cross-validated** against the worker's last known GPS location to prevent fraudulent claims from unaffected zones.

---

## Adversarial Defense & Anti-Spoofing Strategy

> **Market Crash Event Response** — This section directly addresses the coordinated fraud scenario: 500 delivery partners using fake GPS to drain a platform's liquidity pool.

### Why Simple GPS Verification Is Dead

A single GPS check is trivially defeated by mock location apps (available freely on Android). Any fraud ring with basic coordination can fake a location pin. GigShield's defense is designed on the assumption that **no single signal can be trusted in isolation**. A legitimate claim must pass corroboration across four independent layers simultaneously.

---

### Layer 1 — GPS Physics & Trajectory Validation

A real delivery partner's movement leaves a forensic signature: road-constrained paths, realistic velocity curves, natural deceleration at junctions, consistent cell tower handoffs. Spoofed GPS leaves a different one.

**What we check:**
- **Trajectory coherence:** The worker's GPS trace over the preceding 30 minutes must follow plausible road geometry (within 50m of a mapped road). Spoofed emulators often produce perfectly linear movement or teleport between coordinates.
- **Speed physics:** Maximum realistic speed for a two-wheeler in an urban disruption zone is ~40 km/h. Movement faster than this during a claimed "unable to work" period flags the claim.
- **Cell tower cross-check:** GPS coordinates are corroborated against the serving cell tower's known coverage area. A GPS ping claiming Indiranagar, Bengaluru from a tower in Whitefield fails this check.
- **Stationary validation:** During an active disruption claim, the worker should be stationary or minimally mobile. Active delivery movement (GPS trace showing pickup-to-dropoff patterns) during a claimed disruption period auto-rejects the claim.

**Outcome:** GPS spoofing that passes visual inspection fails trajectory physics analysis. This layer eliminates individual bad actors using mock location apps.

---

### Layer 2 — Fraud Ring Detection via Network Graph

This is the critical layer that addresses the **coordinated 500-partner scenario**. Individual anomaly detection misses a fraud ring by design — each individual claim looks plausible in isolation. Network analysis catches what individual checks cannot.

**How it works:**

GigShield constructs a graph where:
- **Nodes** = individual workers
- **Edges** = connections between workers who share: a device fingerprint, the same sub-zone claim within a tight time window, correlated claim timing patterns, or overlapping account registration metadata

**Ring detection signals:**
- **Temporal clustering:** A genuine rainstorm triggers claims distributed across a zone over 1–3 hours as workers encounter the disruption at different times. A fraud ring triggers a burst of claims within a narrow 5–15 minute window. Statistical burst detection (Z-score > 3 on claim rate) flags this immediately.
- **Device fingerprint overlap:** Multiple worker accounts registered from the same device ID or sharing a common device identifier signal coordinated account creation.
- **Shared IP registration:** Workers who registered their accounts from the same IP address cluster are flagged as potentially coordinated.
- **Graph density threshold:** If a sub-zone has more than N workers with 2+ shared edges claiming simultaneously, the entire cluster is flagged. Payouts for the cluster are paused pending review.

**The key distinction:** A legitimate mass disruption (e.g., a city-wide flood) produces a **distributed, uncorrelated** claim graph — workers across many sub-zones, registering from different devices, claiming at varied times. A fraud ring produces a **dense, correlated** cluster. These two patterns are statistically distinguishable even at 500-person scale.

**Outcome:** The fraud ring fails at this layer even if every individual GPS check passes. The coordinated timing pattern alone is sufficient to trigger a zone-level hold.

---

### Layer 3 — Per-Worker Behavioral Baseline

Each worker builds a longitudinal behavioral profile. The ML model learns their typical working patterns, usual zone, historical claim frequency, and delivery platform activity.

**What creates a trustworthy baseline:**
- Workers with 4+ weeks of clean history and consistent platform activity are assigned a **Trust Score** (0–100).
- A first-time worker claiming on Day 1 of their first policy, during their first disruption event, with no delivery history on their linked platform ID receives a low Trust Score and routes to manual review.
- A worker with 6 months of verified delivery history, 2 prior legitimate claims, and consistent GPS patterns in their declared zone receives a high Trust Score and gets expedited auto-approval.

**This is how we distinguish the genuinely stranded worker from the fraudster:**
The honest Ravi who's been delivering in Indiranagar for 8 months gets paid in minutes. The suspicious new account created 3 days ago, claiming from the same zone as 47 other new accounts, does not.

**Outcome:** This layer protects honest workers from being caught in broad fraud sweeps while giving investigators a precise signal on which claims deserve scrutiny.

---

### Layer 4 — Liquidity Circuit Breaker (Zone-Level Protection)

Even if individual fraud signals are subtle, the aggregate effect of a coordinated attack is detectable at the zone level.

**How it works:**
- GigShield tracks a rolling **Zone Claim Rate** for each pin code: the number of active claims as a percentage of registered workers in that zone.
- If the Zone Claim Rate spikes more than **3× the historical baseline** within a 2-hour window, the system automatically:
  1. **Pauses new payout disbursements** from that zone
  2. **Flags all pending claims** in the zone for manual review
  3. **Alerts the admin dashboard** with zone, time, claim volume, and anomaly severity
  4. **Notifies legitimate affected workers** that their claim is under expedited review with an ETA

**Blast radius containment:** This cap ensures that even a sophisticated fraud ring that defeats Layers 1–3 cannot drain the liquidity pool. The maximum exposure from any single coordinated attack is bounded by the circuit breaker threshold.

**Protecting honest workers during a circuit breaker event:** Legitimate workers in an affected zone are not rejected — they are queued for priority human review with a target resolution of <4 hours. Workers with a Trust Score above 80 receive a provisional advance payout (50% of estimated claim) pending full review.

---

### Summary: Why This Architecture Works

| Attack Type | Defeated By |
|-------------|-------------|
| Single worker using mock location app | Layer 1 (GPS physics) |
| Small group with coordinated GPS spoofing | Layer 1 + Layer 2 (network graph) |
| Large fraud ring (500 partners) with fake GPS | Layer 2 (ring detection) + Layer 4 (circuit breaker) |
| New account fraud (first claim, no history) | Layer 3 (behavioral baseline) |
| Sustained low-volume fraud ring | Layer 2 (graph density over time) + Layer 3 |

The system is designed so that **defeating any single layer requires simultaneously defeating all others**. A real fraud ring would need to: spoof GPS with trajectory coherence (Layer 1), avoid device/IP/timing correlation with co-conspirators (Layer 2), build months of fake delivery history (Layer 3), and stay below zone-level statistical thresholds (Layer 4) — simultaneously. This is not operationally feasible at scale.

---

## AI/ML Integration Plan

### 1. Dynamic Premium Calculation (Risk Scoring Model)

- **Approach:** Gradient Boosted Trees (XGBoost) trained on historical weather data, delivery density data, and zone-level disruption frequency
- **Inputs:** Zone pin code, worker's active hours, historical claim frequency in zone, seasonal risk index
- **Output:** Personalised weekly premium multiplier (0.8× – 1.6× base price)
- **Retraining:** Weekly using new weather and claim data

### 2. Fraud Detection Model

- **Approach:** Isolation Forest for anomaly detection + Graph Neural Network for ring detection + rule-based layer
- **Signals monitored:**
  - GPS trajectory physics violations
  - GPS location vs claimed disruption zone mismatch
  - Claim filed during hours worker was GPS-active (contradicts "unable to work")
  - Network graph density and temporal clustering
  - Unusually high claim frequency vs peer workers in same zone
  - Duplicate claim patterns across policy resets
- **Output:** Fraud Risk Score (0–100). Score > 70 = manual review. Score > 90 = auto-reject.

### 3. Payout Estimator

- **Approach:** Regression model
- **Inputs:** Worker's average daily earnings (from platform API / self-declared), hours disruption lasted, coverage tier
- **Output:** Rupee payout amount, capped at tier maximum

---

## Fraud Detection

| Layer | Mechanism | How It Works |
|-------|-----------|--------------|
| GPS Physics | Trajectory coherence check | Road geometry, speed limits, cell tower corroboration |
| Network Graph | Ring detection (GNN) | Temporal clustering, device fingerprint overlap, shared registration signals |
| Activity Contradiction | Delivery activity check | No payout if platform API shows active deliveries during disruption window |
| Behavioral Baseline | Per-worker Trust Score | Longitudinal profile; new accounts get heightened scrutiny |
| Duplicate Prevention | Claim deduplication | Same worker cannot claim two overlapping disruptions simultaneously |
| Anomaly Detection | ML model (Isolation Forest) | Flags statistical outliers vs zone cohort |
| Velocity Check | Rate limiting | More than 3 claims/week triggers enhanced review |
| Circuit Breaker | Zone-level rate monitoring | Zone claim spike → pause payouts, alert admin, queue for review |

---

## Platform Choice

We are building a **Web Application (mobile-responsive / PWA)**.

**Reasoning:**
- E-commerce delivery partners primarily use smartphones but admin/insurer portals require desktop
- A Progressive Web App (PWA) gives native-like mobile UX without App Store approval overhead
- React PWA targets both worker (mobile) and insurer dashboard (desktop) in one codebase
- Faster to build and iterate within the 6-week timeline

---

## Tech Stack

| Layer | Technology | Why |
|-------|-----------|-----|
| Frontend | React.js (PWA) | Fast, component-based, mobile-responsive |
| Backend | Node.js + Express | REST APIs, lightweight, team familiarity |
| Database | PostgreSQL | Relational data for policies, claims, payouts |
| ML Models | Python + FastAPI | XGBoost for premium scoring, Isolation Forest + GNN for fraud |
| Weather API | OpenWeatherMap (free tier) | Rainfall, temperature, heat index triggers |
| AQI API | OpenAQ / IQAir (free tier) | Real-time air quality data |
| News/Curfew | NewsAPI (free tier) | Location-filtered curfew/Section 144 alerts |
| Payments | Razorpay Test Mode | Simulated UPI payouts |
| Auth | Firebase Auth | Quick, secure worker authentication |
| Hosting | Vercel (frontend) + Render (backend) | Free tier, fast deploys |
| Version Control | GitHub | Single repo across all phases |

---

## Development Plan

### Phase 1 (Weeks 1–2): Ideation & Foundation ✅
- [x] Finalise persona and problem scope
- [x] Define parametric triggers and premium model
- [x] Write README and system design
- [x] Define adversarial defense and anti-spoofing architecture
- [x] Set up GitHub repo and project board
- [x] Build basic React app shell + routing
- [x] Create worker onboarding UI mockup
- [x] Record 2-minute strategy video

### Phase 2 (Weeks 3–4): Automation & Protection
- [ ] Worker registration + authentication flow
- [ ] Insurance policy creation with dynamic premium
- [ ] Integrate OpenWeatherMap + OpenAQ APIs
- [ ] Build claims management module
- [ ] Implement ML premium scoring (XGBoost)
- [ ] Build automated trigger monitoring service
- [ ] Implement GPS physics validation (Layer 1)
- [ ] Build network graph ring detection (Layer 2)
- [ ] 2-minute demo video

### Phase 3 (Weeks 5–6): Scale & Optimise
- [ ] Full fraud detection stack (Isolation Forest + GNN)
- [ ] Per-worker Trust Score and behavioral baseline (Layer 3)
- [ ] Zone-level liquidity circuit breaker (Layer 4)
- [ ] Simulated instant payout via Razorpay test mode
- [ ] Worker dashboard (coverage status, payout history, Trust Score)
- [ ] Insurer/admin dashboard (loss ratios, predictive analytics, fraud alerts)
- [ ] End-to-end disruption simulation demo
- [ ] Final pitch deck (PDF)
- [ ] 5-minute demo video



*Built with ❤️ for India's gig economy. GigShield — Because every delivery partner deserves a safety net.*
