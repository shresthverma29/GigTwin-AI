# GigShield AI — Income Protection for Gig Workers

**GigShield AI** is an AI-powered parametric insurance platform that provides instant income protection to gig workers (delivery partners, ride-sharing drivers, task workers) using Digital Twin modeling, AI income prediction, and behavioral fraud verification.

Instead of manual claims, GigShield AI predicts expected income, detects disruptions, verifies authenticity, and automatically triggers payouts within 2–4 hours via UPI.

**Mission:** Make gig worker insurance instant, automated, fraud-resistant, and accessible.

---

## 🎯 The Problem

India has **12 million gig workers** with zero income protection. When disruptions hit—heavy rain, pollution spikes, platform outages, demand crashes—workers lose income immediately with no safety net.

### Why Traditional Insurance Fails

❌ Claims take weeks to process  
❌ Heavy documentation required  
❌ Manual verification delays  
❌ Limited gig worker eligibility  
❌ Not designed for variable daily income  

### Our Solution

✅ **2-minute enrollment** (no paperwork)  
✅ **Instant auto-payouts** (2–4 hours via UPI)  
✅ **Zero manual claims** (parametric triggers)  
✅ **AI fraud detection** (behavioral verification)  
✅ **Digital Twin modeling** (personalized income baseline)  

---

## 👥 Target User Persona

### Ravi — Delivery Partner (Age 23)

```
Daily Income:      ₹850
Savings:          <₹10,000
Platform:         Swiggy
Device:           Smartphone
Problem:          Heavy rain = ₹0 income that day

Traditional insurance:
  • Requires documents
  • Claims take 2–3 weeks
  • Not built for gig workers
  
GigShield AI:
  • Automatic detection
  • Same-day payout
  • Mobile-first process
  • No manual filing
```

### Target Demographics

| Attribute | Value |
|-----------|-------|
| Age | 18–40 |
| Income Type | Daily variable earnings |
| Average Income | ₹400–₹1,500/day |
| Device Type | Smartphone |
| Primary Risk | Immediate income loss during disruptions |

---

## 🏗️ System Architecture

GigShield AI consists of **four core layers**:

```
┌─────────────────────────────────────────────────┐
│ Data Sources Layer                              │
│ OpenWeather · AQI · NDMA · Gig Platform APIs   │
└──────────────────┬──────────────────────────────┘
                   ↓
┌─────────────────────────────────────────────────┐
│ AI Engine Layer                                 │
│ Digital Twin · Disruption Classifier            │
│ Fraud Detection · Dynamic Pricing               │
└──────────────────┬──────────────────────────────┘
                   ↓
┌─────────────────────────────────────────────────┐
│ Insurance Workflow Layer (Guidewire)            │
│ PolicyCenter · ClaimCenter · BillingCenter      │
└──────────────────┬──────────────────────────────┘
                   ↓
┌─────────────────────────────────────────────────┐
│ Output Layer                                    │
│ Worker Mobile App · UPI Payouts · Dashboard     │
└─────────────────────────────────────────────────┘
```

---

## 🤖 How Our AI Works

GigShield AI uses a **three-engine AI architecture**:

### Engine 1: Income Prediction (Digital Twin)

Each worker receives a personalized Digital Twin model based on:

```
✓ Historical earnings (90 days)
✓ Working hours patterns
✓ Location productivity
✓ Gig platform demand
✓ Seasonal trends
✓ Weekly consistency
```

**Output:** Expected weekly income baseline

**Example:**
```
Expected income: ₹5,500
Actual income:   ₹2,100
Deviation:       62% ← INCOME LOSS DETECTED

→ Triggers fraud check + possible payout
```

---

### Engine 2: Disruption Detection

AI validates disruptions using **multi-signal analysis**:

