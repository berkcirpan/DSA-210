Social Media Usage and Step Count Analysis

Project Objective

The aim of this project is to analyze the relationship between my daily social media usage (Twitter, TikTok, and Instagram) and my physical activity, measured in daily step counts. Data from 2024-12-16 to 2025-01-09 was collected and processed to explore patterns and correlations between these two variables.

Data Collection and Preprocessing

1. Data Sources
	•	Apple Health Step Data: Exported as an XML file containing step count records.
	•	Social Media Usage Data: Manually recorded daily usage time (in minutes) for Twitter, TikTok, and Instagram combined.

2. Preprocessing Steps
	•	Apple Health Data:
	•	Parsed the XML file using Python’s xml.etree.ElementTree library.
	•	Extracted relevant information: startDate, endDate, and value (step count).
	•	Filtered data to only include records from the target date range.
	•	Grouped step counts by day to calculate daily totals.
	•	Social Media Data:
	•	Loaded the Excel file using pandas.
	•	Cleaned and filtered the data to match the date range of the step data.

3. Merging Data

Both datasets were merged on the Date column to create a unified dataset containing:
	•	Date: The day of the record.
	•	TotalSteps: Total step count for the day.
	•	Minute: Total social media usage (in minutes) for the day.


 Exploratory Data Analysis

1. Time Series Trends
	•	Objective: To observe daily fluctuations in both step counts and social media usage.
	•	Visualization: A line plot was used to compare trends over time.
	•	Observation: Social media usage remained consistent, while step counts fluctuated significantly.

2. Correlation Analysis
	•	Objective: To quantify the relationship between step counts and social media usage.
	•	Visualization: A heatmap was generated to show correlations between variables.
	•	Result: A weak negative correlation of -0.30 was observed.

3. Density Analysis
	•	Objective: To understand where most values are concentrated for each variable.
	•	Visualization: Scatter plot with density histograms on both axes.
	•	Observation: Step counts were densely concentrated around 4,000-10,000 steps, while social media usage clustered between 50-150 minutes.

4. Regression Analysis
	•	Objective: To explore the linear relationship between step counts and social media usage.
	•	Visualization: A scatter plot overlaid with a regression line.
	•	Observation: The regression line confirmed a slight negative trend.


Key Findings
	1.	Correlation:
	•	A weak negative correlation (-0.30) was identified between daily step counts and social media usage.
	•	Increased social media usage is associated with a slight decrease in physical activity.
	2.	Daily Trends:
	•	Social media usage showed consistent levels across the analyzed days.
	•	Step counts varied significantly, indicating external factors influencing physical activity.
	3.	Density and Distribution:
	•	Step counts were most frequently between 4,000 and 10,000, while social media usage was primarily between 50 and 150 minutes.


 Visualizations
	1.	Scatter Plot:
	•	Shows the relationship between step counts and social media usage.
	•	Highlighted areas of density where values are more frequent.
	2.	Line Plot:
	•	Compared daily step counts and social media usage trends over time.
	3.	Density Plot:
	•	Visualized the concentration of data points for both step counts and social media usage.
	4.	Heatmap:
	•	Displayed correlations between variables.

Example visualizations are saved in the /plots directory.


Future Improvements
	1.	Incorporating More Data:
	•	Include additional health metrics such as sleep duration or calorie counts to gain deeper insights.
	2.	Expanding the Time Range:
	•	Analyze a broader date range to observe long-term trends and patterns.
	3.	Automating Data Collection:
	•	Use APIs to automate the collection of social media usage data.



