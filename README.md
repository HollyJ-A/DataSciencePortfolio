# Data Science Portfolio

## Overview
### Hello! My name's Holly. I have a passion for data science, and using insights to drive real change!  
I am a Data Science Apprentice, passionate about using data and statistical insights to fight for poweful causes, and telling untold stories. 
I am interested in many areas of data science, however I am particularly fascinated by AI and Machine Learning, and I will aim to explore this throughout later projects.

## Work Experience
### Data Analyst in Financial Services  September 2023-Present
I have started my career as a data analyst in financial services. As part of my role, I aim to improve the customer experience by utilising data to improve product offerings and processes.

## Education
### Level 4 Data Analyst
From September 2023 until March 2025, I completed the Level 4 Data Analyst apprenticeship, receiving a level 4 data analytics qualification.

From May 2025, I have started the Level 6 Data Science Apprenticeship, and am keen to learn even more about data skils.

## Projects
### An investigation into the impact Fast Fashion has on the environment 
# An investigation into the relationship between Fast Fasion Production and Climate change.

## Datasets used 
### Fast Fashion Dataset: https://www.kaggle.com/datasets/khushikyad001/the-true-cost-of-fast-fashion-impact/data
### Climate Change Dataset: https://www.kaggle.com/datasets/robjbutlermei/uk-daily-weather-1961-2024


## Code used
### Historic data analysis: http://localhost:8888/notebooks/StatisticalAnalysis.ipynb
### Correlation matrix: http://localhost:8888/notebooks/Correlationmatrix.ipynb

## Data Infrastructure and Tools
Within this project, a variety of different tools were used to gain the best understanding of the data.
Power Query was the tool used in data transformation, and was chosen because of its ability to automate data importing, reshaping and cleansing. 
Power BI was utilised to visualise the data in an interactive dashboard format. The aim of the dashboard was to explore the relationship between fast fashion and the climate. 
Power BI was an appropriate tool for this, largely due to its interactive capabilities. 
This project leveraged Python as a tool during the data analytics stages, specifically utilising Pandas and seaborn during data visualisation and EDA, and matplotlib during correlation analysis.
Pandas and seaborn were selected as Pandas easily loaded the data as a csv file into Jupyter notebooks, and seaborn was used to create visualisations that explored the relationship between the data.

## Data Engineering
First, the Climate dataset was cleansed, beginning with Null values being removed from the dataset. This decision was made, as imputation of the values would not be viable for this analysis, as weather data can be volatile, and rapidly fluctuate over a short period of time, meaning an imputed median or mode value may not be truly representative of the fluctuations. 
Following this, the data quality principal ‘consistency’ was checked. (UK Governmant Data Quality Framework, 2020). Some inconsistent formatting of the data in the precipitation column was identified, with most values being to 6 or 7 decimal places, while others were in the form of E-05. These values were converted using mathematical formulas, to having 6 decimal places, making them suitable for analysis.
Transformation also involved removing several years’ worth of data, as the project is only looking at climate data over the last 10 years, as this is the data available from the fashion dataset. To join the data using an inner join, the date columns would need the same value, therefore any data outside of this range was removed.
The group by function was then used, so that the format of grouping by year and month was consistent across both datasets. The climate data was grouped on the Year, and then the month, and then averages were created to fill these columns. The average of the monthly temperature, precipitation, windspeed, dewpoint temperature and runoff were calculated by Power Query and added as additional columns. 
The Fashion dataset was also transformed, following the same initial steps as the climate dataset. However, the fashion dataset was grouped by year, then country, and then brand, so that these groups could be highlighted when visualising the data, adding more than just volumes to analysis.

## Data Visualisation
This project utilised Power Bi for visualisations, through the creation of a dashboard to highlight key figures and explore the relationship between the climate and fashion data

Some key features of this visualisation were the 'cards'. These cards were used to call out key statistics around the impacts fast fashion has on the environment. This was an intentional chocie, as it meant that chronologically, if the dashboard was being read from left to right, the user would be shocked by the statistics immediatly, encouraging them to view the rest of the dashboard.

<img width="449" height="259" alt="image" src="https://github.com/user-attachments/assets/c3442743-f6be-4611-ab3f-a4f660be08a0" />

Another key feature of the dashboard was the forecast chart. This line chart visualised the historic change in temperature over the last 10 years. However, as the project involved exploring the deeper impacts of fast fashion on climate change, it felt crucial that the impacts were projected forward to explore the analysis deeper.

<img width="438" height="158" alt="image" src="https://github.com/user-attachments/assets/43e0dc70-ab1b-4ac9-aad8-b1466bc1014e" />




