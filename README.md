# Gym Members Exercise Dataset Analysis

## Description
**Description:** This project analyzes gym members' exercise patterns, physical attributes, and fitness metrics through SQL-based queries and Excel visualizations to uncover demographic trends, workout intensity, and fitness progression. Using interactive charts, providing a comprehensive view of member behaviors, health trends, and correlations between metrics like heart rate, workout duration, and calories burned.

## Table of Contents
- [Overview](#project-overview)
- [Key Question](#questions)
- [Data Sources](#data-sources)
- [Technologies Used](#technologies-used)
- [Methodology](#methodology)
  - [Data Collection](#data-collection)
  - [Data Cleaning](#data-cleaning)
  - [Data Analysis](#data-analysis)
  - [Data Visualization](#data-visualization)
- [Findings](#findings)
- [Conclusion](#conclusion)
- [Attribution](#attribution)
- [Contact](#contact)

## Project Overview
**Overview:** This analysis aims to support gym management and trainers in designing tailored fitness programs and optimizing training recommendations based on members’ unique profiles, using data-driven insights from 973 samples of gym data to create visualizations offering insights into how demographic factors impact fitness behaviors and progress.

## Questions
**Research Questions:**  
- How do demographic factors (age, gender) relate to workout intensity and duration? 
- What are typical heart rate patterns, and how do they correlate with calories burned? 
- Can we identify trends in fitness progress over time based on experience levels?

## Data Sources
**Sources:** Data was sourced from Kaggle sample dataset saved as 'gym_members_exercise_tracking.csv' in the dataset folder.

## Technologies Used
**Technologies:** This project was developed using Excel for the creation of visualizations, Jupyter Notebooks for initial data processing, and SQL for data cleaning, managing and manipulating data.

## Methodology
### Data Collection
**Collection:** Data from the gym members exercise sessions were collected from a kaggle dataset by Kala Khorasami for data scientists, health researchers, and fitness enthusiasts interested in studying exercise habits or analyzing the relationship between demographic and physiological data to use. 

### Data Cleaning
The 'gym_members_exercise_tracking.csv' data underwent a rigorous cleaning processes, including unit conversions, alignment corrections, and formatting to ensure compatibility with visualization tools. <br>
<br>**Cleaning:** To clean and preprocess the data, it involved removing duplicates. After selecting all columns to check if duplicates could exist across any of them, the output message confirmed there were no duplicates found. Next, the data was processed for having any missing values. After applying Conditional Formatting, highlighting Cell Rules and adding a filter on Excel to highlight any blanks, it found that were no missing values found on this dataset. <br> <br> Using Conditional Formatting to highlight extreme values it revealed potential outliers in both Calories_Burned and Session_Duration (hours). In the Calories_Burned distribution, there are several points that could represent exceptionally high-calorie burns, possibly from unusually intense or prolonged workouts. Similarly, Session_Duration (hours) shows a few high values that deviate from the main grouping, suggesting some users may have unusually long exercise sessions. These outliers could significantly impact analysis by skewing averages or correlations, so further investigation or handling (e.g., removal or adjustment) may be warranted. <br>
In addition, using SQL to clean and preprocess the Gym Members Exercise Data to ensure this further it involved identifying nulls, ensuring each entry is unique by identifying and removing the duplicates.

### Data Analysis
**Analysis:** Reviewing original dataset, it revealed several preliminary patterns. It showed that higher-intensity workouts, like HIIT and Cardio, are likely associated with increased Max_BPM and Avg_BPM values, as well as greater Calories_Burned per session compared to lower-intensity workouts, such as Yoga. BMI and Fat_Percentage also appear related, though this may vary with muscle mass, particularly among those with higher Experience_Level. <br> <br> Additionally, more experienced members tend to have higher Workout_Frequency (days/week) and possibly longer Session Duration. Age may influence Resting_BPM, with older individuals potentially showing higher resting heart rates. These initial observations point to likely correlations between workout type, frequency, and individual physical characteristics. <br> <br> 

**Statistics of Key Columns** <br>

Session Duration (hours):<br> 
- Mean: 1.26 hours
- Median: 1.26
- Max: 2.0 hours
- Standard deviation: 0.36 <br>

Calories Burned: <br>
- Mean: 905.42 calories
- Median: 893.0 calories
- Max: 1783 calories
- Standard Deviation: 272.64 calories <br>

Average Heart Rate (BPM): <br>
- Mean: 143.77 BPM
- Median: 143.0 BPM
- Max: 169 BPM
- Standard Deviation: 14.35 BPM <br>

**Analysis:** Workout Duration is quite consistent around 1.26 hours, with a low spread. Calories Burned shows more variability, suggesting some workouts are significantly more intensive.
Heart Rate varies moderately, with most values clustered near the mean of 143 BPM.
This overview provides a solid understanding of central tendencies and variability, which can inform decisions on workout design and intensity.


 

Analytical methods included time series analysis, comparative analysis, and categorical comparison, focusing on visual clarity and data integrity.

### Data Visualization
**Visualization:** The project features a variety of visualization types such as 2D maps, bar charts, heat maps, and more to represent the complex data effectively.

## Findings
**Findings:** Key findings highlight the dynamic nature of the solar system, showing variations in planetary rotations, orbits, and environmental conditions that provide a deeper understanding of celestial mechanics.

## Conclusion
**Conclusion:** The Solar System Model project successfully leverages advanced data visualization techniques to illustrate the intricate relationships and physical characteristics of celestial bodies, promoting greater public engagement and educational opportunities in astronomy.

## Attribution
**Attribution:** Credits to NASA's National Space Science Data Center, Astropy library, and all data providers who made this project possible.

## Contact

<details>
<summary>Click to expand!</summary>

For any questions, comments, or collaborations, feel free to reach out.

- **Contact**: [Contact Richard](https://eclipseanalytics.bss.design/)
- **Website**: [Visit Richard's Website](https://eclipseanalytics.bss.design/)
- **GitHub**: [Visit Richard's GitHub Portfolio](https://github.com/EclipseAnalytics/Data-Analyst-Portfolio)

</details>
