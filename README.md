

# E-News Express A/B Testing Analysis

This project presents an end-to-end analysis of the **E-News Express case study**, highlighting the business problem, data-driven insights, and strategic recommendations derived from an A/B test conducted using **Python (Seaborn, SciPy/Scikit-learn)** and **Excel**.

---

## Business Problem

E-News Express, an online news portal, has experienced a decline in monthly subscribers. To address this, the company introduced a **new landing page** aimed at improving user engagement and overall experience.

###  Key Objectives

- **User Engagement** → Measured by time spent on the page  
- **Conversion Rate** → Percentage of visitors who subscribe  
- **Language Preferences** → Behavioral differences across:
  - English
  - Spanish
  - French users  

---

##  Business Recommendations

Based on the analysis, the following strategies are recommended:

###  1. Deploy the New Landing Page
The new page significantly improves both engagement and conversion → **roll out fully**.

###  2. Technical Optimization
- Faster load times  
- High-quality visuals  
- Short, readable content  
- Clear key takeaways  

###  3. Mobile-First Design
Optimize for smartphones, aligning with modern user behavior.

###  4. Content Hyper-Localization
- Maintain English, Spanish, and French  
- Add **location-specific content** for relevance  

###  5. Behavioral Segmentation
Segment users by:
- Engagement level (high vs. low interaction)  
- New vs. returning users  

###  6. Dynamic Customization
Use dynamic content blocks to:
- Reduce friction  
- Improve retention  

---

##  Solution Methodology

A structured data science workflow was followed:

1. **Data Setup**
   - 100 observations  
   - No missing values or duplicates  

2. **Exploratory Data Analysis (EDA)**
   - Univariate and bivariate analysis  

3. **Visualization**
   - Histograms  
   - Boxplots  
   - Bar charts (via Seaborn)  

4. **Hypothesis Testing**
   - Significance level: **α = 0.05**  
   - Tests used:
     - T-tests  
     - Z-tests  
     - ANOVA  
     - Chi-Square  

---

##  EDA Insights & Data Overview

###  Dataset Summary
- Total users: **100**
- Groups:
  - Control (Old Page): 50  
  - Treatment (New Page): 50  

###  Time Spent
- Average: **5.38 minutes**  
- Converted users: ~**6.5 minutes (median)**  
- Non-converted users: ~**3.5 minutes (median)**  

###  Landing Page Performance
- New page median: **~6 minutes**  
- Old page median: **~4.5 minutes**  

###  Language Distribution
- English: 32 users  
- French: 34 users  
- Spanish: 34 users  

- English had highest raw conversion (~65.6%)  
- Time spent across languages: **~5–6 minutes (similar)**  

---

##  Statistical Hypothesis Testing

### 1. Engagement (Time Spent)
- **Test:** T-test  
- **Result:** p = 0.00028 < 0.05  
-  Users spend significantly more time on the new page  

---

### 2. Conversion Rate
- **Test:** One-tailed Z-test  
- **Result:** p = 0.008 < 0.05  
-  New page has higher conversion rate  

---

### 3. Language Dependency (Conversion)
- **Test:** Chi-Square Test  
- **Result:** p = 0.213 > 0.05  
-  Conversion is NOT dependent on language  

---

### 4. Language vs Time Spent
- **Test:** ANOVA  
- **Result:** p = 0.432 > 0.05  
-  No significant difference across languages  

---

##  Final Conclusions

- The **new landing page is highly effective**  
- It significantly:
  - Increases engagement  
  - Boosts conversions  

- Performance is **consistent across English, Spanish, and French users**, making the solution scalable  

###  Next Steps

To maximize impact:
- Optimize for **mobile performance**  
- Implement **personalized content strategies**  
- Introduce **dynamic user experiences**  

---

##  Tools & Technologies

- **Python**
  - Seaborn (visualization)
  - SciPy / Scikit-learn (statistical testing)
- **Excel**
- **A/B Testing Framework**
- **Statistical Analysis**
