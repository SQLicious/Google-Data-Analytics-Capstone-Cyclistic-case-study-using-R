# **Google Data Analytics Capstone Project Cyclistic-Case study**


This repository houses the final capstone project for the "Google Data Analytics" professional certificate on Coursera. It features a comprehensive dashboard demonstrating the practical application of data analysis and visualization in a business context.

**Key Highlights:**
- **Dashboard**: Explore the interactive visualization created in Tableau, providing clear insights derived from complex data analyses.
-  [View Dashboard](https://public.tableau.com/shared/27X7YYZ5X?:display_count=n&:origin=viz_share_link)

**Table of Contents**

Why this project?

Case study introduction

Scenario

About the company

Step 1: Ask

Step 2: Data Preparation

Step 3: Process (Data Wrangling)

Step 4: Analyze

Step 5: Share (Data Visualization)

Step 6: Act

**Why this project?**

This document was created as the final deliverable for the Google Data Analytics Capstone project. I started this certification program through Coursera in October 2022 and completed it in Feb 2023. Throughout each course in the Google Data Analytics Certificate, I developed the skills such as structured thinking, Storytelling, Excel, Tableau, SQL, and R. Through this project I am demonstrating the skills needed to transition into a career in data analytics.

**Introduction**

In this case study, you will perform many real-world tasks of a junior data analyst. You will work for a fictional company, Cyclistic, and meet different characters and team members. To answer the key business questions, you will follow the steps of the data analysis process: ask, prepare, process, analyze, share, and act.

This markdown file structure is modeled on the Data analysis process presented as part of the Google Data Analytics Certificate which is:

1. **Ask** : Business Challenge/Objective/Question
2. **Prepare** : Data generation, collection, storage, and data management
3. **Process** : Data cleaning/data integrity
4. **Analyze** : Data exploration, visualization, and analysis
5. **Share** : Communicating and interpreting results
6. **Act** :  Putting your insights to work to solve the problem

**Scenario**

You are a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company's future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations.

**About the company**

In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system at any time.

Cyclistic's finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, the Director of Marketing Moreno believes that maximizing the number of annual members will be critical to future growth.

Customers who purchase single-ride or full-day passes are called "casual riders". Customers who purchase annual memberships are Cyclistic "members".

**Step 1: Ask**

Three questions will guide the future marketing program:

1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

**Statement of business task**

**GOAL** : Analyze how annual members and casual riders use Cyclistic bikes differently. The insights from this analysis would be shared with the marketing team which would help them design marketing strategies aimed at converting casual riders into members.

**Stakeholders**

Primary Stakeholders: Director of Marketing (Lily Moreno), Cyclists Executive team

Secondary Stakeholders: Cyclistic marketing analytics team

**Step2: Data preparation**

The data we will be using is Cyclistic historical trip data from June 2021 to May 2022. The dataset used has been made available by Motivate International Inc. at [this link](https://divvy-tripdata.s3.amazonaws.com/index.html) under this [license](https://ride.divvybikes.com/data-license-agreement). It consists of 12 CSV files (each for a month). Each CSV has 13 columns with the corresponding number of observations.

The sheer volume of observations in each file could be a challenge using Excel to wrangle the combined as Excel took a while to perform calculations on all rows. So, we will use R programming to clean and wrangle the data. Also, a sample of the combined dataset was decided to be better due to computational limitations.

File name              Number of rows

202106-divvy-tripdata 729595

202107-divvy-tripdata 822410

202108-divvy-tripdata 804352

202109-divvy-tripdata 756147

202110-divvy-tripdata 631226

202111-divvy-tripdata 359978

202112-divvy-tripdata 247540

202201-divvy-tripdata 103770

202202-divvy-tripdata 115609

202203-divvy-tripdata 284042

202204-divvy-tripdata 371249

202205-divvy-tripdata 634858

Total number of rows in all 12 files: **5,860,776**

**ROCCC** approach was used to check issues with bias or credibility in this data.

- **R** eliability- The data is complete and accurate, and it represents all bike rides taken in the city of Chicago for the selected duration of our analysis.
- **O** riginal - The data is from Motivate International Inc, which operates the City of Chicago's Divvy bicycle-sharing service.
- **C** omprehensive- The data includes all relevant information about the ride including the type of bike, ride\_id, rideable\_type, started\_at, ended\_at, start\_station\_name,, start\_station\_id, end\_station\_name, end\_station\_id,
- **C** urrent- The data made available on the site are Up to date until Feb 2023
- **C** ited- The data is cited under divvy current license agreement: [Data Licence agreement](https://ride.divvybikes.com/data-license-agreement)

Dataset Limitations

A quick review of the datasets for completeness revealed that 'start\_station\_name' ,' start\_station\_id',end\_station\_name', and'end\_station\_id' are missing for some rides. Further observations suggest that the most missing data about "start station name" belongs to electric bikes

**Step 3: Process (Data Wrangling)**

Imported data in R studio.

Made columns consistent and merged them into a single data frame.

Checked for and treated missing values.

Transformed data-format types.

Added new columns

Removed the rows where trip duration is negative.

Cleaned column names and checked for duplicate records in rows.

**Step 4: Analyze the Data**

Summary of steps performed to identify trends or relationships I found in the data. Exported a summary file for further analysis.

1. Reviewed the Distribution of the Numerical Variables
2. Reviewed Categorical Variables
3. Checked Cardinality of Categorical Variables
4. Checked Outliers
5. Review Relationships between independent variables  and dependent variables
6. Performed Descriptive stats analysis

**Step 5: Share**

Tableau Public was used to show some key trends and patterns. Microsoft PowerPoint is used to present the key insights uncovered.

Cyclistic Bike Share Tableau story
<https://public.tableau.com/shared/T8Y8TWSN6?:display_count=n&:origin=viz_share_link>

**Step 6: Act**

Prepared the deliverables the Director of marketing asked us to create, including the three top recommendations based on my analysis.

Final conclusions

Here are my top 3 recommendations based on the above key findings:

Additional data you could use to expand on your findings?
