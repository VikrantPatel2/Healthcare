# Healthcare Waiting List Analysis Dashboard

![Healthcare Dashboard](https://tse4.mm.bing.net/th/id/OIP.ADQb3jYZVA2cMcKUVV8GTwHaEc?r=0&pid=Api&P=0&h=180)

## 📊 Project Overview

This project is an interactive **Healthcare Waiting List Analysis Dashboard** built in **Microsoft Power BI**.

The dashboard analyzes healthcare waiting-list data across multiple years and provides a clear view of:

- Total waiting-list volume
- Latest-month waiting list compared with the previous year
- Waiting-list distribution by case type
- Waiting times across different time bands
- Waiting-list patterns by age profile
- Specialty-level waiting-list performance
- Historical trends over time
- Detailed records that can be filtered and explored

The goal is to turn large, multi-year healthcare waiting-list datasets into an interactive reporting solution that can support **monitoring, comparison, trend analysis, and operational decision-making**.

---

## 🎯 Business Problem

Healthcare organizations need to continuously monitor waiting lists to understand:

1. How large the current waiting list is
2. Whether waiting-list volume is increasing or decreasing
3. Which case types contribute most to the total
4. Which age groups have higher waiting volumes
5. How many patients are waiting for extended periods
6. Which specialties have higher waiting-list pressure
7. How waiting lists change over time

Working with separate yearly files makes these questions difficult to answer quickly.

### Solution

This Power BI project combines and analyzes the available waiting-list datasets and presents the results through an interactive dashboard with filters, KPIs, charts, trend analysis, and a detailed drill-down style view.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Power BI** | Dashboard development and visualization |
| **Power Query** | Data loading, transformation, and preparation |
| **DAX** | KPI calculations and analytical measures |
| **CSV** | Source datasets |
| **Data Modeling** | Combining waiting-list data and specialty mapping |

---

## 📁 Dataset

The project uses the supplied healthcare waiting-list CSV files covering **2018–2021**.

### Outpatient Waiting List

- `Op_WL 2018.csv`
- `Op_WL 2019.csv`
- `Op_WL 2020.csv`
- `Op_WL 2021.csv`

These files contain fields including:

- `Archive_Date`
- `Specialty_HIPE`
- `Speciality`
- `Adult_Child`
- `Age_Profile`
- `Time_Bands`
- `Total`

### Inpatient / Other Waiting List

- `IN_WL 2018.csv`
- `IN_WL 2019.csv`
- `IN_WL 2020.csv`
- `IN_WL 2021.csv`

These files contain fields including:

- `Archive_Date`
- `Specialty_HIPE`
- `Specialty_Name`
- `Case_Type`
- `Adult_Child`
- `Age_Profile`
- `Time_Bands`
- `Total`

### Specialty Mapping

`Mapping_Specialty.csv` provides a mapping between individual specialties and broader **Specialty Groups**.

---

## 🔄 Data Preparation & Modeling

The project follows a typical BI workflow:

```text
Raw CSV Files
     ↓
Power Query
     ↓
Data Cleaning & Transformation
     ↓
Combine Multi-Year Data
     ↓
Specialty Mapping
     ↓
Data Model
     ↓
DAX Measures
     ↓
Interactive Power BI Dashboard
```

The yearly files are structured so that the data can be analyzed consistently across time. The specialty mapping adds a higher-level grouping that helps users analyze healthcare activity beyond individual specialties.

---

## 📌 Dashboard Structure

The Power BI report contains two main analytical views:

### 1. Summary Dashboard

<p align="center">
  <img src="https://github.com/VikrantPatel2/Healthcare/blob/06604290fe8a6230bfef4908e7ada52aec39ee9c/Summary.png" alt="Summary Dashboard" width="100%">
</p>

The Summary page provides a high-level view of the waiting-list situation.

### Key KPI

The dashboard displays:

- **Latest Month Wait List:** 704K
- **Previous Year Latest Month Wait List:** 624K

These KPIs provide a quick year-over-year comparison of the latest available waiting-list position shown in the report.

### Case Type Distribution

The dashboard breaks the waiting list into:

- Outpatient
- Day Case
- Inpatient

The case-type distribution is presented through a donut chart, making it easy to identify the largest contribution.

### Waiting Time Analysis

A stacked column chart analyzes waiting-list volume across time bands such as:

- 0–3 Months
- 3–6 Months
- 6–9 Months
- 9–12 Months
- 12–15 Months
- 15–18 Months
- 18+ Months

The visualization is further segmented by age profile.

### Specialty Analysis

The dashboard displays average/median waiting-list information for specialties, including examples such as:

- Anaesthetics
- Breast Surgery
- Cardiology
- Cardio-Thoracic Surgery

### Historical Trend

The bottom section tracks waiting-list movement over time, including separate trends for case types.

---

## 🔎 Detailed View

<p align="center">
  <img src="https://github.com/VikrantPatel2/Healthcare/blob/ab81b4b95deb4217abab1e722c92251831fc33a2/Detailed.png" alt="Detailed Dashboard View" width="100%">
</p>

The Detailed View provides a more granular representation of the waiting-list data.

Users can analyze the data using filters for:

- Archive Date
- Specialty
- Case Type
- Age Profile
- Time Band

The detailed table provides a structured view of waiting-list values by date, age profile, time band, and case type.

This page is particularly useful when a user wants to move from **high-level KPI analysis to detailed investigation**.

---

## 🎛️ Interactive Filters

The dashboard supports interactive filtering through slicers.

### Available filters include:

- **Archive Date**
- **Specialty Name**
- **Case Type**
- **Age Profile**
- **Time Bands**

Changing a filter dynamically updates the relevant dashboard visuals, allowing users to investigate specific segments of the waiting list.

---

## 📈 Key Analytical Areas

### Waiting List Volume

Monitor the overall number of patients on waiting lists and compare the latest period with the corresponding previous-year period.

### Waiting Time Bands

Identify how waiting-list volume is distributed across different waiting periods and detect the size of the long-wait population.

### Age Profile

Compare waiting-list patterns across:

- 0–15
- 16–64
- 65+

### Case Type

Analyze differences between:

- Outpatient
- Day Case
- Inpatient

### Specialty

Compare waiting-list pressure across healthcare specialties and specialty groups.

### Time Trends

Track how waiting-list volumes change across the reporting period from 2018 through 2021.

---

## 💡 Business Questions Answered

This dashboard is designed to answer questions such as:

- What is the latest waiting-list volume?
- How does the latest waiting list compare with the previous year?
- Which case type contributes the most to the waiting list?
- Which waiting-time band contains the largest volume?
- How does waiting-list volume differ across age groups?
- Which specialties show higher average/median waiting-list values?
- How has the waiting list changed over time?
- What happens to the waiting list when a specific specialty or time band is selected?
- How do detailed waiting-list values vary by archive date and case type?

---

## 📊 Dashboard KPIs & Visuals

| Component | Purpose |
|---|---|
| Latest Month Wait List | Current waiting-list KPI |
| PY Latest Month Wait List | Previous-year comparison |
| Case Type Donut Chart | Distribution by case type |
| Waiting Time Band Chart | Waiting volume by time band |
| Age Profile Breakdown | Compare age groups |
| Specialty Analysis | Specialty-level comparison |
| Historical Line Charts | Trend analysis |
| Detailed Table | Granular data investigation |
| Slicers | Interactive filtering |

---

## 📂 Project Structure

```text
Healthcare_Waiting_List_Dashboard/
│
├── README.md
│
└── assets/
    ├── dashboard-summary.png
    └── dashboard-detail.png
```

The original project data files can be kept alongside the Power BI `.pbix` file when publishing the complete project repository.

---

## 🚀 How to Use the Project

1. Install **Microsoft Power BI Desktop**.
2. Open the `Healthcare1.pbix` file.
3. Go to the **Summary** page for the overall analysis.
4. Use the slicers to filter the report.
5. Review KPIs and trend visuals.
6. Move to the **Detailed View** for granular analysis.
7. Experiment with different specialties, case types, age profiles, and waiting-time bands.

---

## 📌 Project Highlights

- Multi-year healthcare waiting-list analysis
- Interactive Power BI dashboard
- KPI-based reporting
- Year-over-year comparison
- Waiting-time band analysis
- Age-profile analysis
- Case-type analysis
- Specialty-level analysis
- Historical trend analysis
- Detailed filtered data view
- Power Query data preparation
- DAX-based analytical reporting

---

## 🧠 Skills Demonstrated

**Power BI:**  
Dashboard Design • Data Modeling • Slicers • Interactive Visuals • Drill-down Analysis

**Data Analytics:**  
Data Cleaning • Data Transformation • KPI Analysis • Trend Analysis • Comparative Analysis • Segmentation

**DAX:**  
Measures • Aggregations • Time-based Comparison • KPI Calculations

**Business Intelligence:**  
Healthcare Reporting • Operational Monitoring • Data Visualization • Decision Support

---

## 👨‍💻 Author

**Vikrant Patel**

Data Analyst | BI & Data Visualization

Interested in **Data Analytics, Business Intelligence, Financial Analytics, and Computational Biology**.

### Portfolio

- GitHub: https://github.com/VikrantPatel2
- LinkedIn: https://www.linkedin.com/in/vikrant-patel-8a5032286/

---

## 📜 Notes

The dashboard screenshots included in this README were generated from the supplied `Healthcare1.pdf` report export. The project description and terminology are based on the supplied Power BI report and CSV datasets.