```
Weather Signal:
  ✓ OpenWeather API rainfall
  ✓ Severity threshold crossing
  
AQI Signal:
  ✓ Air quality index spike
  ✓ Breathing difficulty alert
  
Disaster Signal:
  ✓ NDMA flood alerts
  ✓ Government notifications
  
Platform Signal:
  ✓ Order volume drop
  ✓ Demand reduction
  
Income Signal:
  ✓ Earnings deviation
  ✓ Pattern anomaly
```

**Trigger Logic:**
```
IF (actual_income < threshold) 
   AND (disruption_signal = true)
   AND (fraud_check = pass)
THEN
   Payout triggered automatically
```

---

### Engine 3: Fraud Detection

GigShield AI verifies authenticity using **5 verification layers** instead of GPS alone:

#### Layer 1: Behavioral Pattern Verification
```
✓ Historical earning baseline vs current claim
✓ Working hours consistency
✓ Login activity during disruption
✓ Order acceptance patterns
```

#### Layer 2: Device Integrity Signals
```
✓ Mock GPS detection
✓ Developer mode check
✓ Rooted/jailbreak detection
✓ Sensor consistency validation
```

#### Layer 3: Network Intelligence
```
✓ IP geolocation vs GPS comparison
✓ Tower triangulation verification
✓ WiFi region mapping
✓ VPN detection
```

#### Layer 4: Movement Pattern Analysis
```
✓ Speed validation (realistic travel)
✓ Route continuity checks
✓ Teleport detection (impossible jumps)
✓ GPS drift pattern analysis
```

#### Layer 5: Platform Activity Verification
```
✓ Orders received vs accepted
✓ Online duration
✓ Cancellation logs
✓ Real-time demand trends
```

---

## 🔐 Adversarial Defense & Anti-Spoofing Strategy

### The Core Principle

**Behavior > Location**

Because GPS can be spoofed, but behavioral patterns are significantly harder to fake consistently.

### Genuine Worker vs GPS Spoofer

**Genuine Worker Signals:**
```
Normal Pattern:
  • 18–22 deliveries/day
  • Regular login activity
  • Consistent order acceptance
  
During Disruption:
  • Reduced but NOT zero activity (6–8 deliveries)
  • Login attempts visible
  • Order cancellations documented
  • Gradual income drop (~40%)
  • Platform shows demand reduction
  
Result: ✅ GENUINE DISRUPTION CLAIM
```

**GPS Spoofer Signals:**
```
Fraud Pattern:
  • Perfect GPS location match (inside flood zone)
  • Zero activity
  • Zero login attempts
  • Zero order interaction
  • Static device behavior
  • Sudden complete inactivity
  • No behavioral deviation explanation
  
Result: ❌ FRAUD DETECTED
```

---

### Fraud Ring Detection

GigShield AI detects **coordinated syndicate fraud** using graph-based clustering:

**What triggers alarm:**
```
Multiple workers showing:
  ✓ Identical GPS coordinates
  ✓ Synchronized inactivity (same timestamp)
  ✓ Same device fingerprints
  ✓ Same network/IP clusters
  ✓ Synchronized income drops (same %)
  
Cluster density > threshold → FRAUD RING SUSPECTED
```

**Example Detection:**
```
50 workers identified:
  • Stopped work at same time: 14:30 IST
  • All claim same weather zone: Chennai
  • All show identical GPS drift patterns
  • All use same IP range: 203.X.X.X
  • All dropped earnings by 87%
  
AI Analysis:
  Normal connection rate: 5–10%
  Detected cluster: 87%
  
Action: Investigation escalated, cluster flagged
```

---

## 🎯 End-to-End Product Flow

```
Step 01: Worker Enrolls
└─ Links gig platform account (Swiggy/Zomato/Uber)
   └─ Takes 2 minutes, no documents

Step 02: Digital Twin Built
└─ AI analyzes 90 days of earning history
   └─ Establishes weekly income baseline
   └─ Confidence score: 94% average

Step 03: Premium Deducted
└─ ₹20–40/week automatically deducted
   └─ From weekly gig platform settlement
   └─ Flexible, can cancel anytime

Step 04: Disruption Detected
└─ OpenWeather/AQI/NDMA API triggers
   └─ Real-time event confirmation
   └─ Location-specific impact verified

Step 05: Fraud Check
└─ GPS + behavior + network + device anomaly AI
   └─ Digital Twin comparison
   └─ Fraud ring cluster detection
   └─ Trust score calculated

Step 06: Auto Payout
└─ UPI transfer within 2–4 hours
   └─ No claim forms needed
   └─ Notification sent to worker
```

