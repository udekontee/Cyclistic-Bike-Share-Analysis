# Cyclistic-Bike-Share-Analysis
Google Data Analytics capstone analyzing Cyclistic bike-share behavior to compare casual riders and annual members using Python, Pandas, and data visualization.

## Project Overview

This project analyzes Cyclistic bike-share trip data to understand how casual riders and annual members use the service differently.

The analysis follows the six phases of the Google Data Analytics process:

**Ask → Prepare → Process → Analyze → Share → Act**

The primary business objective is to identify behavioral differences between casual riders and annual members and develop data-driven recommendations that could help Cyclistic encourage casual riders to become annual members.

---

## Business Question

**How do annual members and casual riders use Cyclistic bikes differently?**

The analysis focuses on differences in:

- Ride frequency
- Ride duration
- Day-of-week behavior
- Time-of-day behavior
- Seasonal riding patterns
- Bike type usage

---

## Data Source

The project uses 12 months of historical Divvy bike-share trip data covering:

**September 2025 through August 2026**

The monthly datasets were combined into a single dataset containing more than **6.1 million rides**.

The data includes information such as:

- Ride ID
- Bike type
- Start and end timestamps
- Station information
- Geographic coordinates
- Rider type (casual or member)

The data is provided by Divvy and made publicly available for analysis.

---

## Tools Used

- **Google Colab** — analysis environment
- **Python** — data analysis
- **Pandas** — data cleaning, transformation, and aggregation
- **Matplotlib** — data visualization
- **Google Drive** — dataset storage
- **GitHub** — project documentation and portfolio presentation

---

## Data Preparation and Cleaning

The 12 monthly CSV files were combined into one dataset containing approximately **6.12 million trip records**.

Key cleaning steps included:

- Verified that all monthly files used the same schema
- Removed duplicate ride IDs
- Converted start and end timestamps to datetime values
- Calculated ride duration in minutes
- Removed rides with zero or negative durations
- Investigated unusually long rides
- Excluded rides longer than 24 hours because their durations showed an unusual concentration around approximately 25 hours
- Restricted the analysis to rides beginning between September 1, 2025 and August 31, 2026
- Created additional variables for day of week, month, date, and hour

The final cleaned dataset contained:

**6,110,391 rides**

Missing station information was not automatically removed because those rides remained useful for analyses that did not require station-level information.

---

## Key Findings

### 1. Annual Members Take More Rides

Annual members account for **64.72%** of all rides, while casual riders account for **35.28%**.

This indicates that annual members use the bike-share service more frequently overall.

### 2. Casual Riders Take Longer Trips

Average ride duration:

- **Casual riders:** 17.78 minutes
- **Annual members:** 11.97 minutes

Casual riders therefore take substantially longer rides on average.

### 3. Casual Riding Is More Concentrated on Weekends

Member ridership is strongest during the workweek, with the highest number of member rides occurring on Wednesday.

Casual ridership increases toward the weekend and reaches its highest level on Saturday.

### 4. Members Show Strong Morning and Evening Peaks

Annual members show pronounced riding peaks around **8 AM** and **5 PM**.

Casual ridership increases more gradually throughout the day and does not display the same strong morning peak.

Combined with the weekday riding pattern, this is consistent with members using the service more frequently for routine transportation. However, trip purpose cannot be directly determined from the dataset.

### 5. Casual Ridership Is More Seasonal

Both groups ride less during winter and more during warmer months.

Casual ridership shows particularly strong seasonal variation, falling substantially during winter before increasing through spring and summer.

### 6. Weekend Casual Trips Are Longer

Casual riders have longer average ride durations than members on every day of the week.

On weekends:

- **Saturday:** Casual 23.18 minutes vs. Member 13.60 minutes
- **Sunday:** Casual 24.28 minutes vs. Member 13.49 minutes

This suggests that casual riders may be more likely to take longer leisure or recreational trips, although trip purpose is not directly available in the data.

### 7. Electric Bikes Are Popular With Both Groups

Electric bikes account for:

- **73.60% of casual rides**
- **68.06% of member rides**

Electric bikes dominate usage for both rider groups, with casual riders showing a modestly higher share of electric-bike usage.

---

## Business Recommendations

Based on the analysis, Cyclistic could consider three strategies:

1. **Target casual riders during weekends and high-ridership months.**  
   Casual activity is particularly strong on weekends and during warmer months, making these periods useful opportunities for membership campaigns.

2. **Develop campaigns around longer weekend riding patterns.**  
   Casual riders take substantially longer weekend trips. Cyclistic could test membership messaging aimed at riders who repeatedly use the service for longer weekend trips.

3. **Test membership campaigns with frequent casual electric-bike users.**  
   Electric bikes represent 73.60% of casual rides. Cyclistic could evaluate whether repeat casual electric-bike users respond differently to targeted membership campaigns.

---

## Limitations

This analysis identifies behavioral patterns but does not establish why riders choose casual or annual membership.

The dataset does not include demographic information, trip purpose, individual marketing exposure, membership pricing decisions, or reasons for choosing a particular ride.

Therefore, findings such as possible commuting or recreational behavior should be interpreted as behavioral patterns rather than confirmed trip purposes.

Future analysis could use controlled experiments, such as **A/B testing**, to evaluate whether targeted marketing strategies actually increase membership conversion.

---

## Conclusion

The analysis shows clear differences between casual riders and annual members.

Annual members ride more frequently and demonstrate stronger weekday and morning/evening usage patterns. Casual riders take longer trips, ride more heavily on weekends, and show greater seasonal variation.

These findings suggest that Cyclistic could focus membership-conversion efforts on casual riders during weekends and high-ridership months while testing targeted campaigns based on observed riding behavior.

---

## Project Notebook

The complete Python analysis, including data preparation, cleaning, exploratory analysis, visualizations, and business recommendations, is available in:

**`Cyclistic_Bike_Share_Analysis.ipynb`**

---

## Author

**U Dekontee Kun**

Data Analytics | Business Intelligence | Data Science

[GitHub Profile](https://github.com/udekontee)
