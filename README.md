# UIDAI-Data-Hackathon-2026-Biometric-Analytics-Dashboard

## Executive Overview
This interactive dashboard provides a comprehensive analysis of national biometric update trends. It empowers stakeholders to monitor demographic distributions, evaluate regional disparities, conduct deep time-series analyses, and identify system anomalies or structural policy shifts.

---

## 📊 Core Metrics & Key Performance Indicators (KPIs)

*   **Total Biometric Updates:** 70 Million (70M)
*   **Child Updates:** 34 Million (34M)
*   **Adult Updates:** 36 Million (36M)
*   **Average Updates per Day:** 783.86K
*   **National Child Ratio %:** 0.49

---

## 🗂️ Dashboard Structure & Features

The application is organized into 5 primary specialized analytical views:

### 1. Executive Overview
*   **Summary Cards:** Immediate visibility into high-level metrics (Total, Child, and Adult updates, Daily averages).
*   **Temporal Splits:** Stacked and clustered bar charts tracking `Child_Updates` vs `Adult_Updates` by `YearMonth` throughout 2025.
*   **Volume Tracking:** Monitors the combined monthly progression of all system registrations.

### 2. Regional Disparity
*   **Concentration Analysis (Pareto Principle):** Highlights that **approximately 20% of states account for nearly 80% of total biometric updates**, indicating strong regional demographic concentration.
*   **Volume Rankings:** Absolute performance tracking across states, revealing leading regions:
    1. *Uttar Pradesh* (~9.6M)
    2. *Maharashtra* (~9.2M)
    3. *Madhya Pradesh* (~5.9M)
    4. *Bihar* (~4.9M)
*   **Time-Series Tracking by State:** Micro-charts assessing date-wise volumetric trendlines unique to individual states (e.g., Andhra Pradesh, Assam, Arunachal Pradesh).

### 3. Age Demographics
*   **Gender/Age Split:** Donut chart evaluating the breakdown between Adult Updates (50.94%) and Child Updates (49.06%).
*   **Age Transition Funnel:** Evaluates continuation behavior from childhood (ages 5-17) into adulthood. A healthy **Transition Rate of 1.04%** shows that adult updates slightly exceed child updates, pointing to sustained engagement beyond mandatory age-based milestones.
*   **Geographic Child Ratios:** Visualizes district-wise distributions and state-level averages for child update ratios (with Mizoram and Chandigarh leading at 0.71 and 0.66, respectively).

### 4. Time Series Analysis
*   **Smoothing & Moving Averages:** Compares actual daily updates against **7-day** and **30-day moving averages** to smooth out weekday/weekend variations and surface the true system trajectory.
*   **Growth Tracking:** A daily volatility index tracking the `Daily Change Rate %` to capture rapid system acceleration or decelerations.

### 5. Anomaly Detection
*   **Statistical Thresholding:** Employs a **Z-Score Based Anomaly Detection Model** to flag anomalous biometric update behaviors that breach upper or lower control boundaries.
*   **Structural Shifts:** Identifies a major system event post-August 2025. A sharp decline from peak metrics (~9.8M down to a baseline of 0.3M–0.6M) indicates a permanent **structural shift** (e.g., policy transition, completion of a massive localized enrollment drive, or modified reporting methodologies) rather than a temporary technical anomaly.

---

## 🛠️ Tech Stack & Data Sources

*   **BI Tooling:** Power BI
*   **Data Dimension Targets:** State, District, Date, YearMonth, Age Group (Child vs Adult).
*   **Analytical Models:** 7-Day & 30-Day Moving Averages, Pareto Distribution (80/20 Rule Analysis), Z-Score Thresholding.

---

## 💡 Key Operational Insights

1. **The August 2025 Pivot:** Data pipelines must adapt to the "new normal" baseline established after August 2025. Historical trend models prior to this date should be partitioned to avoid skewing predictive metrics.
2. **Targeted Scaling:** Because a small handful of states drive the vast majority of volume (e.g., UP, Maharashtra, MP), infrastructure optimization and resource allocation should prioritize these high-density regions.
3. **Child Engagement Stability:** The age transition funnel proves that the ecosystem successfully retains users as they cross demographic thresholds, ensuring long-term data freshness.
