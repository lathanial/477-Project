# 477-Project
Overview:
	While an individual can assume that generic seasonal patterns within the weather have a significant correlation to the sales of certain clothing products, this project investigates the correlation between the sales of seasonal products and unexpected and anomalous weather patterns (i.e., a warm fall or a cool spring). Climate variability is one of the biggest drivers in terms of things that affect consumer purchasing behavior in the fashion and retail space; understanding these patterns can help massive fashion companies, such as H&M or PacSun, optimize inventory management. Throughout the project, historical weather data along with retail sales data from various sources, such as the U.S. Census Bureau, will be used to identify any correlations between weather anomalies and clothing sales patterns.
	The project will specifically focus on identifying how anomalous weather impacts seasonal fashion item sales. This will ultimately positively impact the supply chains connected with multiple fashion corporations.

Research Questions:
	My primary question is: How do anomalous weather patterns affect seasonal clothing and accessories sales throughout the U.S.
	As for a couple of secondary questions, they would consist of:
Do warm fall/winter seasons lead to decreased cold-weather apparel sales?
Do unusually cold spring/summer seasons lead to increased purchasing of layering pieces during the season>
Which regions in particular (if there’s a variance) show strong correlations of anomalies equating to sales variations
Is there any lag time between weather event changes and sales changes?
Do weather anomalies have any affect on the sales growth overtime in the fashion sector?

Team: Lathanial Wells
	Due to constraints with my schedule this semester and constant flying back and forth between Illinois and California, I am working alone. As a result, I am solely responsible for all data acquisition, design integration, cleaning, etc.


Datasets: 
The first dataset I’d use right now is from the NOAA Climate Data Online. The dataset is accessed from https://www.ncei.noaa.gov/cdo-web/
The data format will be JSON.
The variables I’d want to collect are daily/monthly temperature, precipitation levels, date and time information, and temperature anomalies. 
The geographic coverage will consist of all of the U.S. climate zones. Timewise, the coverage would span over the past decade, as that is when the influx of fast fashion and more relevant seasonal pieces began to popularize.
The data is U.S. government data with no privacy concerns and is free to use.

The second dataset is from the U.S. Census Bureau. I am specifically accessing the retail sales data from that. The data format will be JSON.
The variables I will need to collect are:
Monthly sales figures for clothing accessories
Sales by region
Year-over-year percentage changes
The geographic coverage will be the same as the region of the previous data set.
The time coverage will also be of the last decade.
The data is public domain from the U.S. government. It’s also free to use.

The Data Integration Strategy will include temporal alignment to make sure that the data from both data sets is aligned. A lot of the data will be aggregated monthly for matching purposes. There will also be geographic alignment to ensure that there is no inaccurate analysis. Some of the key variables will be date/month, geographic, temperature, and sales figures.

Some potential challenges for integration would be with different geographic irregularities, given how the different data sources lay out the geographic data. Also some potential mishandling from weather stations. Configuring what is truly defined as anomalous weather could be a significant block for going forward with the project as well.

Time:
Week 1-2 | Setup and Data Acquisition | Module 3
	I will set up the GitHub repository, obtain the correct API tokens, verify data availability, and document some data sources and access methods.

Week 3-4 | Storage and Organization | Modules 4 & 5
	I will design the database scheme, create a filesystem structure, set up data validation, load our data into the database, and document the strategies for storage.

Weeks 5-6 | Data Integration and Quality Assessment | Modules 7-9
	I will create geographic mapping between the weather stations and Census regions from both data sets, define and configure anomalies, perform initial data quality assessments, and complete the status report.

Weeks 7-8 | Data Cleaning and Analysis | Module 10
	I will handle missing values and outliers, standardize formats, perform correlation analysis, create models, and generate visualizations.

Weeks 9-10 | Workflow Automation and Finalization | Remaining Modules
	I will create the metadata and data documentation, generate final visualizations, write the final report, and create the final GitHub release.

Addressing Course Requirements
	The project will directly address the DataOne Lifecycle for Module 1.
	Since the project uses publi domain data and both datasets have open data policies, ethical data handling within module 2 is satisfied.
	The data are from two distinct data sources with different formats. So Module 3 is addressed.
	There will be a solid filesystem structure along with a relational database model to address module 5.
	Module 6-8 will be addressed through calculating the anomalies and creating indices while also joining weather and saleys data and handling granularity differences.
	Module 9 will be addressed with profile completeness and consistency.
	Module 10 will be addressed with handling outliers and dealing with missing data.
	Modules 11 and 12 will be addressed with some automation practices, likely with Python,
	Module 13 will be addressed through completing documentation for the methods used so they can be accurately assessed if there’s a need for reproduction.
	Module 15 will be addressed through creating metadata.

Constraints:
	Some constraints that I will encounter are the lack of data availability for what is needed. Some temporal/time constraints will be encountered throughout the project given the recency of the data. Technically, as I am working alone, all the tasks will fall on me.

Gaps:
	I will need to determine the best approach for dealing with lag effects and mapping weather stations to Census regions.
	I will also need to determine if monthly data for aggregation is sufficient or if weekly analysis is feasible/better.
	There’s also many unknowns that I would not know that I don’t know. Data quality and integration challenges could be prevalent.
