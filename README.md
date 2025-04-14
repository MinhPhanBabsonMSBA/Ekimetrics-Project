# 📊 Marketing Mix Modeling for Hope Street Cosmetics

Welcome to our group project repository for **Marketing Mix Modeling (MMM)**, developed as part of the MKT6300-02 course (Spring 2025). In this project, we act as marketing analytics consultants from **Ekimetrics**, advising **Hope Street Cosmetics**, a global beauty brand, on the effectiveness of its marketing efforts.

---

## 🧴 About the Client

**Hope Street Cosmetics** is a high-end beauty company known for its luxury skincare and makeup products. Their global sales channels include:

- 🏬 Brand-Owned Stores  
- 🖥️ Brand Website (Brand.com)  
- 🛍️ Specialty Multi (e.g. Sephora, Ulta)  
- 🏢 Department Stores (Retailer Brick & Mortar)  
- 🧾 Retailer Websites (Retailer.com)

Despite increasing marketing budgets, the brand has seen slower sales growth, prompting the CMO to better understand:

- The **ROI of various marketing tactics**  
- The **impact of COVID-19** on revenue  
- The **baseline (unaffected) level of sales**  
- The **real contribution of promotional efforts**

---

## 🧭 Project Objective

To help Hope Street Cosmetics make data-driven marketing decisions, we applied the **Marketing Mix Modeling** methodology to assess:

- The efficiency of different marketing channels  
- Optimal budget allocation  
- Business outcomes with and without promotions  
- Strategy refinements based on campaign ROI

---

## 🛠️ Project Methodology

The project followed a 4-week consulting-style engagement involving:

1. **🔍 Week 1: Introduction & Discovery**  
   - Industry research  
   - Mini-discovery document summarizing the beauty sector  

2. **🧹 Week 2: Data Treatment**  
   - Clean and preprocess data using Python in Jupyter Notebooks  
   - Tasks include:
     - Weekly outdoor campaign metrics  
     - Imputing missing Facebook data  
     - Identifying YouTube campaign outliers  
   - Output: `final_database.csv`  

3. **📈 Week 3: Modeling**  
   - Build MMM in Python  
   - Evaluate campaign ROI using Ekimetrics’ Excel Analysis Workbook  
   - Final deliverables:
     - `Modeling_Workbook.ipynb`  
     - `Analysis_Workbook.xlsx`  

4. **🎤 Week 4: Final Deliverable**  
   - Present findings and recommendations to stakeholders  
   - Interpret model outputs and provide actionable insights  
   - Business casual group presentation with Ekimetrics  

---

## 📊 Modeling Outcomes

During the modeling phase, we built a linear regression-based Marketing Mix Model using weekly sales and marketing data for **Hope Street Cosmetics** from January 2019 to December 2020. The key outcomes of the model include:

### 🔢 Top Features Impacting Sales

| Variable                          | Coefficient Estimate | Interpretation                             |
|-----------------------------------|-----------------------|---------------------------------------------|
| `blackfriday_2019`                | \$4.07M              | Strong positive lift from Black Friday 2019 |
| `cyber_monday`                    | \$3.24M              | Major digital sales driver during holiday season |
| `flash_sale_promo`               | \$2.52M              | Effective short-term revenue driver         |
| `covid_trend`                    | +57,590              | Captures general pandemic impact            |
| `fbig_imp` (Facebook Impressions)| +0.037               | Scaled impact of digital campaigns          |
| `bing_brand_search_clicks`       | +22.0                | High ROI for branded search                 |
| `tv_pure_spend`                  | +1.10                | Consistent contributor to baseline sales    |

> *Note: All features were standardized for modeling purposes. T-stats were used to assess significance. Some variables had zero or near-zero coefficients, indicating limited or negative contribution.*

### 📉 Baseline vs Incremental Sales

The model decomposed total weekly sales into:

- **Baseline Sales (No Advertising)** – the natural demand from loyal or organic customers  
- **Incremental Sales** – the uplift caused by paid media, promotions, and campaigns  

This split helps the brand understand how much of its revenue is organically generated vs driven by marketing efforts.

### 📈 ROI Evaluation with Excel

Using the **Ekimetrics ROI Analysis Workbook**, we analyzed the return on investment (ROI) for major channels:

| Channel/Activity                  | ROI ($ per $1 Spend) |
|----------------------------------|-----------------------|
| Flash Sale Promotions            | ~4.0                 |
| Google Brand Search              | ~3.2                 |
| Facebook Impressions             | ~2.5                 |
| Outdoor Campaigns                | ~1.8                 |
| Print & TV Campaigns             | Mixed (timing-dependent) |

These findings allow the brand to shift budget toward high-return activities and make informed tradeoffs when planning future campaigns.

---

## 📁 Project Structure
Ekimetrics Project/
│
├── data/
│   └── final_database.csv              # Cleaned dataset for modeling
│
├── notebooks/
│   ├── outdoor_campaigns.ipynb         # Weekly metrics for outdoor campaigns
│   ├── facebook_imputation.ipynb       # Missing value treatment
│   ├── youtube_outliers.ipynb          # Outlier handling
│   └── Modeling_Workbook.ipynb         # Final marketing mix model
│
├── reports/
│   └── beauty_sector_summary.pdf       # Industry discovery document
│
├── analysis/
│   └── Analysis_Workbook.xlsx          # ROI & scenario evaluation
│
└── presentation/
└── Final_Presentation.pdf          # Business presentation to stakeholders
---

## 🧪 Tools Used

- **Python (Jupyter Notebooks)** – Data treatment and model building  
- **Pandas, NumPy, Matplotlib** – Data manipulation and exploratory analysis  
- **Excel (Ekimetrics Workbook)** – ROI interpretation and scenario planning  
- **Google Docs / MS Word** – Industry research & reporting  
- **PowerPoint / PDF** – Business presentation materials  

---

## 📆 Timeline

| Week | Focus Area               | Deliverables                         |
|------|--------------------------|--------------------------------------|
| 1    | Introduction & Discovery | Beauty Industry Report               |
| 2    | Data Treatment           | 4 Notebooks + Final Database         |
| 3    | Modeling                 | Modeling Notebook + Excel Workbook   |
| 4    | Final Deliverable        | Final Presentation                   |

---

## 🏁 Final Outcome

Our analysis helped Hope Street Cosmetics:

- Quantify the ROI of key marketing tactics  
- Decompose sales into organic vs. promotional drivers  
- Isolate the impact of COVID-19 on consumer behavior  
- Inform better budgeting decisions for future planning  

---