---

## 🛡️ UX Balance — Honest Worker Protection

GigShield AI uses a **trust-first approach** instead of punitive rejections.

### Risk-Based Processing

```
Low Risk (80–100 trust score)
  → Instant payout without questions

Medium Risk (60–79 trust score)
  → Quick soft verification
  → Lightweight proof requested (selfie, location refresh)
  → Most pass within minutes

High Risk (40–59 trust score)
  → AI review required
  → Claims specialist involvement
  
Fraud Risk (<40 trust score)
  → Investigation + claims team
```

### Soft Verification Instead of Rejection

If anomalies detected, workers aren't automatically rejected:

**Lightweight Verification Options:**
```
Option 1: Live Location Refresh
  • Re-confirm GPS location right now
  • Quick GPS check
  
Option 2: App Activity Validation
  • Show platform login/order activity during claim period
  • Instant verification
  
Option 3: Selfie Verification
  • Photo timestamp matching claim time
  • Quick identity check
  
Option 4: Session Confirmation
  • Verify device session during disruption
```

Most genuine workers clear verification within minutes.

### Partial Payout Protection

If verification is still pending:

```
Step 1: Release 30% payout immediately
Step 2: Worker receives partial relief
Step 3: Complete verification in background
Step 4: Release remaining 70% after verification

Result: Genuine workers not financially harmed during checks
```

### Honest Worker Detection Logic

System defaults to **trust** if:

```
✓ Did worker attempt to log in during disruption?
✓ Did worker try to accept orders?
✓ Did platform demand drop in area?
✓ Is disruption independently confirmed?

If 3+ of above = YES
  → Treat as genuine claim
  → Accept even if some geo signals are weak
```

---

## 📊 Market Opportunity

| Metric | Value |
|--------|-------|
| **Addressable gig workers in India** | 12 million |
| **Current insurance penetration** | 0% |
| **Weekly premium per worker** | ₹20–₹40 |
| **Annual premium pool (10% penetration)** | **₹780 Cr** |

GigShield AI addresses a completely **uninsured market**.

---

## 💼 Key Features

### For Gig Workers
✅ 2-minute enrollment via gig platform link  
✅ Transparent digital twin income model  
✅ Flexible coverage tiers (₹20–40/week)  
✅ Instant UPI payouts (no claims process)  
✅ Real-time earnings dashboard  
✅ Trust-first verification (not punitive)  
✅ Income protection during disruptions  

### For Insurers
✅ Live disruption event monitoring  
✅ Real-time fraud detection dashboard  
✅ City-level risk intelligence  
✅ Automated policy lifecycle (weekly)  
✅ Zero-touch parametric claims  
✅ Premium-to-payout analytics  
✅ Fraud ring early warning system  

---

## 🚀 Execution Plan

### Phase 1: Prototype ✅ (Implemented)

- ✅ Worker onboarding interface
- ✅ Simulated income dataset
- ✅ AI income prediction model
- ✅ Disruption trigger logic
- ✅ Fraud detection simulation
- ✅ Dashboard prototypes
- ✅ System architecture visualization

### Phase 2: Integration 🔄 (Planned)

- 🔄 Gig platform API integrations (Swiggy, Zomato, Uber)
- 🔄 Real-time disruption feeds
- 🔄 Mobile application (iOS/Android)
- 🔄 Payment gateway integration (UPI/bank)
- 🔄 Guidewire PolicyCenter/ClaimCenter integration

### Phase 3: Production 🎯 (Future)

