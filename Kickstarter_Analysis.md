
# Kickstarter Analysis


## Overview of Project
The purpose of this analysis was to do a deep dive into crowdfunding data with intentions of isolating factors that are most likely responsible for successful play campaigns. 

### Analysis and Challenges
Filtering, formatting, finding averages, multiple advanced excel formulas, pivot tables, pivot charts, and line graphs were some of the ways that were used in this analysis to demonstrate trends in recognizing patterns and factors that played a huge role in successful play campaings.

My first challenge was creating the pivot table for "Theater Outcomes by Launch Date" to match the solution posted in our challenge module. To solve this, I tested by moving the values around in the different fields to see how each actoin behaved and that's how I ultimately got the table to match the solution posted. For the second challenge, I didn't know how to change the colors of the lines for that line chart to match the posted the solution so I did a Google search and found the solution for that. The third challenge that I ran that my line chart for "Outcomes Based on Goal" wasn't matcing the posted solution. When I realized my chart wasn't matching, I went back to check every cell and after some time of still not being able to figure it out, I took a break and came back. After I came back, I reviewed it again and realized my mistake was that I filtered out "plays" in the subcategory from the Kickstarter worksheet and that skewed all my data!

#### Analysis of Outcomes Based on Launch Date
For this analysis, I created a new sheet titled "Theater Outcomes Based by Launch Date." In this new sheet, I inserted a pivot table and added the following fields to the report: "Parent category" and "Years" into the Filters area, "Outcomes" into the Columns area, "Date Created Conversion" into the Rows area, and "Count of outcomes" into the Values area. Once those were set, I filtered out only "theaters" from the Parent category drop down. From there, I inserted a line chart so we can see a visualization of outcomes by launch date.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/111472879/187561647-277f8909-efc9-4008-9b43-7faf2998908a.png)

#### Analysis of Outcomes Based on Goals
For this analysis, I created a new sheet titled "Outcomes Based on Goals" then created columns and rows per the modules instructions on the type of data we were going to collect. For the "Number of Successful," I used the exel formula =COUNTIFS(Kickstarter!$D:$D,"<1000",Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays") and applied that to the rest of the remaining rows so it can populate the number of successful play for all the other ranges. For the "Number of Failed," I used the excel formula =COUNTIFS(Kickstarter!$D:$D,"<1000",Kickstarter!$F:$F,"failed",Kickstarter!$R:$R,"plays") and applied that to the rest of the remaining rows so it can populate the number of successful play for all the other ranges. For the "Number Canceled," I used the excel formula =COUNTIFS(Kickstarter!$D:$D,"<1000",Kickstarter!$F:$F,"canceled",Kickstarter!$R:$R,"plays") and applied that to the rest of the remaining rows so it can populate the number of successful play for all the other ranges. To Capture the "Total Projects," I used the excel formula =B2+C2+D2 and applied that to the remaining rows as well. To calculate the "Percentage Successful," I used the excel formula =B2/E2 and applied that to the remaining rows. To calculate the "Percentage Failed," I used the excel formula =C2/E2 and applied that to the remaining rows. To calculate the "Percentage Canceled," I used the excel formula =D2/E2 and applied that to the remaining rows. I then inserted a line chart to demonstrate the data.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/111472879/187561865-1cf25de6-a4ab-4d8c-9a39-4d43b2fb4977.png)

### Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    
    The first conclusion I can take away from the data is that the highest number of successful and highest number of failed plays occured when they were launched in May. The second conclusion I can see is that the lowest number of successful playes launched in December and the lowest number of failed plays launched in January and March.

- What can you conclude about the Outcomes based on Goals?

    I can conclude that plays were more likely to succeed with a lower set goal.

- What are some limitations of this dataset?

    We only get to see three years worth of data for plays.

- What are some other possible tables and/or graphs that we could create?
    
    Some examples of other possible tables and/or graphs that we could use are column charts, pie charts and/or bar charts.