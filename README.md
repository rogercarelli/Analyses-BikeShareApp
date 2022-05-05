# BIKE-SHARE CASE OF STUDY
## Scenario
The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, your team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, your team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve your recommendations, so they must be backed up with compelling data insights and professional data visualizations
About the company 

In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime. 
Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members. 

Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will be key to future growth. Rather than creating a marketing campaign that targets all-new customers.

Moreno believes there is a very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs. Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to do that, however, the marketing analyst team needs to better understand how annual members and casual riders differ, why casual riders would buy a membership, and how digital media could affect their marketing tactics. Moreno and her team are interested in analyzing the Cyclistic historical bike trip data to identify trends. 


Three questions to guide the future marketing program: 
* How do annual members and casual riders use Cyclistic bikes differently? 
* Why would casual riders buy Cyclistic annual memberships? 
* How can Cyclistic use digital media to influence casual riders to become members? 


Moreno has assigned you the first question to answer: How do annual members and casual riders use Cyclistic bikes differently? You will produce a report with the following deliverables: 
* A clear statement of the business task 
* A description of all data sources used 
* Documentation of any cleaning or manipulation of data
* A summary of your analysis 
* Supporting visualizations and key findings 
* Your top three recommendations based on your analysis

---
---

# DOCUMENTATION
## Business task 
Main objective is to answer the question: “How do annual members and casual riders use Cyclistic bikes differently?”
To break down the main objective, it is necessary to go deeper and answer some questions: 
  1.	What are the rider’s behaviors?
  2.	How do members use the bike?
  3.	How do casuals use the bike?
  4.	How far they ride? For how long?
  5.	How many members and casuals’ rides happened in the past 12 months?
  6.	How many times unique users ride the bike over the week?
  7.	Does the season affect the rides? 
The main source to get the above the answers is through data analyses and nothing more. Some information was provided in the Scenario file, but it was impossible to draw any initial thoughts.

## Data sources
The data has been made available by Motivate International Inc. under this license: [Data License Agreement | Divvy Bikes](https://ride.divvybikes.com/data-license-agreement)

Cyclistic’s historical trip data to analyze and identify trends is available in this link: Index of bucket ["divvy-tripdata"](https://divvy-tripdata.s3.amazonaws.com/index.html)

For the analyses, the data was downloaded from April 2021 to March 2022. Therefore, 12 “.csv” files were stored inside a folder called “ride_data”.
 
## Manipulation of data
For the data manipulation, Python (Jupyter Notebook) was used as main language to combine and clean the data.
After merging the past 12 months into one dataset, we could observe a 5+ million rows of data. To verify data integrity some steps were taken:

* Remove any rows with empty values. 
* Create a column with the ride duration in seconds.
  * If the duration is more than 24 hours or less than 60 seconds, the row was removed.

The steps above yielded a 4+ million rows dataset which were saved into a SQL database separated in three tables. All the steps taken for merging, cleaning and analyzing data was uploaded at GitHub for public access. 

To visualize the _data merging and cleaning file_, access the link:  [“data preparation from Roger’s GitHub”](https://github.com/rogercarelli/Analyses-BikeShareApp/blob/e3402797f6e563b78f53c7b04600d7deabc5b4bc/step-01_data_preparation.ipynb)

For the data analyses, the same programing language (python on jupyter notebook) was used. The analyses consist in working with the SQL database and Pandas Python’s library to identify trends, patterns and discrepancies. To visualize the generated data, the python’s library called Plotly was used, but GitHub is unable to show graphs. For a better understanding, Tableau was used to support the visuals. 

To visualize the _analyses_ file, access the link:  [“data analyses from Roger’s GitHub”](https://github.com/rogercarelli/Analyses-BikeShareApp/blob/e3402797f6e563b78f53c7b04600d7deabc5b4bc/analyses.ipynb)

To see the _Tableau’s dashboard_ with all the visuals, access the link: [“data visualization from Roger’s Public Tableau”](https://public.tableau.com/views/Analyses-BikeShareApp/Dashboard1?:language=pt-BR&:display_count=n&:origin=viz_share_link)
 
## Key findings and recommendations
xxxxxxx
