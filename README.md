# RetailNova-AD-Performance-Analysis
# 🧠 RetailNova Meta Ads Performance Optimization (Facebook & Instagram)

## 🏢 Project Background
**RetailNova** is a global e-commerce brand specializing in lifestyle and fashion products.  
In **June 2025**, the marketing team invested **$2.5 million** in paid advertising campaigns across **Facebook** and **Instagram**.  

As part of the Data Analytics team, I developed a unified reporting solution to:
- Measure campaign performance across awareness, engagement, and conversion stages.  
- Compare Facebook vs Instagram efficiency.  
- Identify actionable optimization opportunities for ad creatives, targeting, timing, and budget allocation.

---

## 🧮 Data Structure & Model
The project database includes four core tables and one parameter table used for dynamic measures in Power BI.

| Table | Description |
|--------|--------------|
| **ads** | Ad-level details: platform, ad type, target gender, target age group, linked campaign ID. |
| **ad_events** | Fact table capturing user interactions (Impression, Click, Share, Comment, Purchase). |
| **campaigns** | Campaign metadata including total budget and active dates. |
| **users** | Demographic and geographic attributes of targeted users. |
| **Select Dynamic Measure** | *Disconnected parameter table* used for dynamic metric switching inside Power BI (not joined in the ERD). |

