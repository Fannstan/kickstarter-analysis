# Kickstarting with Excel

## Overview of Project
Louise is planning to launch a kickstarter campaign for a play that she wishes to present and has asked that she be given an analysis of kickstarter campaigns so that she can best decide when and how to best launch her own fundraising campaign.  The initial analysis provided to Louise included narrowing the kickstarter data down to that of campaigns that were launched in the US and for theater plays.  Information was also presented for measures of central tendency for both successful and failed campaigns, as well as an analysis of the months that showed the highest count of successful campaigns.  Louise launched her campaign for her play and it has come close to its fundraising goal shortly after the launch date.  With the fundraiser underway, Louise has asked for additional information regarding the success of kickstarter campaigns in relation to their launch date and fundraising goals.   

### Purpose
The purpose of this project is to show theater outcomes based on launch date and based on goal amount.  This information is shown both in table form and visualized by using charts.    

## Analysis and Challenges 

### Analysis of Outcomes Based on Launch Date
Within the Kickstarter_Challenge workbook, the sheet labeled 'Theater Outcomes by Launch Date' A pivot table was used to narrow down the data. The pivot table fields used were outcomes and date created conversion and the values used were the count of outcomes.  The pivot table was filtered by Parent Category and year.  The parent category was filtered down to 'theater' and the Outcomes columns were filtered to only include successful, failed, and canceled outcomes.  The pivot table was then put into chart form, with the Launch Date months on the X-axis and the count of outcomes on the Y-axis. 


![Theater_Outcomes_vs_Launch_Date](https://user-images.githubusercontent.com/103215123/164945957-a7fd3335-7702-470c-9576-65f55232f92e.png)




### Analysis of Outcomes Based on Goals
Within the Kickstarter_Challenge workbook, the sheet labeled 'Outcomes Based on Goals' contains a table where the fundraising Goal amounts are split into a set of ranges.  A countif() formula was used to pull in the number of successful, failed, or canceled outcomes within each goal range for the subcategory 'Plays'. The total number of projects within that goal range was also calculated and then used to determine the percentage successful, failed, or canceled.  A chart was then created to show the results found in the table, with the goal amounts listed on the X-axis and the Percentage Outcome listed on the Y-axis.  

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/103215123/164945788-ae91f4ee-b3b5-4e77-a6ab-edada55a01d8.png)



### Challenges and Difficulties Encountered
Some challenges or difficulties that I had was figuring out how to hide the field buttons that were on the pivot chart.  After searching in a couple of menus, I found that this can be done by going into the PivotChart Analyze tab and then going to the Field Buttons dropdown menu and selecting hide all. Another challenge that I can see coming up is that the Countifs() formula can be a little tedious to update for each outcome and the $ anchors must be used if you are going to copy the formula used in one column to another and then edit specific portions of the formula for the new column.  

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? 
  - The highest number of successful theater outcomes were launched in May and the second highest number of theater outcomes were launched in June.  The lowest number of failed theater outcomes was in November. The lowest number of launches was in the month of Dec and this month also showed to have the lowest number of successful launches.    

- What can you conclude about the Outcomes based on Goals?
  - The highest percentage of successful outcomes was in the goal range of less than $1000.  The goal range that had the most number of projects was $1000 to $4,999 and the percentage successful in this range was 73%.  The highest two goal ranges saw the highest percentages of failed outcomes.  

- What are some limitations of this dataset? 
  - The data for Theater Outcomes by Launch Date was only filtered down to the Parent Category of Theaters, so this data set may have included data (such as theater building or renovation campaigns) that was not as directly relevant to Louise who is launching a kickstarter campaign for a play.  The dataset used for Outcomes Based on Goals had no canceled outcomes, this would have also been shown on the Outcomes by Launch Date analyis if the subcategory had been used to filter the table.  

- What are some other possible tables and/or graphs that we could create?
  - Some other possible tables might filter down to the country that Louise plans to launch her Play.  Another table might also show outcomes based on goals for a specific year or narrowed down further to a specific month, to see the success and fail rates per goal range for that specific launch month. It might also be helpful to use a table to show information on the length of time that the campaign is open for, number of successful or failed outcomes or the goal amount ranges that fall within a one week campaign vs a 2 month campaign.  

