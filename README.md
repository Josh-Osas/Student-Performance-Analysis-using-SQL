# SQL Student Performance Data Analysis by Joshua Osarumwense

This project showcases my proficiency in SQL by analysing the factors influencing student performance using data from an **EDUCATION** database. The analysis explores various attributes, such as **study hours**, **attendance**, **parental involvement**, and **access to resources**, and their impact on **exam scores**. Through advanced SQL techniques, I integrated data from multiple tables to extract meaningful insights and patterns.

## 🧑🏽‍💻 Technologies Used

- **SQL**: Used for data exploration, consolidation, and querying.
- **EDUCATION Database**: Includes tables like **FACTORS**, **PARENTS**, and **STUDENTS**.
- **CASE Statements**: Used to categorise data based on conditions (e.g., study hours, attendance levels).
- **Aggregation Functions**: Utilized functions like **AVG()**, **COUNT()**, and **ROUND()** for summary statistics.
- **FULL JOIN**: Combined multiple tables to form a comprehensive dataset for analysis.

## 🔍 Data Exploration

The project began with exploring data from the following tables:

- **FACTORS Table**: Contains attributes like hours studied, attendance, access to resources, etc., which influence academic performance.
- **PARENTS Table**: Includes socioeconomic factors such as parental involvement, income, and education level.
- **STUDENTS Table**: Holds demographic details, previous scores, and current exam performance.

### Key Attributes:
- **Exam scores**
- **Attendance**
- **Parental involvement**
- **Access to resources**
- **Extracurricular activities**

## 🔗 Data Consolidation

To gain a holistic view, I created a unified table, **EXAM**, by performing a **FULL JOIN** on **STUDENTS**, **FACTORS**, and **PARENTS**, aligned by **Student_ID**. This integrated dataset allows for deeper analysis of trends, correlations, and the impact of various factors on student performance.

## 📊 Key Queries and Insights

### 1. Average Exam Score by Hours Studied
- **Method**: Grouped students by study hour ranges (e.g., "30+ HOURS") using a **CASE** statement and calculated the average scores using **AVG()**.
- **Insights**: Students studying 30+ hours achieved the highest average score (71), highlighting a strong correlation between study time and academic success.

### 2. Average Exam Score by Attendance Levels
- **Method**: Categorized attendance into ranges (e.g., "80+ HOURS") using a **CASE** statement and calculated the average score.
- **Insights**: Highest attendance (80+ hours) correlated with the highest score (69.2), while lower attendance (41-60 hours) showed reduced scores (62.4), emphasizing the importance of consistent attendance.

### 3. Impact of Parental Involvement on Exam Scores
- **Method**: Grouped students into **High**, **Medium**, and **Low** parental involvement and calculated average scores.
- **Insights**: High parental involvement led to the highest scores (68.1), emphasizing the role of parental support in academic success.

### 4. Top 10 Students with the Most Improvement
- **Method**: Calculated percentage improvement using the formula:  
  `((EXAM_SCORE - PREVIOUS_SCORES) / PREVIOUS_SCORES) * 100`, filtered for non-zero previous scores, and sorted by improvement.
- **Insights**: Student 11110 improved the most (76.9%), identifying significant progress and potential areas for intervention.

### 5. Top 10 Students with the Largest Drop in Scores
- **Method**: Calculated percentage drops in scores and ranked students by largest negative changes.
- **Insights**: Student 5897 experienced the largest drop (-39%), highlighting potential areas for support and intervention.

### 6. Gender Distribution of Students Scoring Above Average
- **Method**: Filtered students exceeding the average score (67.2) and grouped them by gender using **COUNT()**.
- **Insights**: 1735 males scored above average compared to 1273 females, indicating potential gaps in preparation or external factors affecting performance.

### 7. Average Exam Score for Students with and Without Access to Resources
- **Method**: Grouped students by **ACCESS_TO_RESOURCES** levels and calculated average scores using **AVG()**.
- **Insights**: Students with high access to resources scored the highest (68.1), reinforcing the positive impact of resources on performance.

## 💡 Conclusion

This SQL project demonstrates my ability to effectively explore, consolidate, and analyse data using advanced SQL techniques. By integrating academic, demographic, and socioeconomic data, I was able to uncover key insights such as the importance of study hours, attendance, parental involvement, and access to resources on student performance. The project highlights my ability to extract actionable insights that can inform decision-making and drive educational improvements.

## 📈 Technical Highlights

- **Advanced SQL Joins**: Used **FULL JOIN** to integrate data from multiple tables.
- **CASE Statements**: Applied to categorize data based on conditions like study hours and attendance.
- **Aggregation Functions**: Leveraged functions like **AVG()**, **COUNT()**, and **ROUND()** for comprehensive data analysis.
- **Actionable Insights**: The analysis identifies trends in student performance, improvement, and the impact of various factors.


