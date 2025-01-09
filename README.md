# My Step Count and University Assignments

## Introduction

Sabanci University DSA210 Introduction to Data Science Course Fall 2023-2024 Term Project.
This project will include the analysis of my step count and the University assignments' impact on my step count.


## Motivation 

My motivation for this project stems from the desire to:
-   Understand Behavioral Patterns: Explore how academic deadlines influence your physical activity habits.
-   Personal Health Insights: Gain insights into your overall physical well-being during periods of high academic stress.
-   Data-Driven Decision Making: Use findings to adjust time management and activity levels to maintain balance during stressful academic periods.


### Tools and Libraries Used

**[Visual Studio Code](https://code.visualstudio.com/):**  Used as the primary Integrated Development Environment (IDE) for writing and managing the project code.

**[Pandas](https://pandas.pydata.org/):**  Used for data manipulation, cleaning, filtering, and structuring. Pandas provided an efficient way to process and analyze the large dataset of step counts and task days.

**[Matplotlib](https://matplotlib.org/):**  Employed for creating static, publication-quality visualizations, such as bar charts, line graphs, and cumulative step plots.

**[Seaborn](https://seaborn.pydata.org/):**  Used to create more visually appealing and complex visualizations like box plots, KDE plots, and heatmaps for data analysis.

**[Numpy](https://numpy.org/):**  Utilized for numerical operations, particularly for generating arrays, calculating means, and performing mathematical computations.

**[XML ElementTree (ET)](https://docs.python.org/3/library/xml.etree.elementtree.html):**  Used to parse the raw XML file exported from the fitness tracking application. It enabled the extraction of structured data for further analysis.

**[Scipy](https://www.scipy.org/):**  Included for statistical hypothesis testing, such as:
- **T-Test**: To compare mean step counts between task and normal days.
- **Mann-Whitney U Test**: For comparing step distributions between task and normal days.
- **Kruskal-Wallis Test**: To identify significant differences between step counts across multiple groups.

## Data Sources

I had two main sources of data:

-   Data that i exported from my [Apple Health](https://apps.apple.com/us/app/apple-health/id1242545199) app with a request.
-   Data that i exported from my [Zepp Life (Formerly MiFit)](https://apps.apple.com/tr/app/zepp-life-formerly-mifit/id938688461?l=tr) app which i
wasn't able to use due to the corrupted data or great amount of [missing data](ZeppLife_data.csv).
-   Information about the dates of assignments from sucourse (didn't use code).

### Requested data

Requested data is in .xml format and contains: (I only used step count since that was the most relevant one to my project)
(I didn't use Active Energy Burned and Walking Distance, since those data would give similar visualizations to steps taken)

-   **Daily Step Count:** Information of how many steps i took in a day.
-   **Daily Walking and Running Distance:** Distance traversed in a day.
-   **Daily Active Energy Burned:** How much energy i burned doing activities in a day.
-   **Daily Basal Energy Burned:** The energy burned to carry out fundamental metabolic functions in a day.
-   **Daily Flights Climbed:** The distance walked vertically in a day.  
-   **Daily Headphone Audio Exposure:** The volume of the sound given my headphones in a day.

ssssssssssssssssssssss
## Research Questions
1. **Activity Patterns**:
   - How do physical activity levels vary during periods of high academic stress, such as exams or homework-heavy weeks?
   - Are there observable differences in activity between weekdays and weekends?

2. **External Influences**:
   - What role do factors such as weather or travel days play in shaping physical activity trends?

3. **Device Comparison**:
   - How consistent are the measurements between my smartwatch and phone app for steps, kilometers, and flights climbed, calories burned?
   - Do discrepancies exist between the datasets, and what might explain them?

4. **Long-Term Trends**:
   - What general trends emerge from daily, weekly, and monthly activity data?

## Dataset Description
- **Smartwatch Data**: Includes daily records of steps taken, kilometers traveled, flights climbed, and calorie burn.
- **Phone App Data**: Similar activity metrics captured using GPS and motion sensors.
- Additional data, such as weather conditions or personal stress logs, may be incorporated to add context.

## Project Aims
1. **Identify Patterns**: Explore how physical activity changes during academic stress periods and other external influences.
2. **Validate Data Sources**: Compare data from the smartwatch and phone app to assess accuracy and reliability.
3. **Visualize Findings**: Create visualizations that clearly illustrate activity trends, relationships, and discrepancies between datasets.
4. **Draw Insights and Recommendations**: Use findings to evaluate the effectiveness of wearable devices and their tracking methods.

## Example Claims
1. **Activity Impact of Exams**: Physical activity decreases significantly during exam weeks compared to normal routines, reflecting the influence of academic stress.
2. **Device Discrepancies**: Initial comparisons suggest inconsistencies between smartwatch and phone app data, particularly in step counts.

## Project Plan
1. **Data Collection and Cleaning**: Gather and prepare data from both sources for analysis.
2. **Exploratory Analysis**: Investigate trends, patterns, and relationships in the data.
3. **Comparison Analysis**: Evaluate discrepancies between smartwatch and phone app metrics.
4. **Visualization**: Develop graphs and charts to support claims and highlight findings.
5. **Report**: Compile insights, conclusions, and recommendations into a cohesive report.
