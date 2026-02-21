# 🇺🇸 US Election 2024 — Arizona's 7th Congressional District Analysis & Prediction

![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

> A data-driven analysis and prediction project for the **2024 Presidential Election**, **District Congressional House Representative race**, and **Voter Turnout** in **Arizona's 7th Congressional District** — built using R, Python, web scraping, and geospatial data.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [About the District](#-about-the-district)
- [Objectives](#-objectives)
- [Key Factors Analyzed](#-key-factors-analyzed)
  - [Demographics](#-demographics)
  - [Socioeconomic Indicators](#-socioeconomic-indicators)
  - [Regional & Geopolitical Issues](#-regional--geopolitical-issues)
  - [Political & Electoral History](#-political--electoral-history)
  - [Other Contextual Factors](#-other-contextual-factors)
- [Data Sources](#-data-sources)
- [Tech Stack](#-tech-stack)
- [Methodology](#-methodology)
- [Results & Insights](#-results--insights)

---

## 🔍 Overview

This project forecasts electoral outcomes for the **2024 U.S. General Election** specifically within **Arizona's 7th Congressional District (AZ-07)**. It combines historical election data, demographic profiles, socioeconomic indicators, and geospatial analysis to predict:

1. **Presidential race outcome** at the district level
2. **Congressional House Representative winner**
3. **Voter turnout percentage**

Additionally, the project provides a **brief qualitative and quantitative analysis** of the district-specific factors that shape voter behavior, desires, and needs.

---

## 🗺️ About the District

**Arizona's 7th Congressional District** is situated in the **southwestern part of the state**. As of the most recent redistricting, it encompasses:

| County         | Coverage       |
|----------------|----------------|
| **Yuma**       | Entire county  |
| **La Paz**     | Partial        |
| **Maricopa**   | Partial        |
| **Pima**       | Partial        |
| **Pinal**      | Partial        |
| **Santa Cruz** | Partial        |

The district is characterized by:

- A significant **Hispanic/Latino population**
- Proximity to the **U.S.–Mexico border**
- A mix of **urban, suburban, and rural communities**
- Key industries in **agriculture, military (MCAS Yuma)**, and **trade/logistics**
- Historically competitive but **leans Democratic** in recent cycles

---

## 🎯 Objectives

- **Predict** the presidential vote share and winner in AZ-07
- **Predict** the congressional House race outcome
- **Estimate** voter turnout and identify turnout drivers
- **Analyze** socioeconomic, demographic, and political factors influencing voter preferences
- **Visualize** results through maps, charts, and geospatial overlays

---

## 🔑 Key Factors Analyzed

The following district-specific factors were considered for their potential impact on electoral outcomes:

### 🧑‍🤝‍🧑 Demographics

- Racial and ethnic composition (particularly Hispanic/Latino population share)
- Age distribution and median age
- Population growth and migration patterns

### 💼 Socioeconomic Indicators

- Median household income and poverty rate
- Employment sectors (agriculture, defense, retail, logistics)
- Educational attainment levels
- Healthcare access and insurance coverage

### 🌎 Regional & Geopolitical Issues

- **Immigration and border security** — direct proximity to the U.S.–Mexico border
- **Water scarcity and Colorado River policy** — critical for Yuma's agricultural economy
- **Military presence** — Marine Corps Air Station Yuma's economic influence
- **Trade and cross-border commerce** — USMCA impacts on local businesses

### 🗳️ Political & Electoral History

- Historical voting patterns and partisan lean (Cook PVI)
- Incumbency effects and candidate quality
- Early voting and mail-in ballot trends
- Voter registration trends (Democratic, Republican, Independent)

### 🌡️ Other Contextual Factors

- National political environment and presidential approval ratings
- Issue salience (economy, immigration, abortion, cost of living)
- Campaign spending and ground-game intensity

---

## 📊 Data Sources

| Source | Data Collected |
|--------|----------------|
| [Arizona Secretary of State](https://azsos.gov/) | Official election results, voter registration data, turnout statistics (web scraped) |
| [Ballotpedia — Arizona]([https://ballotpedia.org/](https://ballotpedia.org/Arizona%27s_7th_Congressional_District_special_election,_2025)) | Candidate information, district profiles, historical race results (web scraped) |
| [U.S. Census Bureau / TIGER Shapefiles](https://www.census.gov/geographies/mapping-files.html) | Demographic shapefiles, congressional district boundaries |
| [American Community Survey (ACS)](https://www.census.gov/programs-surveys/acs) | Socioeconomic and demographic indicators |
| Government & Demographic Shapefiles | Geospatial boundary data for counties and districts |

> **Note:** Data was collected through a combination of **web scraping** (Ballotpedia, AZ Secretary of State) and **publicly available government shapefiles and datasets**.

---

## 🛠️ Tech Stack

### Languages

- **R** — Statistical modeling, geospatial analysis, visualization
- **Python** — Web scraping, data wrangling, automation

### Key Libraries & Tools

| Purpose              | R Packages                            | Python Libraries                          |
|----------------------|---------------------------------------|-------------------------------------------|
| Data Wrangling       | `dplyr`, `tidyr`, `readr`             | `pandas`, `numpy`                         |
| Web Scraping         | `rvest`, `httr`                       | `BeautifulSoup`, `requests`, `selenium`   |
| Geospatial Analysis  | `sf`, `tigris`, `tmap`                | `geopandas`, `shapely`, `folium`          |
| Visualization        | `ggplot2`, `leaflet`, `plotly`        | `matplotlib`, `seaborn`, `plotly`         |
| Modeling             | `caret`, `glm`, `randomForest`       | `scikit-learn`, `statsmodels`             |

---

## Methodology

## 📐 Methodology

<table>
<tr>
<td align="center" width="150">
<h3>📥</h3>
<b>Step 1</b><br>
Data Collection<br>
<sub>Web Scraping<br>(Ballotpedia & AZ SOS)<br>+ Government Shapefiles<br>+ ACS Demographics</sub>
</td>
<td align="center" width="30">
<h3>➡️</h3>
</td>
<td align="center" width="150">
<h3>⚙️</h3>
<b>Step 2</b><br>
Data Processing<br>
<sub>Cleaning<br>Standardization<br>Multi-Source Merging<br>Geometry Validation</sub>
</td>
<td align="center" width="30">
<h3>➡️</h3>
</td>
<td align="center" width="150">
<h3>🧪</h3>
<b>Step 3</b><br>
Feature Engineering<br>
<sub>Demographic Ratios<br>Vote Margins<br>Turnout Trends<br>Registration Shifts</sub>
</td>
<td align="center" width="30">
<h3>➡️</h3>
</td>
<td align="center" width="150">
<h3>📊</h3>
<b>Step 4</b><br>
Predictive Modeling<br>
<sub>Random Forest<br>Gradient Boosting<br>Decision Tree<br>SVM & Linear Reg</sub>
</td>
<td align="center" width="30">
<h3>➡️</h3>
</td>
<td align="center" width="150">
<h3>🗺️</h3>
<b>Step 5</b><br>
Geospatial Mapping<br>
<sub>Precinct Choropleths<br>County Overlays<br>District Boundaries<br>Poverty Heatmaps</sub>
</td>
<td align="center" width="30">
<h3>➡️</h3>
</td>
<td align="center" width="150">
<h3>📈</h3>
<b>Step 6</b><br>
Reporting<br>
<sub>Charts & Plots<br>Model Comparison<br>Final Insights<br>& Conclusions</sub>
</td>
</tr>
</table>

## Results and Insights

### 1. 🏛️ Presidential Race Prediction - AZ - 07

| Metric | Training Data (Historical) | Model Prediction (2024) |
|--------|---------------------------|------------------------|
| **Winner** | Democrat | **Democrat** |
| **Precincts Won** | 1,065 / 1,494 | 267 / 299 |
| **Win Percentage** | 71.29% | **89.30%** |

> **Interpretation:** The model predicts a **dominant Democratic victory** in AZ-07
> for the 2024 presidential race, with an even stronger margin (~89%) than the
> historical baseline (~71%)

### 2. 🏠 Congressional House Representative Prediction

| Field | Result |
|-------|--------|
| **Predicted Winner** | **Raul Grijalva** (Democrat) |
| **Incumbency** | Incumbent (long-serving representative of AZ-07) |

The model was trained on historical candidate data including vote counts and
incumbency status. After encoding candidates and scaling features using
imputation and standardization pipelines, the **Random Forest classifier**
predicted **Raul Grijalva** as the winning candidate.

The precinct-level choropleth map of the 2022 AZ-07 congressional race
confirmed overwhelming **blue (Democrat)** dominance across the district,
with Republican wins limited to sparse rural precincts.

<img width="722" height="346" alt="Screenshot 2026-02-20 at 10 01 47 PM" src="https://github.com/user-attachments/assets/90529060-e460-44ab-a9ab-6fe56a4296f0" />

### 3. 🗳️ Voter Turnout Prediction

Across the three major counties of AZ-07 (Pima, Maricopa, Yuma)

**County-Level Breakdown (Gradient Boosting):**

| County | Predicted Ballots | Eligible Voters | Turnout % |
|--------|------------------|-----------------|-----------|
| Pima | 354,640 | 637,671 | **55.61%** |
| Maricopa | 1,562,866 | 2,357,115 | **66.30%** |
| Yuma | 55,716 | 93,988 | **59.28%** |
| **Total** | **1,973,222** | **3,088,774** | **63.88%** |

> **Key Takeaway:** Maricopa County drives the highest absolute turnout due to
> population size, while Yuma County shows moderate engagement (~59%), likely
> influenced by its rural character and demographic composition.

### 4. 🔍 Key Factors Influencing Voter Preferences

The R-based demographic and socioeconomic analysis revealed several critical
factors that shape voter behavior in AZ-07:

#### 🧑‍🤝‍🧑 Racial & Ethnic Composition

| County | Dominant Race | Percentage |
|--------|--------------|------------|
| Maricopa | White | 53.25% |
| Pima | White | 50.05% |
| **Yuma** | **Hispanic** | **65.26%** |

> Yuma County's **supermajority Hispanic population** (65.26%) is a defining
> characteristic of AZ-07. This demographic heavily influences the district's
> lean toward Democratic candidates and elevates **immigration, border policy,
> and bilingual services** as top electoral issues.

#### 💰 Median Household Income

The ACS data comparison of U.S.–Mexico border states reveals Arizona's
relative economic position:

| State | Median Household Income |
|-------|------------------------|
| California | Highest among border states |
| Texas | Mid-range |
| **Arizona** | **Below California & Texas** |
| New Mexico | Lowest among border states |

> Within AZ-07, **Yuma County has the lowest median income**, correlating with
> higher poverty rates and greater demand for social safety net programs — a
> factor that historically benefits Democratic candidates.

#### 🎓 Education Levels

Analysis of high school diploma and bachelor's degree attainment across
AZ-07 counties revealed:

- **Maricopa County** leads in bachelor's degree holders, reflecting its
  urban/suburban character
- **Yuma County** has the lowest educational attainment, correlating with its
  agricultural economy and immigrant workforce
- **Pima County** falls in between, anchored by Tucson's university presence

> Lower education levels in Yuma correlate with **economic vulnerability**
> and increased sensitivity to **cost-of-living and wage issues**.

#### 💼 Employment Status

- All three counties show **high employment rates** relative to state averages
- **Yuma County** has the **highest unemployment rate** among the three,
  driven by seasonal agricultural employment patterns
- Maricopa and Pima benefit from diversified economies (tech, defense, healthcare)

> Seasonal unemployment in Yuma makes **job security and agricultural labor
> policy** critical swing factors.

#### 👶 Age Distribution

- Yuma County trends **younger**, consistent with its larger Hispanic
  family demographic
- Maricopa shows a balanced age distribution with significant retiree populations
- Pima has a notable university-age cohort (University of Arizona)

> A younger electorate in Yuma increases the importance of **education
> funding, youth employment, and affordable housing** as campaign issues.

#### 🏥 Poverty & Health Insurance

The poverty choropleth map (from shapefile analysis) revealed:

- **Concentrated poverty pockets** in southern Yuma and parts of rural Pima
- Strong spatial correlation between **high poverty areas and Democratic
  precinct wins**
- Health insurance coverage gaps align with poverty clusters

> Poverty concentration in AZ-07 makes **Medicaid expansion, ACA protections,
> and social welfare programs** electorally significant.

#### 🗺️ Geospatial Patterns

The precinct-level maps revealed:

- **Urban precincts** (Tucson suburbs in Pima, southwest Maricopa) are
  **overwhelmingly Democratic**
- **Rural precincts** (eastern La Paz, rural Pinal) show **pockets of
  Republican support**
- The **border corridor** (Yuma to Santa Cruz) is a **Democratic stronghold**