**Entity Relationship Diagram**
![ERD](https://github.com/dev-laveshSharma/RetailNova-AD-Performance-Analysis/blob/main/screenshot/Data%20Model.png)

---

## 🧾 Executive Summary 

The **Meta Ads Performance Analysis** for *RetailNova* provides a comprehensive evaluation of advertising effectiveness across **Facebook** and **Instagram**.

Across both platforms, RetailNova’s campaigns demonstrated **strong awareness and engagement** but revealed **conversion inefficiencies** toward the end of the funnel.  
The analysis focuses on key funnel KPIs — from impressions and clicks to purchases and conversion rates — to understand how effectively each platform drives users from visibility to action.

### 📊 Platform KPI Comparison

| **Metric** | **Facebook** | **Instagram** | **Insight / Takeaway** |
|-------------|--------------|----------------|-------------------------|
| **Impressions** | 216 K | 123.8 K | Facebook delivers ~75 % higher reach — ideal for top-funnel awareness. |
| **Clicks** | 25.4 K | 14.7 K | Facebook attracts more user actions; stronger ad visibility overall. |
| **Engagements** | 29.3 K | 16.8 K | Both platforms are highly engaging; Instagram performs better relative to reach. |
| **Purchases** | 1.3 K | 708 | Facebook generates higher total conversions; both share similar efficiency gaps. |
| **CTR (Click-Through Rate)** | 11.76 % | 11.86 % | Nearly identical CTRs — ad campaigns effective across both channels. |
| **Engagement Rate** | 13.56 % | 13.60 % | Excellent audience resonance; content appeals equally well. |
| **Conversion Rate** | 5.21 % | 4.82 % | Slightly stronger post-click conversion on Facebook; mid-funnel leakage persists. |
| **Purchase Rate** | 0.61 % | 0.57 % | Low overall efficiency from reach to purchase — optimize landing pages & retargeting. |
| **Top Ad Formats** | Video / Carousel | Video / Stories | Instagram Stories excel in engagement; Facebook remains consistent across formats. |

These results show that RetailNova’s **ad creatives and targeting strategies outperform industry benchmarks** (average CTR ~1–2 %), confirming exceptional top-funnel performance.  
However, the drop-off between engagement and purchase highlights a **conversion leakage**, likely due to landing-page experience, offer alignment, or retargeting gaps.

### Additional Insights
- **Demographics:** Female users (**43 %**) aged **18–30** represent the most engaged audience segment across both platforms.  
- **Geographies:** **India and the US** generate the highest engagement volume, while **Germany and the UK** contribute higher-value conversions.  

### Summary & Impact
In conclusion, RetailNova’s Meta campaigns achieve **strong audience resonance and brand visibility** but face **low purchase efficiency**.  
By enhancing post-click user experiences, implementing smarter retargeting strategies, and tailoring creative formats by platform, RetailNova can realize an estimated **20–25 % uplift in ROI** without increasing overall marketing spend.

<p align="center">
  <img src="https://github.com/dev-laveshSharma/RetailNova-AD-Performance-Analysis/blob/main/screenshot/Facebook%20Insights.png" alt="Facebook Dashboard" width="48%" />
  <img src="https://github.com/dev-laveshSharma/RetailNova-AD-Performance-Analysis/blob/main/screenshot/Instagram%20Insights.png" alt="Instagram Dashboard" width="48%" />
</p>

<p align="center">
  <em>Figure: Facebook (left) and Instagram (right) Meta Ad Performance Dashboards</em>
</p>


---

## 🔍 Insights Deep Dive

> *Approach – Each category includes overall and platform-filtered (Facebook / Instagram) visuals to detect both universal and platform-specific trends.*

### 🧍‍♀️ Category 1 – Audience Demographics
**Overall Findings**
- Females ≈ 43 % of engagements vs 22 % males.  
- Core audience = 18 – 30 yrs.  
- **Action:** Focus creatives & offers on young female customers.  

**Platform View**
- Similar demographic structure across both platforms.  
- Instagram slightly skews younger (< 25 yrs).  

![Gender – Overall](images/category1_gender_overall.png)
![Gender – Facebook](images/category1_gender_facebook.png)
![Gender – Instagram](images/category1_gender_instagram.png)
![Age – Overall](images/category1_age_overall.png)

---

### 🌍 Category 2 – Geographic Insights
- Top markets: **India & US** (high volume), **Germany & UK** (high value).  
- **Action:** Run high-reach campaigns in India / Brazil; premium conversions in Europe.  
- Platform trend: both show consistent geography ranking; Instagram engagement slightly denser in urban markets.  

![Geo Map Overall](images/category2_map_overall.png)
![Geo Facebook](images/category2_map_facebook.png)
![Geo Instagram](images/category2_map_instagram.png)

---

### ⏰ Category 3 – Time Trends
- Weekly engagement stable (no sharp drops).  
- Hourly peaks 3 PM – 8 PM → ideal ad delivery window.  
- Calendar heatmap shows spikes around 19–21 & 25–27 June → promotion impact.  
- Platform comparison: both follow similar patterns; Facebook engages earlier afternoon, Instagram later evening.  

![Weekly Trend Overall](images/category3_weekly_overall.png)
![Hourly Trend Overall](images/category3_hourly_overall.png)
![Calendar Heatmap](images/category3_calendar_overall.png)

---

### 🎬 Category 4 – Ad Type Performance
| Ad Type | CTR | Conv Rate | Eng Rate | Takeaway |
|----------|-----|-----------|-----------|-----------|
| Video | **11.8 %** | **5.6 %** | **13.7 %** | Best overall |
| Stories | 11.3 % | 5.2 % | 13.6 % | Strong secondary |
| Image | 11.2 % | 4.9 % | 13.5 % | Moderate |
| Carousel | 11.1 % | 5.1 % | 13.4 % | Stable |

- **Platform nuance:** Instagram Stories & Videos excel; Facebook performs steady across formats.  
- **Action:** Shift ≈ 30 % budget to video & story formats.  

![Ad Type Overall](images/category4_adtype_table_overall.png)
![Ad Type Facebook](images/category4_adtype_facebook.png)
![Ad Type Instagram](images/category4_adtype_instagram.png)

---

### 🔁 Platform Comparison Summary
![Platform KPI Compare](images/platform_comparison_metrics.png)

- Facebook = broader reach, stable CTR.  
- Instagram = higher story engagement, comparable conversion.  
- **Recommendation:** Run cross-platform complementary strategy — awareness via Facebook, conversion via Instagram.

---

## 💡 Recommendations

| Observation | Recommendation |
|--------------|----------------|
| High CTR but low purchases | Improve landing page UX and retarget high-intent clickers. |
| Dominant female 18 – 30 segment | Build persona-driven content & influencer collabs. |
| Evening engagement peak | Allocate budget 3 PM – 8 PM to maximize ROI. |
| India / Brazil volume; UK / Germany value | Segment campaigns by goal (awareness vs premium conversion). |
| Video & Stories outperform | Increase budget share for these formats. |
| Platform differences | Maintain distinct Facebook and Instagram playbooks. |

---

## 🧰 Tech Stack & Files
**Tools:** SQL (for data prep & KPIs), Power BI (for model + visuals), Excel (for validation).  

- [`/SQL/SQL_Cleaning_Queries.sql`](SQL/SQL_Cleaning_Queries.sql)  
- [`/SQL/SQL_Business_Queries.sql`](SQL/SQL_Business_Queries.sql)  
- [`/Dashboard/Dashboard.pbix`](Dashboard/Dashboard.pbix)  
- [**Interactive Power BI Dashboard →**](https://app.powerbi.com/...) *(add your link)*  

---

## 🧾 Supporting Documents
| File | Description |
|------|--------------|
| `Business Requirements Document.pdf` | Defines KPIs and visual specs. |
| `Dashboard Insights.pdf` | Insight summary per visual. |
| `Project Explanation in Interview.pdf` | Verbal walk-through. |
| `Data Dictionary.xlsx` | Column-level metadata. |
| `Presentation.pptx` | Executive slide deck. |

---

## 👤 Author
**Lavesh Sharma**  
Data Analyst | Marketing Analytics | Power BI | SQL  
[LinkedIn](https://linkedin.com/in/your-profile) • [Portfolio](https://github.com/your-profile)
