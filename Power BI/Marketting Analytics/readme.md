# Marketing Analytics Dashboard – Power BI

This project is a marketing analytics case study built in Power BI to analyze the performance of paid campaigns promoting data and analytics programs. It turns raw ad export data into an interactive dashboard that helps answer which campaigns, audiences, and cities drive the best results at the lowest cost.

---

## Files in this folder

- `Marketing Analytics Dashboard.pbix` – Main Power BI report.  
- `Marketing Analytics Dashboard Snapshot.png` – Screenshot of the final dashboard for quick preview.  
- `Blog - Marketing Analytics.pptx` – Slide deck / blog visuals explaining the project and insights.  
- `Marketing-Analytics.xlsx` – Source dataset used to build the Power BI model (ad performance export).

> Open `Marketing-Analytics.xlsx` in Power BI Desktop as the data source if you want to rebuild or extend the report.

---

## Dataset

The dashboard is built on an ad performance dataset with:

- **Campaign information**: campaign name, page, day, delivery status  
- **Audience attributes**: age (binned), gender, city  
- **Performance metrics**: impressions, reach, link clicks, results (conversions)  
- **Cost metrics**: amount spent (INR), CTR, CPC, CPM  

Each row represents performance for a campaign/ad set and audience slice over a given period.  

> If you fork or reuse this project, ensure the dataset is handled responsibly and anonymized where required.

---

## Dashboard overview

The report is a single-page Power BI dashboard with:

- Slicers for **Campaign**, **Page**, **City**, and **Delivery Status**  
- KPI cards for **Total Results**, **Total Spend**, **Avg Cost per Result**, **CTR %**, **Total Impressions**, and **Top Campaign**  
- Visuals:
  - Campaign performance (results by campaign)  
  - Cost per result by campaign  
  - Monthly trend of impressions, reach, and results  
  - Overall funnel: impressions → reach → clicks → link clicks → results  
  - Share of results by age group  
  - Top 10 cities by results  

These visuals together give a full view of campaign performance, efficiency, funnel drop‑offs, and audience/geography behavior.

---

## Key questions answered

The analysis focuses on practical marketing questions:

- Which campaigns deliver the highest reach and conversions?  
- Which campaigns are most cost‑efficient (lowest cost per result)?  
- Which age groups and cities perform best?  
- How do impressions, reach, and results trend over time?  
- Where is spend high but performance relatively weak, indicating optimization opportunities?  

---

## How to use the report

1. Clone or download this repository.  
2. Open `Marketing-Analytics.xlsx` in **Power BI Desktop** (if building from scratch) or open `Marketing Analytics Dashboard.pbix` directly.
3. If Power BI asks for a file path, relink the PBIX to `Marketing-Analytics.xlsx` in the same folder.  
4. Use the slicers at the top of the report to filter by campaign, page, city, or delivery status.  
5. Hover over visuals to see detailed tooltips such as cost per result and CTR %.  

You can modify measures or add new visuals (for example, ROAS or CAC) to extend the analysis.

---

## Skills demonstrated

- Data modeling and DAX measures (CTR %, Avg Cost per Result, CPM, Top Campaign)  
- Dashboard layout and UX design in Power BI  
- Marketing analytics concepts: TOFU/BOFU metrics, funnel analysis, audience and geo segmentation
- Storytelling through KPIs, charts, and a supporting blog/case study

---

## About this project

This project is part of a broader analytics portfolio showcasing the ability to turn marketing data into clear, actionable insights using Power BI and core marketing analytics concepts.
