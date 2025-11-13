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
![ERD](images/data_model.png)

---

## 📊 Executive Summary (Platform-Aware)

The **Meta Ads Performance Analysis** for *RetailNova* highlights a marketing funnel that excels in **visibility and engagement** but loses efficiency in **conversions**.  

Across both platforms:
- **Total Impressions:** 216 K  **Clicks:** 25.4 K  **Engagements:** 29 K  
- **CTR 11.76 %** and **Engagement Rate 13.56 %** far exceed retail benchmarks (1 – 2 %), confirming highly effective creatives and targeting.  
- **Purchases 1.3 K**, **Conversion Rate 5.21 %**, and **Purchase Rate 0.61 %** reveal a sharp drop-off from engagement → purchase — likely caused by landing-page friction or offer misalignment.  

### Platform Highlights
| KPI | Facebook | Instagram | Observation |
|------|-----------|-----------|--------------|
| Impressions | Higher volume | Slightly lower | Facebook drives reach |
| CTR / ER | Strong | Strong | Both effective top-funnel |
| Conversion Rate | Moderate | Comparable / slightly lower | Similar funnel leakage |
| Engagement Mix | Balanced | Slightly higher on Stories | Instagram better for visuals |

### Key Takeaways
1. **Awareness & interest strong; conversion weak.**  
2. **Female 18 – 30 segment** dominates engagement — tailor creatives accordingly.  
3. **Video & Story ads** outperform all other formats.  
4. **Peak hours:** 3 PM – 8 PM; schedule ads accordingly.  
5. **Platform split:** Use Facebook for reach, Instagram for conversion-driven storytelling.

![Dashboard Overview](images/dashboard_overview.png)

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
