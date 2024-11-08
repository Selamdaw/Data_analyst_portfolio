
# Exercise Tracking Project

## Description
This project analyzes gym members' exercise patterns, physical attributes, and fitness metrics through SQL-based queries and Excel visualizations to uncover demographic trends, workout intensity, and fitness progression. Using charts, providing a comprehensive view of member behaviors, health trends, and correlations between metrics like heart rate, session duration, and calories burned.

## Table of Contents
- [Background](#background)
- [Project Overview](#project-overview)
- [Key Question](#questions)
- [Data Sources](#data-sources)
- [Technologies Used](#technologies-used)
- [Methodology](#methodology)
  - [Data Collection](#data-collection)
  - [Data Cleaning](#data-cleaning)
  - [Data Analysis](#data-analysis)
  - [Data Analysis in SQL](#data-analysis-sql)
  - [Data Visualization](#data-visualization)
- [Findings](#findings)
- [Conclusion](#conclusion)
- [Attribution](#attribution)
- [Contact](#contact)

## Background
The motivation for this project was to leverage gym exercise tracking data to create a series of visualizations that depict the factors that impact fitness progress and practices in an educational format. This project was designed to aid gym goers and fitness coaches with education and provide a clear visualization tool for a large dataset. Additionally, to enhance my skills and practice using large datasets, utilizing Excel and SQL to visualize and clean data. 

## Project Overview
**Overview:** This analysis aims to support gym management and trainers in designing tailored fitness programs and optimizing training recommendations based on members’ unique profiles, using data-driven insights from 973 samples to create visualizations that offer insights into how demographic factors impact fitness behaviors and progress.

## Key Questions
**Research Questions:**  
- How do demographic factors (age, gender) relate to workout intensity and duration? 
- What are typical heart rate patterns, and how do they correlate with calories burned? 
- Can we identify trends in fitness progress over time based on experience levels?

## Data Sources
**Sources:** Data was sourced from Kaggle sample dataset saved as 'gym_members_exercise_tracking.csv' containing 973 samples of gym data in the dataset folder.

## Technologies Used
**Technologies:** This project was developed using Excel for the creation of visualizations, Excel for initial data processing, and SQL for data cleaning, managing and manipulating data.

## Methodology
### Data Collection
**Collection:** Data from the gym members exercise sessions were collected from a Kaggle dataset by Kala Khorasami for data scientists, health researchers, and fitness enthusiasts interested in studying exercise habits or analyzing the relationship between demographic and physiological data. 

### Data Cleaning
The 'gym_members_exercise_tracking.csv' data underwent a rigorous cleaning processes, including unit conversions, alignment corrections, and formatting to ensure compatibility with visualisation tools. <br>
<br>**Cleaning:** To clean and preprocess the data, it involved removing duplicates. After selecting all columns to check if duplicates could exist across any of them, the output message confirmed there were no duplicates found. Next, the data was processed for having any missing values. After applying Conditional Formatting, highlighting Cell Rules and adding a filter on Excel to highlight any blanks, it found that were no missing values found on this dataset. <br> <br>
Furthermore using SQL based queries to clean the data involved identifying nulls, ensuring that each entry is unique by identifying and removing the duplicates, standardizing data formats, correcting misalignments, and converting units where necessary. <br>

Using Conditional formatting on Excel to highlight extreme values revealed potential outliers in both Calories_Burned and Session_Duration (hours). In the Calories_Burned distribution, there are several points that could represent exceptionally high-calorie burns, possibly from unusually intense or prolonged workouts. Similarly, Session_Duration (hours) shows a few high values that deviate from the main grouping, that suggests some users may have unusually long exercise sessions. These outliers could significantly impact analysis by skewing averages or correlation (e.g., removal or adjustment). <br>

### Data Analysis
When analysing the original dataset, it revealed several preliminary patterns. It showed that higher-intensity workouts, like HIIT and Cardio, are likely associated with increased Max_BPM and Avg_BPM values, as well as greater Calories_Burned per session compared to lower-intensity workouts, such as Yoga. BMI and Fat_Percentage also appear related, though this may vary with muscle mass, particularly among those with higher Experience_Level. <br> <br> Additionally, more experienced members tend to have higher Workout_Frequency (days/week) and possibly longer Session Duration. Age may influence Resting_BPM, with older individuals potentially showing higher resting heart rates. These initial observations point to likely correlations between workout type, frequency, and individual physical characteristics. <br> <br> 

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

**Analysis:** Session Duration is quite consistent around 1.26 hours, with minimal variation. Calories Burned shows more variability, suggesting some workouts are significantly more intensive. Heart Rate varies moderately, with most values clustered near the mean of 143 BPM. This overview provides a solid understanding of central tendencies and variability, which can inform decisions on workout design and intensity.

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
**Findings:** The key data findings offer insights into fitness trends across gender, experience level, and age segments

The gender data shows that males and females have comparable session durations, but males burn slightly more calories on average per session​(Query1_demographics_visualisation). The experience level data reveals that as fitness experience increases, both the average heart rate and calories burned rise, indicating that experienced individuals push themselves harder, achieving greater calorie burn ​(Query2_experience_level). 

The increase in both average heart rate and calorie burn implies that more experienced individuals engage in higher-intensity workouts, which may indicate greater fitness motivation or tolerance​(Query2_experience_level). Meanwhile, gender differences in calorie burned might relate to physiological factors like muscle mass, which affects calorie burn rate, even if session duration is similar between genders.

The age trends indicate that workout duration remains consistent across age groups, while calories burned peaks in the 26-35 range and slightly decreases with age, indicating peak calories burned in early adulthood, which gradually declines with age (Query4_age_and_fitness_trends.pdf).

## Conclusion
**Conclusion:** The Gym Members Exercise project successfully leverages advanced data visualization techniques to illustrate the relationship between age, gender, and experience level in fitness performance. Findings indicate peak calorie expenditure in early adulthood, which gradually declines with age, while more experienced members achieve higher calorie burns through increased workout intensity. These insights reveal patterns that can inform tailored fitness strategies for different demographics, enhancing member engagement and health outcomes.

## Attribution
**Attribution:** Credits to Kala Khorasami for the Kaggle sample dataset.

## Contact

<details>
<summary>Click to expand!</summary>

For any questions, comments, or collaborations, feel free to reach out.

- **Contact**: [Contact Selam ](selamdawit02@gmail.com)
- **GitHub**: [Visit Selam's GitHub Portfolio](https://github.com/Selamdaw/Data_analyst_portfolio)

</details>
