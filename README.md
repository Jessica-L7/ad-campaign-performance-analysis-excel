# Advertising Campaign Performance Dashboard (Excel)

This repository contains an Excel-based analysis of digital advertising campaign performance. The objective was to transform raw marketing campaign data into a structured analytical model capable of evaluating channel efficiency, creative performance, and audience engagement.

The workflow follows a typical analytics pipeline: data preparation → KPI derivation → segmentation analysis → executive visualisation. The final output is a dashboard designed to support quick evaluation of advertising spend efficiency across platforms and audience segments.

Screenshots of the dashboard are included below.

<img width="933" height="298" alt="image" src="https://github.com/user-attachments/assets/9b275d8c-a633-4a2c-8a6d-686ca32d7e95" />
<img width="929" height="266" alt="image" src="https://github.com/user-attachments/assets/613b9256-a79c-4913-96c9-27c5abd8ecca" />

---

## Technical Skills Demonstrated

Excel capabilities demonstrated in this project include:

- Data preparation and structuring for analysis  
- Pivot table modelling and aggregation  
- Formula-based KPI derivation  
- Cross-sheet referencing and cell-based calculations  
- Dynamic chart linking to pivot outputs  
- Segmentation analysis across campaign dimensions  
- Dashboard construction for performance monitoring  

---

## Project Overview

The project focuses on analysing advertising campaign performance using Excel. Raw campaign data was structured and transformed into a pivot-driven analytical model capable of generating key performance metrics such as Cost Per Click (CPC) and Cost Per Acquisition (CPA).

Rather than relying on static charts, the workbook uses pivot tables, formula-driven metrics, and cross-sheet references so that analytical outputs update automatically as the underlying pivot tables change. This approach allows the dashboard to behave as a lightweight analytical model rather than a static report.

---

## Data Preparation

The raw dataset was cleaned and structured to ensure consistency across campaign attributes such as platform, subchannel, device, creative format, and audience demographics.

Basic preparation steps included:

- Standardising categorical values  
- Ensuring numeric fields were correctly formatted for aggregation  
- Structuring the dataset so it could support pivot-based analysis  
- Preparing campaign attributes for segmentation analysis  

<img width="950" height="537" alt="image" src="https://github.com/user-attachments/assets/a953a4aa-c51b-4752-8dfd-d5bf81ce88e1" />

This structure allows the dataset to be analysed across multiple campaign dimensions without requiring additional transformation during analysis.

---

## Pivot-Driven Modelling

Pivot tables serve as the primary analytical engine within the workbook.

Multiple pivot tables were constructed to aggregate campaign performance across key dimensions such as marketing channel, advertising subchannel, audience age groups, device type, and creative format.

These pivots summarise campaign performance metrics including spend, impressions, and clicks, allowing campaign efficiency to be evaluated across different segments.

Charts within the dashboard are directly linked to these pivot tables so that updates to filters or segment selections automatically propagate through the visualisations.

<img width="944" height="527" alt="image" src="https://github.com/user-attachments/assets/cfbce470-0eb5-4aa0-b528-5e8986a5d48b" />

---

## Formula-Driven KPI Derivation

Key performance indicators were calculated using Excel formulas rather than being manually inserted.

Metrics such as CPC and CPA were derived by combining aggregated values from the pivot tables using formula-based calculations. Typical examples include:

```
Spend / Clicks
Spend / Conversions

```

Additional calculations throughout the workbook use standard Excel cell references and cross-sheet references such as:

=Subchannels!B7

<img width="944" height="507" alt="image" src="https://github.com/user-attachments/assets/0602a47b-9e6e-4c3e-b5a6-415565e2179f" />

This ensures that KPI calculations update automatically whenever the underlying pivot tables refresh, keeping the dashboard outputs synchronised with the source data.

---

## Segmentation Analysis

The analysis evaluates campaign performance by breaking results down across key audience and campaign dimensions.

Segmentation analysis was performed across attributes such as marketing channel, campaign subchannel, device type, audience age groups, and creative format.

By analysing campaign performance across these segments, the dashboard highlights differences in advertising efficiency across platforms, demographics, and creative strategies.

This approach reflects common marketing analytics workflows used to identify high-performing audience segments and optimise campaign allocation.

---

## Dashboard Construction

The final dashboard consolidates the pivot tables, charts, and KPI calculations into a single analytical interface designed for rapid performance evaluation.

Key Excel techniques used in the dashboard include:

- Pivot table aggregation for campaign metrics  
- Dynamic chart linking to pivot table outputs  
- Cross-sheet referencing between analytical layers  
- Formula-driven KPI calculations  
- Conditional formatting to highlight performance variation  
- Structured worksheet organisation separating raw data, analysis, and visualisation layers  

The resulting dashboard updates automatically when pivot tables refresh, allowing campaign performance to be explored quickly without manually rebuilding calculations or charts.

<img width="931" height="282" alt="image" src="https://github.com/user-attachments/assets/95088b72-536a-4a5c-ad2e-b19103d45cba" />
<img width="932" height="344" alt="image" src="https://github.com/user-attachments/assets/dfcc61eb-edaf-4771-aaf2-4ad902070081" />

---

## Repository Files

| File | Description |
|-----|-----|
| `advertising_campaign_dataset.csv` | Original dataset sourced from Kaggle |
| `Advertising_Campaign_Dashboard.xlsx` | Excel workbook containing pivot tables, KPI calculations, and dashboard visualisations |

---

## Recommendations & Analytical Extensions

While Excel is effective for rapid exploratory analysis and ad-hoc reporting, several extensions could further strengthen this analysis if the dataset were larger or if reporting needed to be automated.

### Data Preparation & Scale

If the dataset contained larger volumes of campaign data or required regular ingestion, initial preparation and aggregation could be handled using SQL. This would allow campaign performance metrics to be computed directly in the database before being surfaced in reporting layers.

### Metric Standardisation

Key advertising KPIs such as CPC, CPA, CTR, and CPM could be standardised within a dedicated calculation layer to ensure consistent definitions across reports. In larger analytics environments this logic is typically centralised within a data model rather than calculated independently within dashboards.

### Reporting Automation

For recurring campaign monitoring, dashboards could be connected to automated data refresh pipelines or BI tools such as Looker or Tableau. This would remove manual refresh steps and allow marketing teams to track performance continuously.

### Deeper Performance Analysis

Additional analysis could also incorporate:

- time-series performance trends across campaign periods  
- attribution comparisons between marketing channels  
- creative performance testing across audience segments  
- efficiency comparisons across advertising platforms  

These extensions would allow the analysis to move beyond descriptive reporting toward more strategic campaign optimisation.
