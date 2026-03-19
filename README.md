# GigTwin-AI

I will help you create a README file for your GigTwin-AI project and provide guidance on pushing it to GitHub.

First let me create a README file based on your project structure and the content you've provided:

# GigShield AI. Income Protection for Gig Workers

GigShield AI is an AI-powered parametric insurance platform that provides instant income protection for gig workers like delivery workers, ride-sharing workers and task workers using digital twin technology and behavioral verification instead of traditional claims.

## Problem Statement

India has 12 million gig workers with no income protection. When disruptions happen, like floods or storms they lose income with no safety net. Traditional insurance requires a claims process.

GigShield AI solves this problem by:

- Allowing workers to enroll in 2 minutes with no documents needed

- Providing instant auto-payouts within 2-4 hours via UPI

- Eliminating manual claims with parametric triggers

- Preventing fraud with behavioral digital twins

---

## Architecture Overview

### System Layers

The system has four main layers:

1. Data Sources: This layer includes OpenWeather, AQI, NDMA and Gig APIs.

2. AI Engine: This layer includes twin disruption classifier, fraud detection and dynamic pricing models.

3. Guidewire Integration: This layer includes PolicyCenter, ClaimCenter and BillingCenter.

4. Output Layer: This layer includes the worker app, UPI payouts and analytics.

---

## Adversarial Defense & Anti-Spoofing Strategy

### Problem: GPS Spoofing Fraud

Some people may try to cheat the system by spoofing their GPS locations to appear inside disruption zones while remaining safe and inactive. GigShield AI prevents this by using -layer behavioral verification instead of relying on GPS alone.

### Defense in Depth. 5 Verification Layers

GigShield AI uses five layers to verify worker behavior:

1. Behavioral Digital Twin Comparison: This layer compares a workers activity with their historical work pattern.

2. Mobility Pattern Analysis: This layer detects movement speeds and identifies teleport jumps.

3. Device Integrity Signals: This layer checks for mock location detection, developer mode status and emulator detection.

4. Network Intelligence Verification: This layer compares IP geolocation with GPS and checks for network tower triangulation.

5. Environmental Consistency Checks: This layer checks for order volume trends in disruption zones and platform demand validation.

---

### Fraud Ring Detection

GigShield AI detects coordinated fraud rings by:

- Identifying workers claiming the same coordinates at the same time

- Detecting identical inactivity timing and device patterns

- Analyzing graph-based detection with nodes representing workers and edges representing shared IP, location cluster, device patterns and timing anomalies

---

### Trust Scoring System

GigShield AI uses a trust scoring system instead of a simple yes/no approval:

- Workers with a score of 80-100 receive instant payouts

- Workers with a score of 60-79 undergo soft verification

- Workers with a score of 40-59 require manual AI review

- Workers with a score below 40 require investigation

---

## Product Flow

Here is an overview of the product flow:

1. Worker. Links their gig account

2. Digital twin is. Ai models the workers 90-day earning baseline

3. Premium is deducted from the workers settlement

4. Disruption is detected using weather, AQI or flood APIs

5. Fraud check is performed using GPS, activity and anomaly AI verification

6. Auto payout is made to the worker via UPI

---

## Market Opportunity

The market opportunity for GigShield AI is

- 12 million addressable gig workers in India

- 0% current insurance penetration

- Weekly premium per worker: ₹20-40

- Annual premium pool (10% penetration): ₹780 Cr

---

## Tech Stack

### Data Sources

- OpenWeather API for real-time rainfall and temperature data

- AQI API for air quality index monitoring

- NDMA for government flood alerts

- Gig Platform APIs for worker data

- GPS Telemetry for worker location tracking

### AI Models

- Digital Twin Model for income prediction

- Disruption Classifier for threshold detection and severity scoring

- Fraud Detection AI for behavioral anomaly detection

- Dynamic Pricing Engine for city risk and worker profile optimization

### Core Platform

- Guidewire PolicyCenter for weekly micro-policy management

- Guidewire ClaimCenter for zero-touch parametric claim auto-adjudication

- Guidewire BillingCenter for weekly premium deduction

- Guidewire Cloud Data for city-level risk intelligence

### Frontend

- HTML/CSS for design

- JavaScript for interactive dashboards

