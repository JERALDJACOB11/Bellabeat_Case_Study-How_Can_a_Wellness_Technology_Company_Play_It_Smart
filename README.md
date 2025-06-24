# Bellabeat Case Study: Smart Wellness Technology Data Analysis
---
## Bellabeat Case Study: 
- <a href="https://github.com/JERALDJACOB11/Bellabeat_Case_Study-How_Can_a_Wellness_Technology_Company_Play_It_Smart/blob/main/Bellabeat%20Case%20Study.pdf">Presentation</a>
## Scope of Work: 
- <a href="https://github.com/JERALDJACOB11/Bellabeat_Case_Study-How_Can_a_Wellness_Technology_Company_Play_It_Smart/blob/main/S-O-W-Bellabeat%20Case%20Study%20(1).pdf">S-O-W Link</a>
## Business Questions
- **"What are trends in smart device usage?"**
- **"How could these trends apply to Bellabeat customers?"**
- **"How could these trends influence marketing?"**

### Key Research Questions
- Do people walk or sleep more on weekdays or weekends?
- How can Bellabeat app remind women to wind down earlier and walk more steps by monitoring user activity?
- How can Bellabeat run social media ads addressing sleep and walk cycles with messaging like "Your holistic women wellness app"?

## 📝 Business Task Statement
> "Analyze FitBit data to find trends in user activity, sleep, and heart rate. Then, use these trends to suggest marketing strategies for the Bellabeat app, helping women improve their wellness."

---

## Data Quality Assessment (ROCCC Framework)

| Criteria | Assessment | Details |
|----------|------------|---------|
| **Reliable** | ✅ | Contains personal fitness tracker information from thirty Fitbit users |
| **Original** | ✅ | Data made available by Mobius (Owner) via Kaggle |
| **Comprehensive** | ✅ | Includes daily physical activity, steps, heart rate, sleep monitoring |
| **Current** | ⚠️ | Data generated between 12/13/16 to 12/15/16 (outdated) |
| **Cited** | ✅ | CC0 Public Domain dataset via Kaggle |

## 📊 Data Source Description

- **Dataset**: FitBit Fitness Tracker Data from Kaggle (CC0 Public Domain)
- **Scope**: Daily activity, steps, heart rate, and sleep data from 30 users
- **Dataset used**: <a href="https://www.kaggle.com/datasets/arashnic/fitbit">Direct Link</a>
  
### ⚠️ Limitations
- Small sample size (only 30 people)
- Outdated data (from 2016)
- Trends may differ for larger/current populations

---

## Data Cleaning Documentation

| File | Problem | Action Taken |
|------|---------|--------------|
| dailyActivity | Dates not formatted | Formatted as Date and formatted remaining columns to respective format |
| dailyActivity | Duplicates | Removed duplicate rows [No duplicate rows found, 940 unique rows] |
| sleepDay | Extra time in dates | Removed time, kept date |
| sleepDay | Unclear column names | Renamed to "Total Sleep Minutes" etc. |
| sleepDay | Unrealistic sleep values | Removed rows with sleep < 180min or > 900min |

## 📋 Process Summary
Data cleaning involved removing duplicates, formatting, filtering, validating data, renaming columns and merging datasets. For activity and sleep data, dates were extracted from timestamps. All steps were documented in a comprehensive cleaning log.

---

## Key Analytics Findings

### 🚶‍♀️ Activity Analysis (Steps)

| Metric | Value |
|--------|-------|
| **Average daily steps (total)** | 17,221 |
| **Weekday average** | 8,498 |
| **Weekend average** | 8,723 |
| **Difference** | 225 more steps on weekends |
| **Percentage difference** | 2.64% |

**Key Insight**: People walk 225 more steps on weekends compared to weekdays.

### 😴 Sleep Analysis

| Metric | Value |
|--------|-------|
| **Average daily sleep (total minutes)** | 894 |
| **Weekday average** | 425 minutes (7.1 hours) |
| **Weekend average** | 469 minutes (7.8 hours) |
| **Difference** | 43 minutes more on weekends |
| **Percentage difference** | 10.17% |

**Key Insight**: People sleep 43 minutes longer on weekends.

## 🔬 Advanced Analysis

### 1. Sleep Efficiency Analysis
**Question**: Do people spend more time actually sleeping vs. lying in bed on weekends?

| Day Type | Sleep Efficiency |
|----------|------------------|
| Weekday | 91.96% |
| Weekend | 90.84% |

**Finding**: Weekday sleep is slightly more efficient (92%) vs weekends (91%).

