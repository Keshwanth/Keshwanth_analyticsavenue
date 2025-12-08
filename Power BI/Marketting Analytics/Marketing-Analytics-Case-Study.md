# Marketing Analytics: A Power BI Dashboard Case Study

## Introduction: What is Marketing Analytics?

Marketing analytics is how brands use data from every ad impression, click, and conversion to understand what is working and what is not. When an ad runs on Instagram, YouTube, or Google, platforms record how many people saw it (reach), how many clicked (CTR), what each click cost (CPC), and how many finally became customers (CAC or cost per acquisition). Instead of guessing, marketers use these metrics to refine targeting, creatives, and budgets so they can spend less and earn more.

In this project, a Power BI dashboard was built to analyze performance of digital campaigns promoting analytics programs such as SQL Skills Training, Python for Beginners, and AI & ML Foundations. The objective was to turn raw ad-level data into clear insights on which campaigns, audiences, and cities drive the most conversions at the best cost.

## How Modern Marketing Analytics Works

Modern marketing analytics typically runs on a cloud-based stack that pulls data from multiple sources, processes it, and surfaces insights through dashboards and models. Data flows from ad platforms and application events into storage, where it can then power descriptive reports, predictive models, and even automated alerts for campaign optimization.

AI and advanced analytics add several benefits on top of basic reporting:

- **Enhanced Customer Insights**: Discovering hidden patterns in large volumes of customer behavior data enables hyper-personalized marketing strategies.
- **Real-Time Optimization**: Live performance data is used to tweak bids, creatives, and audiences while campaigns are running.
- **Smarter Budget Allocation**: Identifying the most effective channels and segments ensures resources go to high-performing areas.
- **Predictive Analytics**: Forecasting trends and likely outcomes of different strategies enables proactive decision-making.
- **Improved ROI via Automation**: Repetitive monitoring and optimization tasks are automated, saving time and resources.

## Understanding the Full-Funnel Measurement Framework

Marketing success is not measured at a single point but across multiple stages. The full-funnel approach divides the customer journey into three critical phases:

### Top-of-Funnel (TOFU)
TOFU metrics focus on brand awareness and initial engagement:
- Unique reach: How many distinct people see the ad?
- Impressions: Total ad views, regardless of uniqueness.
- Completion rate: For video ads, what percentage watch to completion?
- Click-Through Rate (CTR): What share of viewers click the ad?

### Middle-of-Funnel (MOFU)
MOFU metrics indicate growing purchase intent:
- Detail page views: Are viewers exploring product/service pages?
- New-to-brand percentage: What share are first-time visitors?
- Branded search index: Are people searching for your brand after seeing ads?

### Bottom-of-Funnel (BOFU)
BOFU metrics capture the conversion and profitability stage:
- Conversion rate: What share of clickers take the desired action (purchase, sign-up)?
- Orders or units sold: Actual business outcome.
- Return on Advertising Spend (ROAS): Revenue generated per rupee spent.
- Advertising Cost of Sales (ACOS): How much is spent to drive one sale?
- Customer Acquisition Cost (CAC): Average cost to acquire one new customer.

## Dataset Overview

The dataset used in this analysis is a detailed ad export containing the following key fields:

**Campaign Information**: Campaign name, Page (brand), Day, and Delivery status.

**Audience Attributes**: Age (grouped into bins), Gender, and City.

**Performance Metrics**:
- Impressions: Total number of ad views.
- Reach: Unique number of people who saw the ad.
- Link clicks: Number of clicks on the ad link.
- Results: Number of conversions (sign-ups, registrations, or purchases).

**Financial Metrics**:
- Amount spent (INR): Total ad spend.
- CTR: Click-through rate (link clicks ÷ impressions).
- CPC: Cost per click (spend ÷ link clicks).
- CPM: Cost per thousand impressions (spend ÷ impressions × 1000).

Each row represents the performance of a specific ad or ad set for a given audience slice and time period, providing full visibility from exposure to conversion.

## Building the Power BI Marketing Dashboard

### Data Preparation and Measures

After importing the Excel file into Power BI, key columns were validated and renamed where necessary. Core measures were created to enable strategic analysis:

- **Total Results**: Sum of all conversions across the dataset.
- **Total Spend**: Total amount spent on ads in INR.
- **Total Impressions**: Total number of ad impressions.
- **Total Link Clicks**: Total number of ad link clicks.
- **Avg Cost per Result**: Total spend divided by total results (a key efficiency metric).
- **CTR %**: Link clicks divided by impressions, expressed as a percentage.
- **CPM**: Spend per 1,000 impressions.
- **Top Campaign**: A measure that dynamically returns the campaign name with the highest total results.

### Dashboard Layout and User Experience

A single 1920×1080 canvas was designed to keep the entire story on one page, making it ideal for decision-makers, presentations, and portfolio reviews.

**Filtering Layer**: The top section contains four dropdown slicers—Campaign, Page, City, and Delivery Status—allowing users to instantly slice the entire dashboard by brand, geography, delivery performance, and campaign selection.

**KPI Summary**: Below the slicers, six key metric cards display:
- Total Results
- Total Spend (in INR)
- Avg Cost per Result
- CTR %
- Total Impressions
- Top Campaign (dynamically updated)

**Visual Analytics Layer**: Six complementary charts tell the complete performance story:

1. **Campaign Performance**: A horizontal bar chart ranking campaigns by total results, with campaigns sorted in descending order of performance. This immediately identifies the top and bottom performers.