- 🎯 Scalable AI infrastructure
- 🎯 Advanced fraud detection ML models
- 🎯 Insurance partnership agreements
- 🎯 Smart contract automation
- 🎯 City-level expansion (tier 1+2)

---

## 🛠️ Tech Stack

### Data Sources
- **OpenWeather API** — Real-time rainfall, temperature
- **AQI API** — Air quality index monitoring
- **NDMA** — Government flood alerts
- **Gig Platform APIs** — Swiggy, Zomato, Amazon Flex, Zepto, Uber, Ola
- **GPS Telemetry** — Worker location tracking

### AI Models
- **Digital Twin Model** — LSTM-based income predictor (per worker)
- **Disruption Classifier** — Threshold detection & severity scoring
- **Fraud Detection AI** — Multi-signal behavioral anomaly detection
- **Dynamic Pricing Engine** — City risk × worker profile × history

### Core Platform (Guidewire)
- **PolicyCenter** — Weekly micro-policy management
- **ClaimCenter** — Zero-touch parametric claim auto-adjudication
- **BillingCenter** — Weekly premium collection & settlement
- **Guidewire Cloud Data** — City-level risk intelligence

### Frontend
- **HTML/CSS** — Responsive insurance dashboard
- **JavaScript** — Interactive UI & real-time updates
- **Chart.js** — Real-time analytics visualization
- **Mobile** — React Native (future)

---

## 📱 Live Demo Features

The interactive prototype includes:

### Screen 1: Insurer Dashboard
- Active policy metrics (4,812 policies across 6 cities)
- Live disruption event tracking (Chennai rainfall: 82mm)
- Real-time payout processing (₹1.97L this week)
- Fraud detection queue (99.6% auto-approval rate)
- Payout triggers chart (weekly breakdown)
- Premium vs payout analytics
- City risk index visualization
- Active disruption event table

### Screen 2: Worker Onboarding
- 4-step enrollment flow
- Platform linking (Swiggy, Zomato, Amazon Flex, Zepto)
- Digital twin income visualization
- Weekly earning baseline display (₹5,500)
- Coverage tier selection (Basic/Standard/Pro)
- Policy activation confirmation
- Real-time progress tracking

### Screen 3: System Architecture
- End-to-end product flow visualization
- 4-layer system architecture diagram
- Guidewire integration points
- Data sources overview
- AI engines breakdown
- Market opportunity metrics
- Technology stack details

---

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari)
- No installation required

### Viewing the Live Demo

```bash
# Clone the repository
git clone https://github.com/shresthverma29/GigTwin-AI.git
cd GigTwin-AI

# Open in browser
open gigshield_guidewire_design\ 2\ \(13\).html
# Or
start gigshield_guidewire_design\ 2\ \(13\).html  # Windows
```

**Features:**
- ✅ Interactive insurer dashboard with real-time data
- ✅ 4-step worker onboarding simulator
- ✅ System architecture visualization
- ✅ Live disruption event tracking
- ✅ Fraud detection reviews
- ✅ Premium vs payout analytics with Chart.js
- ✅ Responsive mobile-friendly design

---

## 📊 Current Demo Metrics

Live dashboard shows:

```
Active Policies:              4,812 (across 6 cities)
Premiums Collected (Jun):     ₹1.34L (+8% vs May)
Payouts This Week:            ₹1.97L (214 workers in Chennai)
Fraud Flags Under Review:     3 (99.6% auto-approval rate)

Active Disruption:
  • Chennai rainfall: 82mm (exceeded 50mm threshold)
  • Triggered policies: 214
  • Estimated payout: ₹1,97,080
  • Status: Processing

City Risk Index (Jun 2025):
  1. Delhi: 86 (High)
  2. Mumbai: 78 (High)
  3. Chennai: 65 (Medium)
  4. Jaipur: 58 (Medium)
  5. Bengaluru: 32 (Low)
```

---

## 🌍 Market Crash Response Strategy