### 2. Sleep vs. Activity Correlation
**Question**: Do people who walk more sleep better?

| Step Group | Average Sleep Minutes |
|------------|----------------------|
| < 10,000 Steps | 409 |
| ≥ 10,000 Steps | 456 |

**Finding**: Users who walk 10,000+ steps sleep **47 minutes longer** on average.

### 3. User Behavioral Patterns
**Question**: Do all users sleep more on weekends?

| Pattern | Number of Users |
|---------|-----------------|
| Sleeps more on weekends |  90% |
| Sleeps more on weekdays ("Night owls") |  10% |

**Finding**: 90% of users follow typical weekend sleep patterns, but 10% are "night owls" with different behaviors.

---

## Data Visualizations & Insights
### Visualization 
- <a href="https://github.com/JERALDJACOB11/Bellabeat_Case_Study-How_Can_a_Wellness_Technology_Company_Play_It_Smart/blob/main/Bellabeat%20Case%20Study.pdf">Presentation</a>
### 🚶‍♀️ Steps: Weekday vs. Weekend
| Day Type | Average Steps |
|----------|---------------|
| Weekday | 8,498 |
| Weekend | 8,723 |

**Insight**: Users walk 225 more steps on weekends. Bellabeat can encourage weekday movement with motivational alerts like *"Let's catch up to your weekend stride!"*

### 😴 Sleep: Weekday vs. Weekend
| Day Type | Avg Sleep (Minutes) |
|----------|---------------------|
| Weekday | 425 |
| Weekend | 469 |

**Insight**: Users sleep 43 minutes longer on weekends. Bellabeat could prompt users with friendly *"Time to wind down"* bedtime reminders on weeknights.

#### 🎯 Activity Impact on Sleep
| Step Group | Avg Sleep Minutes |
|------------|-------------------|
| < 10,000 Steps | 409 |
| ≥ 10,000 Steps | 456 |

**Insight**: Users who walk 10,000+ steps sleep 47 minutes more. Bellabeat can link daily steps to sleep quality, showing how **movement = better rest**.

### 💡 Strategic Recommendations for Bellabeat

#### Product Integration Opportunities
Bellabeat could enhance user engagement through:

1. **Smart Notifications**: Calculate steps and show step counts to encourage more walking
2. **Sleep Cycle Monitoring**: Use Bellabeat's Leaf (wellness tracker worn as bracelet, necklace, or clip) or Time (wellness watch) to track sleep patterns
3. **App Integration**: Both devices connect to Bellabeat app to track activity, sleep, and daily wellness

#### Marketing Strategy Recommendations

1. **Weekday Movement Campaign**: Target reduced weekday activity with motivational messaging
2. **Sleep Optimization Program**: Address weekend vs. weekday sleep pattern differences
3. **Personalized Coaching**: Develop custom guidance for different user segments (including "night owls")
4. **Activity-Sleep Connection**: Highlight the correlation between daily steps and sleep quality
5. **Efficiency-Based Features**: Detect low sleep efficiency and suggest breathing or meditation

### Final Tranfomed Data
- **Activity Data**: <a href="https://github.com/JERALDJACOB11/Bellabeat_Case_Study-How_Can_a_Wellness_Technology_Company_Play_It_Smart/blob/main/Bellabeat_Case_Study_Data%20-%20dailyActivity_merged.csv">Activity Data Link</a>
- **Sleep Data**: <a href="https://github.com/JERALDJACOB11/Bellabeat_Case_Study-How_Can_a_Wellness_Technology_Company_Play_It_Smart/blob/main/Bellabeat_Case_Study_Data%20-%20sleepDay_merged.csv">Sleep Data Link</a>
- **Visual Insight Data**: <a href="https://github.com/JERALDJACOB11/Bellabeat_Case_Study-How_Can_a_Wellness_Technology_Company_Play_It_Smart/blob/main/Bellabeat_Case_Study_Data%20-%20visual_insight.csv">Visual Insight</a>
- **Visualization Data**: <a href="https://github.com/JERALDJACOB11/Bellabeat_Case_Study-How_Can_a_Wellness_Technology_Company_Play_It_Smart/blob/main/Bellabeat_Case_Study_Data%20-%20visualization.csv">Visualization</a>
---

# 🏆 Project Impact

This analysis demonstrates how data-driven insights can directly inform product development and marketing strategy for wellness technology companies, specifically targeting women's health and wellness optimization.

**Disclaimer**: Findings based on 30 users from 2016 data. Trends may differ for larger/current populations.
