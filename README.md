# **Analysis of My Step Count and University Assignments**

---

# [**Explanatory Website**](https://utkucaglar.github.io/Data_Analysis_Project/)

---

## **Introduction**

Sabanci University DSA210 Introduction to Data Science Course Fall 2023-2024 Term Project.
This project will include the analysis of my step count and the University assignments' impact on my step count.

---

## **Hypotheses**

- Null Hypothesis (H₀): There is no significant difference in daily activity levels between task days (including the two days prior) and normal days.
- Alternative Hypothesis (Hₐ): There is a significant decrease in daily activity levels on task days (including the two days prior) compared to normal days.

---

## **Motivation** 

My motivation for this project stems from the desire to:
-   Understand Behavioral Patterns: Explore how academic deadlines influence your physical activity habits.
-   Personal Health Insights: Gain insights into your overall physical well-being during periods of high academic stress.
-   Data-Driven Decision Making: Use findings to adjust time management and activity levels to maintain balance during stressful academic periods.

---

### **Tools and Libraries Used**

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

---

## **Data Sources**

I had two main sources of data:

-   Data that i exported from my [Apple Health](https://apps.apple.com/us/app/apple-health/id1242545199) app with a request. [(raw data)](raw_data_from_health_app.xml)
-   Data that i exported from my [Zepp Life (Formerly MiFit)](https://apps.apple.com/tr/app/zepp-life-formerly-mifit/id938688461?l=tr) app which i
wasn't able to use due to the corrupted data or great amount of [missing data](ZeppLife_data.csv). (HAVEN'T USED)
-   Information about the dates of assignments from sucourse (didn't use code).

---

### **Requested data**

Requested data is in .xml format and contains: (I only used step count since that was the most relevant one to my project)
(I didn't use Active Energy Burned and Walking Distance, since those data would give similar visualizations to steps taken)

-   **Daily Step Count:** Information of how many steps i took in a day.
-   **Daily Walking and Running Distance:** Distance traversed in a day.
-   **Daily Active Energy Burned:** How much energy i burned doing activities in a day.
-   **Daily Basal Energy Burned:** The energy burned to carry out fundamental metabolic functions in a day.
-   **Daily Flights Climbed:** The distance walked vertically in a day.  
-   **Daily Headphone Audio Exposure:** The volume of the sound given my headphones in a day.

---

## **Data Analysis**
For detailed and technical information see [main.ipynb](main.ipynb).

1. At first i exported my data and uploaded them into a folder to work on it in [Visual Studio Code](https://code.visualstudio.com).
2. Then i parsed my data and extracted the ones that i could use for my project.
3. After that i created a dataframe to easliy use my data for visualizations and calculations.
4. I tried to understand my dataset using various amount of visalizations.
5. Experimenting, i noticed there is a relationship between the amount of steps i took a day and the date of an important University related assignment.
6. I made more visualization with that information to further investigate.
7. Then i made some hypothesis testing to see if i can reject the null hypothesis.
8. It turned out my hypothesis was true.

---

## **Findings**

These are what i found out from this project:
- I tend to take assignments serious when the deadline approaches. (as most of the students)
- The midterm exam system in our univeristy punishes the students, who doesn't study daily by forcing them to study and take exams on weekends. (again most of the students)
- I observed a partial recovery in my step count immediately after task days, likely due to the completion of academic responsibilities freeing up time for other activities.

---

## **Limitations and Future Work**

#### **Limitations**

1. **Incomplete Data from Zepp Life App**:  
   - Unfortunately, I was unable to use the data exported from my smartband app (Zepp Life) due to extensive missing data and corrupted files.  
   - If I had access to a clean and complete dataset from Zepp Life, I could have compared it with my data from the Apple Health app. This would have allowed me to identify patterns across multiple data sources and validate findings more robustly.  
   - The lack of comparison with another dataset limits the scope of the analysis and the depth of reflective insights I could provide.  

2. **Limited Sample Size**:  
   - Since my project uses personal data from a single individual (myself), the findings cannot be generalized to a larger population. The project reflects my unique habits and behavior but may not apply universally.

---

#### **Future Work**

1. **Incorporating Additional Data Sources**:  
   - Future iterations of this project could include data from multiple apps or devices to ensure a more comprehensive and comparative analysis. For instance, I could attempt to clean and recover the Zepp Life data or use another wearable device for further tracking.

2. **Exploring Other Metrics**:  
   - Incorporating other activity-related metrics such as heart rate variability, and sleep patterns could provide a more holistic view of the impact of assignments on health and well-being.

3. **Expanding the Dataset**:  
   - Collecting and analyzing data over a longer time period or collaborating with peers to include data from multiple individuals could provide more generalizable results and uncover broader trends.

4. **Real-Time Tracking and Intervention**:  
   - I could integrate real-time tracking to monitor activity levels during high-stress periods and design interventions such as reminders to take breaks or engage in light physical activity during study sessions.

5. **Analyzing Productivity and Performance**:  
   - Future work could involve correlating physical activity with academic performance metrics (e.g., grades) to examine how activity levels influence productivity and focus during task-heavy periods.

6. **Integration with External Factors**:  
   - Adding external data, such as weather or daylight hours, could help understand how environmental factors interact with academic schedules to influence physical activity levels.

By addressing these limitations and exploring these future directions, my project could evolve into a more comprehensive and impactful analysis of how academic responsibilities affect health and behavior.