Gig worker income is sensitive to multiple disruptions:

- Weather events (rain, floods, heatwaves)
- Pollution spikes (high AQI)
- Platform outages
- Fuel price shocks
- Demand crashes
- Economic slowdown

**GigShield AI handles this using:**

### 1. Adaptive Risk Thresholds
AI dynamically adjusts payout sensitivity during downturns to protect the loss pool while ensuring necessary payouts.

### 2. Risk Pool Protection
Loss distributed across insured users and reinsurance partners.

### 3. Dynamic Premium Adjustment
Premium based on:
- Individual risk score
- Location hazard index
- Disruption frequency
- Worker earning stability

This ensures sustainability during large-scale disruptions.

---

## 🔐 Security & Privacy

- **No Password Storage** — OAuth-only access to gig platforms
- **Data Encryption** — All data in transit and at rest encrypted
- **Device Integrity** — Mock GPS & jailbreak detection
- **Network Security** — VPN & proxy detection
- **GDPR/India DPA Compliant** — Privacy-first architecture
- **Audit Trail** — All claims and payouts logged

---

## 📚 Project Structure

```
GigTwin-AI/
├── README.md                                  (this file)
├── gigshield_guidewire_design 2 (13).html     (main interactive demo)
├── docs/
│   ├── ARCHITECTURE.md                        (detailed system design)
│   ├── FRAUD_DETECTION.md                     (anti-spoofing strategy)
│   ├── DIGITAL_TWIN.md                        (income modeling)
│   ├── API_INTEGRATION.md                     (Guidewire integration)
│   └── USER_GUIDE.md                          (worker guide)
├── data/
│   ├── sample_policies.json                   (demo dataset)
│   ├── disruption_events.json                 (sample disruptions)
│   └── earnings_history.json                  (worker income data)
└── assets/
    ├── logo.svg
    ├── city_risk_map.png
    └── screenshots/
```

---

## 📞 Contact & Support

- **Event:** Guidewire Hackathon 2025
- **Demo Date:** June 9, 2025
- **Status:** Live prototype active
- **Repository:** https://github.com/shresthverma29/GigTwin-AI

### Feedback & Issues
- **Report Issues:** [GitHub Issues](https://github.com/shresthverma29/GigTwin-AI/issues)
- **Feature Requests:** [GitHub Discussions](https://github.com/shresthverma29/GigTwin-AI/discussions)
- **Contact:** shresthverma452@gmail.com/jv8132@srmist.edu.in

---

## 🎯 Key Innovation Summary

GigShield AI combines:

✅ **Parametric Insurance** — No manual claims  
✅ **Digital Twin Modeling** — Personalized income baselines  
✅ **Behavioral AI Verification** — Multi-signal fraud detection  
✅ **Fraud-Resistant Payouts** — 5-layer verification  
✅ **Instant Compensation** — 2–4 hour UPI transfers  
✅ **Trust-First UX** — Protects honest workers first  

This removes traditional insurance friction entirely.

---

## 📈 Impact & SDG Alignment

GigShield AI enables:

- ✅ **Financial Stability** for 12M Indian gig workers
- ✅ **Faster Payouts** (2–4 hours vs 2–3 weeks)
- ✅ **Fraud Reduction** (99.6% auto-approval with AI verification)
- ✅ **Increased Platform Trust** (worker confidence)
- ✅ **SDG Goal 8** (Decent Work and Economic Growth)
- ✅ **SDG Goal 1** (No Poverty — income protection)

---

## 🎯 One-Line Pitch

**"GigShield AI prevents parametric insurance fraud using behavioral digital twins, multi-signal verification, and AI fraud graph detection instead of relying on spoofable GPS triggers."**

---

## ⚡ Vision Statement

**Income protection for India's 12 million gig workers — instant, fair, fraud-proof, and accessible to all.**

---

*Last updated: March 20, 2026*  
*Built with ❤️ by Team BeyondTheBench*  
*Demo status: ✅ Live and interactive*