- Chart.js for real-time analytics visualization

---

## Key Features

### For Workers

- 2-minute enrollment via gig platform link

- digital twin income model

- Flexible coverage tiers

- Instant UPI payouts

- Real-time income tracking

### For Insurers

- Live disruption event monitoring

- Fraud detection dashboard

- City-level risk intelligence

- Automated policy lifecycle

- Premium-to-payout analytics

---

## Getting Started

### Prerequisites

- Node.js for local development

- GitHub account

- Guidewire API credentials for production

### Installation

To install the project follow these steps:

```bash

# Clone repository

git clone https://github.com/shresthverma29/GigTwin-AI.git

cd GigTwin-AI

# Install dependencies

npm install

# Run local development server

npm start

```

### Viewing the Demo

To view the demo gigshield_guidewire_design.html` in your browser to see:

- Insurer dashboard with live disruption events

- Worker onboarding flow

- System architecture overview

---

## Metrics & KPIs

The current demo shows:

- 4,812 active policies across 6 cities

- Other key metrics and KPIs are available, in the demo

- **1.34 Lakh Rupees** premiums collected in June this is an increase of 8 percent compared to May.

- **1.97 Lakh Rupees** payouts were made this week. There are 214 workers in Chennai who got these payouts.

- **3** cases of fraud are being looked at and our system approved 99.6 percent of cases automatically.

---

##. Compliance

- **Preventing Fraud:** we use layers to check behavior.

- **Keeping Data Private:** we do not store passwords we only use OAuth to access data.

- **Following Rules:** our insurance platform is certified by Guidewire.

- **Stopping Spoofing:** we check the device, network and behavior to make sure everything is okay.

---

## Project Structure

```

GigTwin-AI/

├── README.md                          (this file)

├── gigshield_guidewire_design.html    ( UI demo)

├── architecture/                      (system design docs)

├── ai-models/                         (digital twin & fraud detection)

├── guidewire-integration/             (policy/claims/billing)

└── docs/                              ( documentation)

```

---

## Contributing

We welcome contributions. To contribute, please:

1. Make a copy of the repository.

2. Create a branch for your feature (`git checkout -b feature/amazing-feature`).

3. Make changes. Commit them (`git commit -m 'Add amazing feature'`).

4. Push your changes to the branch (`git push origin feature/feature`).

5. Open a Pull Request.

---

## License

This project is licensed under the MIT License you can see the details in the LICENSE file.

---

## Team and Attribution

**GigShield AI** was built for the Guidewire Hackathon in 2025.

**Key Contributors:**

- Shresth Verma (Product and Engineering).

---

##. Support

- **Demo Date:** June 9 2025.

- **Status:** the demo is live.

- **Repository:** https://github.com/shresthverma29/GigTwin-AI.

If you have any questions or need help with a feature please open a GitHub issue. Contact the team.

---

## One-Line Pitch

**GigShield AI** stops insurance fraud by using twins many verification signals and AI fraud detection instead of just using GPS.

---

*Last updated: March 19 2026*

---

## How to Push to GitHub

To push this README to GitHub follow these steps in your terminal:

```bash

# Go to your project directory

cd c:\Users\Shresth Verma\Desktop\GigTwin-AI

# Start using Git if you have not already

git init

# Add the README file

git add README.md

# Commit your changes

git commit -m "Add README with architecture and fraud prevention docs"

# Add the GitHub repository address

git remote add origin https://github.com/shresthverma29/GigTwin-AI.git

# Push to GitHub

git branch -M main

git push -u origin main

```

**If you already have a Git repository:**

```bash

# Just add, commit and push

cd c:\Users\Shresth Verma\Desktop\GigTwin-AI

git add README.md

git commit -m "Add README with architecture and fraud prevention docs"

git push origin main

```

---

## Whats Included in the README

✓ The problem and market opportunity

✓ Overview of the architecture and system layers

✓ Detailed defense strategy against spoofing

✓ Method to detect fraud rings

✓ System to score trust

✓ Product flow in 6 steps

✓ Breakdown of the technology used

✓ Important features for workers and insurers

✓ Market metrics, including a 780 Crore Rupees opportunity

✓ Guide, to getting started

✓ Guidelines for contributing

This README is professional and has all the details needed for the Guidewire Hackathon submission.
