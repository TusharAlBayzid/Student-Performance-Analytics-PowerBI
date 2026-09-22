🎓 Student Performance Analytics Dashboard
📌 Project Overview
This project is an interactive Data Analytics dashboard developed using Microsoft Power BI to evaluate student academic performance. By processing and modeling raw educational data, this dashboard extracts actionable insights regarding how different demographic factors and preparation strategies impact overall student scores across multiple subjects.

💼 Educational & Business Impact (Actionable Insights)
Demographic Analysis: Evaluates the direct impact of Gender, Ethnicity, and Parental Education on academic success, allowing institutions to identify and support underperforming groups.

Preparation ROI: Analyzes the correlation between completing test preparation courses and final score outcomes, proving the effectiveness of academic interventions.

Top Talent Identification: Dynamically isolates the top-performing students across Math, Reading, and Writing to facilitate advanced placement or scholarship allocations.

Holistic Score Tracking: Provides instant executive-level KPIs for average scores across all subjects and overall percentage.

🛠️ Technical Challenges & Solutions
During the development phase, I tackled several data modeling and visualization challenges:

Complex Metric Aggregation & Error Handling:

Problem: The raw dataset provided separate scores for Math, Reading, and Writing, lacking a unified metric to evaluate overall performance.

Solution: Authored a robust custom Data Analysis Expressions (DAX) measure using the DIVIDE() function: Score Percentage = DIVIDE([Math Score] + [Reading Score] + [Writing Score], 300, 0) * 100. This not only calculated the exact percentage but proactively handled potential zero-division errors, ensuring data integrity.

Visualizing Multi-Dimensional Categorical Ranks:

Problem: Standard bar charts failed to clearly demonstrate how Parental Education ranks dynamically within different Ethnicity groups.

Solution: Implemented an advanced Ribbon Chart. This complex visual effectively maps the flow and rank shifts of parental education categories across different ethnic groups, providing a seamless comparative analysis.

Dynamic Filtering for Top Performers:

Problem: Needed an automated way to continuously highlight only the absolute best students without manual data filtering.

Solution: Utilized Power BI's Top N filtering logic on a Stacked Column Chart, driven by the custom Score Percentage DAX measure, to consistently isolate and display the Top 5 students dynamically.

📂 Repository Contents
Student Performance Analysis Dashboard.pbix : The fully functional Power BI dashboard containing the data model and DAX measures.

Student Performance Analysis Dashboard.pdf : A static PDF export for quick executive review.

Student Performance Analysis Dashboard.png : High-resolution screenshot of the final UI.

student_performance_100.xlsx : The raw dataset utilized for this data modeling project.

👨‍💻 Author
Bayzid Mostak
Data Analyst | Software Engineer

[LinkedIn] https://www.linkedin.com/in/bayzid-mostak-data-analyst/

[GitHub]  https://github.com/TusharAlBayzid
