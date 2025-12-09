# Marketing Analytics Dashboard – Power BI

This project is a marketing analytics case study built in Power BI to analyze the performance of paid campaigns promoting data and analytics programs. It turns raw ad export data into an interactive dashboard that helps answer which campaigns, audiences, and cities drive the best results at the lowest cost.

---

## Files in this folder

- `Marketing Analytics Dashboard.pbix` – Main Power BI report.  
- `Marketing Analytics Dashboard Snapshot.png` – Screenshot of the final dashboard for quick preview.  
- `Blog - Marketing Analytics.pptx` – Slide deck / blog visuals explaining the project and insights.  

*(If your filenames differ, adjust the names above.)*

---

## Dataset

The dashboard is built on an ad performance dataset with:

- Campaign information: campaign name, page, day, delivery status  
- Audience attributes: age (binned), gender, city  
- Performance metrics: impressions, reach, link clicks, results (conversions)  
- Cost metrics: amount spent (INR), CTR, CPC, CPM  

Each row represents performance for a campaign/ad set and audience slice over a given period.

> Note: The raw dataset is not included in this repository to respect data privacy and ownership.

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

---

## Key questions answered

The analysis focuses on practical marketing questions:

- Which campaigns deliver the highest reach and conversions?  
- Which campaigns are most cost-efficient (lowest cost per result)?  
- Which age groups and cities perform best?  
- How do impressions, reach, and results trend over time?  

---

## How to use the report

1. Open `Marketing Analytics Dashboard.pbix` in **Power BI Desktop**.  
2. Use the slicers at the top to filter by campaign, page, city, or delivery status.  
3. Hover over visuals to see detailed tooltips (cost per result, CTR %, etc.).  
4. Use the visuals to compare campaigns, audiences, and locations and derive optimization ideas.

---

## Skills demonstrated

- Data modeling and DAX measures (CTR %, Avg Cost per Result, CPM, Top Campaign)  
- Dashboard layout and UX design in Power BI  
- Marketing analytics concepts: TOFU/BOFU metrics, funnel analysis, audience and geo segmentation

This project is part of a broader analytics portfolio focused on turning marketing data into clear, actionable insights.
