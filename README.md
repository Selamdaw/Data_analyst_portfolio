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

## Background
The motivation for this project was to leverage gym exercise tracking data to create a series of visualizations that depict the factors that impact fitness progress and practices in an educational format. This project was designed to aid gym goers and fitness coaches with education and provide a clear visualization tool for understanding large dataset. Additionally, to enhance my skills and practice using large datasets, utilizing Excel and SQL to visualize and clean data. 

## Project Overview
**Overview:** This analysis aims to support gym management and trainers in designing tailored fitness programs and optimizing training recommendations based on members’ unique profiles, using data-driven insights from 973 samples of gym data to create visualizations offering insights into how demographic factors impact fitness behaviors and progress.

## Key Questions
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
<br>**Cleaning:** To clean and preprocess the data, it involved removing duplicates. After selecting all columns to check if duplicates could exist across any of them, the output message confirmed there were no duplicates found. Next, the data was processed for having any missing values. After applying Conditional Formatting, highlighting Cell Rules and adding a filter on Excel to highlight any blanks, it found that were no missing values found on this dataset. <br> <br>
Furthermore using SQL based queries to clean the data involved identifying nulls, ensuring that each entry is unique by identifying and removing the duplicates, standardizing data formats, correcting misalignments, and converting units where necessary. <br>

Using Conditional Formatting on Excel to highlight extreme values revealed potential outliers in both Calories_Burned and Session_Duration (hours). In the Calories_Burned distribution, there are several points that could represent exceptionally high-calorie burns, possibly from unusually intense or prolonged workouts. Similarly, Session_Duration (hours) shows a few high values that deviate from the main grouping, suggesting some users may have unusually long exercise sessions. These outliers could significantly impact analysis by skewing averages or correlations, so further investigation or handling (e.g., removal or adjustment) may be warranted. <br>


### Data Analysis
Reviewing original dataset, it revealed several preliminary patterns. It showed that higher-intensity workouts, like HIIT and Cardio, are likely associated with increased Max_BPM and Avg_BPM values, as well as greater Calories_Burned per session compared to lower-intensity workouts, such as Yoga. BMI and Fat_Percentage also appear related, though this may vary with muscle mass, particularly among those with higher Experience_Level. <br> <br> Additionally, more experienced members tend to have higher Workout_Frequency (days/week) and possibly longer Session Duration. Age may influence Resting_BPM, with older individuals potentially showing higher resting heart rates. These initial observations point to likely correlations between workout type, frequency, and individual physical characteristics. <br> <br> 

**Key Columns** <br>

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

**Analysis:** Workout Duration is quite consistent around 1.26 hours, with a low spread. Calories Burned shows more variability, suggesting some workouts are significantly more intensive. Heart Rate varies moderately, with most values clustered near the mean of 143 BPM. This overview provides a solid understanding of central tendencies and variability, which can inform decisions on workout design and intensity.

### Data Analysis in SQL 
**Query 1: Demographic Analysis - Average Workout Duration and Calories Burned by Gender** <br>
- Used SQL to group by demographic categories to analyze workout habits. This query helped to observe any patterns in workout duration and calories burned by gender. Looking at Query1_demographics_table.csv, this query calculated the average session_duration and calories_burned for each gender. This helped to identify any differences in workout habits between males and females. Similar to the pivot table but using sql instead. <br>

**Query 2: Exercise Intensity by Experience Level** <br>
- This query helped uncover trends in how more experienced members differ in workout intensity. It grouped data by experience_level (e.g., 1, 2, 3) and calculates the average heart_rate and calories_burned for each level. As shown in 'Query2_experience_level.csv' it helped to see if more experienced members tend to work out with higher intensity (higher heart rate) and burn more calories. <br>

**Query 3: Age and Fitness Trends - Analyze Average Workout and Calories by Age Range** <br>
- Utilized SQL to examine how fitness metrics vary across age ranges. This query created age ranges (18-25, 26-35, etc.) and calculated the average workout_duration and calories_burned for each range. As shown in 'Query4_Age_and_fitness_trends 3(in).csv' it revealed how workout habits and calorie expenditure changed across different age groups.

### Data Visualization
**Visualization:** The project featured a variety of visualization types such as bar charts, line charts, combination charts and more to represent the complex data effectively. These visualisations of the SQL-based queries are found in the 'Visualisations' folder. 

## Findings
**Findings:** Key findings highlight 

the dynamic nature of the solar system, showing variations in planetary rotations, orbits, and environmental conditions that provide a deeper understanding of celestial mechanics.

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
