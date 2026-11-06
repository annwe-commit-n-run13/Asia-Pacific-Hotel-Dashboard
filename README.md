# Global & Regional Hotel Industry Performance Dashboard (2019 vs 2021)

## Executive Summary

This project presents an end-to-end interactive performance analytics dashboard built in Excel, evaluating the impact of the COVID-19 pandemic and initial recovery trends across the global hotel industry. By comparing **Pre-Pandemic (2019)** metrics against **Recovery Stage (2021)** performance, the dashboard highlights key operational KPIs across continents, sub-regions within Asia-Pacific, and 8 major Asian metropolitan hospitality markets.

The analysis evaluates three core Hospitality Key Performance Indicators (KPIs):

* **Occupancy Rate (Occ %):** Percentage of available rooms occupied.
* **Average Daily Rate (ADR):** Average rental revenue earned per occupied room per day (in USD).
* **Revenue Per Available Room (RevPAR):** Total room revenue divided by total available rooms (in USD).

---

## Technical Features & Excel Stack

* **Interactive Dynamic Dashboards:** Built using Pivot Tables, Slicers, and linked Pivot Charts for interactive filtering and drill-down analysis.
* **Multi-Tiered Data Granularity:** Structured into three analytical levels: Global/Continental, Asia-Pacific Sub-regions, and Asian City Markets.
* **Calculated Fields & Metrics:** Custom variance calculations evaluating percentage changes ($\Delta\%$) across Occ %, ADR, and RevPAR between 2019 and 2021.
* **Structured Data Modeling:** Raw data transformations organized into staging pivot sheets (`Occ`, `ADR`, `RevPAR`, `AsiaSubCont`, `Sheet2`, `Sheet3`).

---

## Data Storytelling & Analytical Findings

### 1. Global Performance Overview (Continental Level)

The pandemic caused unprecedented disruption across all continents, but recovery trajectories varied significantly based on domestic travel volume and border reopening timelines:

| Continent | Occ % (2019) | Occ % (2021) | Occ Change (%) | ADR 2019 ($) | ADR 2021 ($) | ADR Change (%) | RevPAR 2019 ($) | RevPAR 2021 ($) | RevPAR Change (%) |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **Americas** | 65.4% | 55.8% | **-14.7%** | $130.05 | $123.63 | **-4.9%** | $85.09 | $68.99 | **-18.9%** |
| **Middle East / Africa** | 63.8% | 51.0% | **-20.1%** | $128.61 | $131.37 | **+2.1%** | $82.07 | $67.05 | **-18.3%** |
| **Europe** | 72.2% | 43.3% | **-40.0%** | $125.93 | $121.71 | **-3.4%** | $90.90 | $52.69 | **-42.0%** |
| **Asia Pacific** | 69.1% | 48.7% | **-29.5%** | $96.58 | $77.71 | **-19.5%** | $66.77 | $37.83 | **-43.3%** |

#### Key Continental Takeaways:

* **The Americas led the recovery:** Supported by a massive domestic travel market, the Americas retained the highest occupancy (55.8%) and experienced the mildest decline in RevPAR (-18.9%).
* **Middle East Pricing Resilience:** The Middle East / Africa region was the **only continent to grow ADR (+2.1% to $131.37)** above 2019 levels, buffered by mega-events (e.g., Dubai Expo) and premium luxury positioning.
* **Asia-Pacific & Europe Lags:** Asia-Pacific suffered the steepest RevPAR collapse (**-43.3%**), closely followed by Europe (**-42.0%**), primarily due to strict international travel restrictions and zero-COVID policies during 2021.

---

### 2. Deep Dive: Asia-Pacific Sub-regional Dynamics

A closer look at the sub-regions within Asia-Pacific reveals clear structural splits:

* **Australia & Oceania:** Displayed premium rate power with an ADR increase to **$139.89 (+4.5% vs 2019)**, driven by high domestic leisure demand, even while occupancy dropped from 74.0% to 47.1%.
* **Northeastern Asia (China, Japan, Korea):** Maintained the highest occupancy in the region at **51.8%** due to strong intra-country demand, but suffered an ADR reduction (-18.3% to $71.40).
* **Southeastern Asia:** Hardest-hit sub-region due to heavy reliance on international tourism. Occupancy plummeted from 68.4% to 38.7% (-43.4%), and RevPAR collapsed from $72.46 to $24.14 (**-66.7%**).
* **Central & South Asia:** Experienced a 32.0% decline in occupancy, with RevPAR dropping from $67.70 to $42.70 (-36.9%).

---

### 3. Market-Level Drilldown: 8 Key Asian Cities

Analysis across 8 major Asian hospitality hubs (*Bangkok, Beijing, Hanoi, Ho Chi Minh City, Hong Kong, Jakarta, Mumbai, Phuket*):

* **Resort/Leisure Hubs (Phuket & Bangkok):** Experienced catastrophic RevPAR compression due to border shutdowns. Phuket and Bangkok saw occupancy compress below 25-30% in 2021.
* **Domestic Commercial Centers (Beijing & Mumbai):** Rebounded significantly faster than international tourist markets. Beijing benefited from domestic corporate travel, while Mumbai saw steady domestic business and quarantine/isolation demand.
* **Gateway Cities (Hong Kong & Singapore transit hubs):** Faced sustained ADR discounting to capture sparse regional traffic.

---

## Core Strategic Insights & Recommendations

1. **Rate Discipline Over Occupancy Chasing:** Regions that maintained pricing power (like Middle East and Australia/Oceania) protected their margins better than markets that heavily discounted rates (like Southeast Asia).
2. **Domestic Market Reliance:** Geographies with large internal domestic travel bases (US, China, India) showed far stronger resilience than destination-resort economies (Thailand).
3. **Revenue Strategy Realignment:** Hoteliers in heavily impacted regions must shift focus toward domestic staycations, corporate packages, and non-room revenue streams (F&B, events) until international routes fully normalize.

---

## Repository Structure

├── Hotel Dashboard Project.xlsx   # Main Excel file containing raw data, pivot models & dashboards
│   ├── Final Dashboard            # Complete interactive master dashboard view
│   ├── DashboardAsiaSub           # Sub-regional Asia-Pacific performance dashboard
│   ├── Dashboard8asianCity        # 8 Asian market performance dashboard
│   ├── Sheet3 / Sheet2            # Aggregated metrics & change % tables
│   ├── Occ / ADR / RevPAR         # KPI-specific summary pivot sheets
│   └── Data / AsiaSubCont         # Cleaned source datasets
└── README.md                      # Project documentation and data story

---

## How to Use the Excel File

1. Download or clone this repository:
```bash
git clone https://github.com/your-username/your-repo-name.git

```


2. Open `Hotel Dashboard Project.xlsx` in Microsoft Excel (2016 or newer recommended for optimal slicer functionality).
3. Navigate to the **`Final Dashboard`** sheet.
4. Use the built-in **Slicers** to filter analysis dynamically by Continent, Sub-Region, or Year.
