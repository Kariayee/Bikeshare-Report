# Bikeshare-Report
PROJECT BACKGROUND

Cyclistic is a Bike-share offering company launched in 2016, equipped with a fleet of 5,824 bicycles available in three types; electric, classic and docked bikes. They employ a geo-tracking system in monitoring their bikes coupled with a network of 692 docking stations around the city of Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime.
On offer are two customer categories. Customers who purchase single-ride or full-day passes, referred to as CASUAL RIDERS and customers who purchase the annual membership called ANNUAL MEMBERS.

This project aims to understand how casual riders and annual members used Cyclistic’s bikes differently in the year 2022.

ABOUT DATA

The raw dataset was sourced from customer entries on the mobile app and the geo-tracking system utilized by the company. The dataset contains 12 tables, each representing a month in the year 2022. The tables contain 13 columns and multiple rows.
ANALYSIS PROCESS

For analysis all 12 tables were combined into a single table and transformed using Power Query before, being loaded into Microsoft Power BI for visualization. During transformation, the data was first carefully inspected for inconsistencies, formatting errors, and other signs of unclean data, that could negatively impact the result of the analysis.

After ascertaining the integrity of the dataset, next on the analysis process is exploration of the dataset, this is essential so as to ensure an accurate rendering of useful insights.

Furthermore, four new columns were created from the existing “Started_at” and “Ended_at” columns which contained date and timestamps. The new columns named “Start_date”, “Start_hour”, “End_date” and “End_hour” were created by twice duplicating the existing “Started_at” and “Ended_at” columns, the “Start_date” and “End_date” columns were converted into a date format, while the “Start_hour” and “End_hour” columns were transformed into time (Hours) formats. Next, to calculate the duration of each ride, a custom column “ride_duration” was created by subtracting the “End_hour” from the “Start_hour”.  

INSIGHTS

•	The analysis shows that number of rides peak in the second and third quarter of the year, during spring and summer months. We get the highest ride count in July for casual riders and August for member riders.
•	Accounting for 53.03% of total rides, we see registered members use Cyclistic bikes more than casual riders. Though not significantly.   
•	With regards to the bike types, the analysis shows riders both members and casuals significantly favor the classic and electric bikes, with users of the docked bike only coming in among casual riders.
•	Also revealed in the analysis is the average ride duration. It shows casual riders clocking in a slightly higher ride duration average than member riders. 