2. **Cost per Result by Campaign**: A column chart using a light cyan color palette, emphasizing efficiency where lower values are better. The subtitle "(Lower is better)" reinforces this insight.

3. **Monthly Trend**: A multi-line chart showing how impressions, reach, and results evolve across months, revealing seasonality and campaign timing patterns.

4. **Overall Funnel**: Horizontal bars showing the drop-off from Impressions → Reach → Clicks → Link clicks → Results, with decreasing shades of cyan to visually represent the narrowing funnel. The subtitle "(Shows total volume at each stage)" clarifies the purpose.

5. **Share of Results by Age Group**: A donut chart displaying the percentage of total results contributed by each age demographic, helping identify the most valuable audience segments.

6. **Top 10 Cities by Results**: A column chart showing the geographic distribution of conversions, with city labels angled for readability and filtering to the top 10 for clarity.

## Key Insights from the Dashboard

### Campaign Performance
A small group of campaigns—particularly AI & ML Foundations and SQL Skills Training—contribute a disproportionate share of total results while maintaining a competitive average cost per result. This indicates strong product-market fit for these offerings and suggests they warrant increased budget allocation.

### Efficiency Metrics
The cost-per-result visualization makes it immediately clear which campaigns justify their spend and which may need creative overhauls or audience refinement. Campaigns with high spend but weak efficiency should be prioritized for A/B testing or potentially paused.

### Temporal Patterns
The monthly trend view reveals that impressions and reach ramp up over time with a clear peak in mid-year months, followed by a decline. Results follow a similar pattern but with more variability, suggesting that conversion rate changes across months independent of reach.

### Funnel Performance
The overall funnel clarifies that while the dataset captures millions of impressions and a strong reach, only a small fraction progress through to clicks, link clicks, and final results. The overall CTR of approximately 3.35% is typical for education-focused ads, and the gap between link clicks and results suggests a landing page or sign-up process optimization opportunity.

### Demographic Insights
The 20–30 age group is the dominant contributor to conversions, accounting for over two-thirds of total results. This suggests that younger, digitally native audiences are most responsive to analytics education offerings.

### Geographic Performance
Cities like Bengaluru, Mumbai, and Hyderabad consistently appear at the top of the performance list by results. These metros likely represent higher concentrations of IT professionals and career-changers interested in data science and analytics skills.

## Recommendations for Campaign Optimization

### Budget Reallocation
Shift budget from low-performing campaigns and demographics toward high-performing ones. Specifically, increase investment in campaigns driving results at or below the median cost per result, particularly in top-performing cities.

### Audience Refinement
Create audience segments specifically targeting the 20–30 age group in Tier-1 cities. Consider developing tailored creatives and landing pages for this demographic to increase conversion rates further.

### Creative and Messaging Optimization
Conduct A/B tests on underperforming campaigns, varying ad creatives, headlines, landing page designs, and call-to-action messaging. Pay special attention to campaigns with high reach but low CTR, as they may be reaching the right audience but not compelling them to click.

### Funnel Analysis and Improvement
The significant drop-off from link clicks to results suggests friction in the sign-up or checkout process. Review the landing page experience, form complexity, and checkout flow to identify and eliminate barriers to conversion.

### Seasonal Campaign Planning
Leverage the observed seasonality by front-loading budget toward high-performing months and reducing spend during lower-performance periods. Consider running promotional campaigns or new course launches during the identified peak months.

## Future Enhancements and Next Steps

### Integration of Revenue Data
Extend the dashboard with downstream business metrics such as enrollment confirmation, course completion rates, and actual revenue per campaign. This would enable calculation of true Bottom-of-Funnel metrics like ROAS (Return on Advertising Spend), ACOS (Advertising Cost of Sales), and CAC (Customer Acquisition Cost).

### Predictive Analytics
Implement machine learning models to forecast future performance based on historical patterns, predict which audience segments are most likely to convert, and automatically recommend budget allocation changes.

### Unified Full-Funnel Measurement
Integrate TOFU, MOFU, and BOFU data into a single cohesive dashboard, enabling comparison of performance at each funnel stage and identification of where optimization efforts would have the highest impact.

### Real-Time Alerting
Set up automated alerts to notify the marketing team when key metrics—such as CTR or cost per result—deviate significantly from expected ranges, enabling rapid response to underperforming campaigns.

### Attribution Modeling
Implement multi-touch attribution to understand how different campaigns and touchpoints combine to drive conversions, moving beyond last-click attribution to a more sophisticated understanding of the customer journey.

## Conclusion

This Power BI marketing analytics dashboard demonstrates how data visualization and interactive analytics can transform raw ad performance data into actionable business intelligence. By combining TOFU and BOFU metrics with demographic and geographic segmentation, the dashboard enables both high-level strategic decisions (which campaigns to fund) and tactical optimizations (which audiences to target, which creatives to test).

The insights derived—particularly the dominance of the 20–30 age group, the strong performance of Tier-1 cities, and clear efficiency differences between campaigns—provide a solid foundation for improving marketing ROI. When extended with revenue data and predictive analytics, this framework becomes a complete full-funnel marketing analytics system capable of guiding both budget allocation and creative strategy.

For professionals building their analytics portfolio, this project demonstrates proficiency in data visualization, DAX formula development, multi-layered dashboard design, and the ability to translate business questions into clear visual narratives—skills that are increasingly valuable in marketing technology and business analytics roles.

---

**Document prepared as a case study of marketing analytics dashboard design and interpretation. All metrics and insights derived from real ad performance data analyzed in Power BI.**
