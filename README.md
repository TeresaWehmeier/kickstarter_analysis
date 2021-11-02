# An Analysis of Kickstarter Campaigns
## Overview of Project

An analysis of crowd sourcing goal outcomes conducted over a period of two weeks utilizes data provided by Kickstarter. The data includes over 4,000 crowd sourcing campaigns broken down into 9 different categories and over 40 sub-categories. This project focuses on the “theater” category, which represents 38% of the entire data set and is the most popular project category at nearly double the next closest.

### Purpose
A Kickstarter client requests a deeper analysis of campaign outcomes based on crowd source launch dates and funding goals. The client’s crowd sourcing interest area is the category "theaters" and specifically in the sub-category "plays".

## Analysis and Challenges

Before analysis of the data started, some basic formatting and cleanup occurred. Category and Subcategory theater/ plays was provided as a single column of data, so the column was split into two columns, category and subcategory, for more detailed analysis. The dates provided for the start and end launch dates were UNIX timestamped, so were converted to a ledgible date with the Excel formula: =(((timestamp_date)/60)/24)+DATE(1970,1,1). This conversion allowed for analysis of the launch dates to be presented in years and months. Finally, a column was added to the data set to identify the year of the launch date.

Pivot tables and charts were developed to get an overview of the data. Charts include Theater Outcomes Based on Launch Date, and Outcomes Based on Goals. Several more graphs were developed and are included in this report as supporting evidence of results.

Statistical analysis includes the mean, median, standard deviation and interquartile range for both successful and failed goals, and a box chart to help identify outliers.

Initial findings include:
* Of the nearly 1400 theater campaigns, over 900 occurred in the US.
* Great Britain is a distant second behind the US in theater crowd sourcing campaigns at just under 360.
* There are three sub-categories within the theater category; “plays” represent a majority at just under 76%.
* 66% of all “play” crowd sourcing campaigns met the goal and none were canceled.
* The most successful launch date for the theater category is May and June.
* Great Britain has more successful projects in both May and June; however, the U.S.'s successful launch month is May.
* Successful goals range between $1000 and $4000.

#### Parent Category by Outcomes
The parent category chart shows theater as the most popular category with a large number of successful project outcomes.

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/parent_category_by_outcomes.png" width="60%" height="40%">

#### Subcategories of Theater Campaign by Outcomes

The subcategories within theaters also shows plays are by far the most popular, also with a large number of successful project outcomes.

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/theater_subcategories_by_outcomes.png" width="60%" height="40%">

#### Descriptive Statistics

Mean, median and Interquartile Ranges (IQR) were developed to determine the median of the data and to aid in identify successful goal ranges. 

<img src ="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/descriptive_statistics_theater_plays.png" width="40%" height="40%">

#### Box Charts
Two box charts were built, the first showing all successful goals, including all outliers.

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/box_chart_successful_play_goals_with_outliers.png" width="60%" height="40%">

Another box chart was created with goals above $6000 removed, which provides a better visual distribution of the data around the median.

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/box_chart_successful_play_goals_with_outliers_6000_over_removed.png" width="60%" height="40%">

### Analysis of Outcomes Based on Launch Date
Using the charts and tables below, launch date trends were evaluated. The most successful launch dates for the theater category were in May and June; however, May, June, July and August all experienced similar failed outcome numbers. Least number of successful launch dates occurred in November and December. Analysis based on the campaign's country of origin shows the U.S. had the most theater campaigns, with Great Britain next highests at 39% of the U.S. number; however, Great Britain experiences much higher campaign success rates than the U.S.

#### Graph of theater outcomes based on launch:

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png" width="60%" height="40%">

#### Graph of theater outcome success rates based on launch month - United States data:

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/Theater_Outcomes_vs_Launch_US.png" width="60%" height="40%">

#### Graph of theater outcome success rates based on launch month - Great Britain data:

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/Theater_Outcomes_vs_Launch_GB.png" width="60%" height="40%">

#### Conclusions Based on Launch Dates
1. The most launches occur in May, at just under 120 projects launched.
2. The most successful launch month for theater campaigns occurs in May, of which 67% are successful.
3. June also experiences above average campaign success, but the majority of these successful launches are in Great Britain.
4. Great Britain has a higher success rate in May and June, while the United States' highest successful launch month is May.
5. The least successful launch month for theater campaigns is in October, which has the highest number of failed lauches; November and December also experience lower success, but also lower theater launches.
6. Although Great Britain has only about 40% of the theater campaign market, their campaign success rates run much higher overall; Great Britain campaign success is 73% for all years and months launched, compared to only 58% in the U.S. 

### Analysis of Outcomes Based on Goals

To identify the most successful goals, an array was created with the goal ranges: Less Than 1000, 1000 to 4999, 5000 to 9999, 10000 to 14999, 15000 to 19999, 20000 to 24999, 25000 to 29999, 30000 to 34999, 35000 to 39999, 40000 to 44999, 45000 to 49999, and Greater than 50000. Using this table with the percentage of outcomes by range, a graph was built that shows where the most successful goals occurred. In the graph the most successful outcomes are clustered around Less than 1000 and 1000 to 4999. The problem with these results is the percentage successful line continues to drop as expected, but then rebounds between 25000 and 49999.

This unexpected fluctuation required a deeper look at the data and found a significantg number of outliers above $5000 goal levels. The two box charts below show the successful goals for all plays; the first showing a significant number of outliers; the second excludes outliers above $6000, providing a better visual distribution of the data around the median.

#### Box Charts
The first box chart includes outliers.

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/box_chart_successful_play_goals_with_outliers.png" width="60%" height="40%">

The second box chart excludes goals above $6000 

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/box_chart_successful_play_goals_with_outliers_6000_over_removed.png" width="60%" height="40%">

#### Outcome Based on Goals

<img src ="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Resources/Outcomes_vs_Goals.png" width="60%" height="40%">

Statistical Comparison of Goals and Pledges by Outcome:

<img src ="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/descriptive_statistics_theater_plays.png" width="40%" height="40%">



### Challenges and Difficulties Encountered

## Results


