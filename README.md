# Applicant Insights Report – Descriptive Analytics

This project provides a data-driven exploration of applicants to a national STEM enrichment program. It examines demographics, socioeconomic status, school types, geographic reach, enrollment, and program completion to inform strategy and outreach.

---

## ✨ Features

- Analysis of applicant data covering **2022–2025**, combining internal registration files with external datasets (NCES, U.S. Census / ACS).  
- Deep cleaning and harmonization across years: standardizing school names, addresses, demographic fields; handling duplicates; classifying school type (public/private/charter/unknown).  
- Enrichment with socioeconomic indicators via ZIP-code median household income (ACS) and creation of SES tiers.  
- Visual and statistical summaries of:  
  - Geographic distribution of applicants (states, cities, maps)  
  - Demographic profiles (gender, race/ethnicity, grade, age)  
  - School type distribution  
  - Program completion rates (overall and stratified by demographic and SES variables)  
  - Trends over time (volume, completion, demographic shifts)  

---

## 📊 Example Outputs

- 🌐 [View HTML Report](https://isaacbmichael.github.io/EDA-Applicant-Report/eda_report.html)  
- 📄 [Download PDF Report](LINK_TO_PDF_IF_AVAILABLE)  

---

## 📂 Repository Contents

- `eda_report.Rmd` – Main R Markdown notebook that generates the report.  
- `eda_report.html` – Interactive / viewable HTML version of the full report.  
- (Optional) `eda_report.pdf` – Printable / shareable PDF version.  
- Supporting data files: normalized applicant datasets, cleaned/enriched data, ACS / NCES sources.  
- Visual assets: charts such as geographic maps, demographic distributions, SES analyses, trend graphs.  

---

## ⚙️ Methodology (Summary)

- **Data Sources**: Internal application files (2022–2025); external school directories (NCES), and ACS median income by ZIP.  
- **Cleaning & Harmonization**: Standardizing variable names across years; resolving naming inconsistencies; deduplication (preferring most complete records).  
- **School Classification**: Using NCES lookup + fallback heuristics for unmatched schools.  
- **Socioeconomic Status (SES)**: Using ACS 5-year estimates for median household income by ZIP code → dividing into income tiers.  
- **Exploratory Analysis**: Visual and summary statistics to uncover demographic, geographic, SES, and program completion patterns; trend analysis over time.  

---

## 🔍 Key Findings & Recommendations

- **Findings**:  
  - Strong geographic concentration in coastal and some southern states; gaps elsewhere.  
  - Demographic imbalance: majority Asian, male; lower representation of Black, Hispanic/Latino, and underrepresented groups.  
  - High participation from high-income ZIPs; relatively few low-income applicants despite financial aid availability.  
  - Overall program completion is high, though some disparities by race/SES/gender etc.  

- **Recommendations**:  
  - Increase outreach in underrepresented states / non-coastal regions.  
  - Partner with schools / community groups in lower-income areas; emphasize free/reduced cost & needs-based aid.  
  - Improve registration form to capture consistent demographic & school data to reduce “unknowns.”  
  - Monitor completion gaps and consider targeted support / mentoring for groups showing lower completion.  

---

## ⚠️ Disclaimer

This project is for educational and operational insight purposes. It does **not** constitute official policy; the analysis is based on proxy metrics (e.g. ZIP-level income) and available data. Data limitations should be considered when interpreting conclusions.

---

© 2025 Isaac B. Michael • [Email](mailto:isaac.b.michael@gmail.com) • [LinkedIn](https://www.linkedin.com/in/isaacbmichael) • [GitHub](https://github.com/isaacbmichael)
