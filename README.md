# An Analysis of Kickstarter Campaigns
## Overview of Project

An analysis of crowd sourcing goal outcomes conducted over a period of two weeks utilizes data provided by Kickstarter. The data includes over 4,000 crowd sourcing campaigns broken down into 9 different categories and over 40 sub-categories. This project focuses on the “theater” category, which represents 38% of the entire data set and is the most popular project category at nearly double the next closest.

### Purpose
A Kickstarter client requests a deeper analysis of campaign outcomes based on crowd source launch dates and funding goals. The client’s crowd sourcing interest area is the category "theaters" and specifically in the sub-category "plays". The client also expressed some interest in theater crowd funding launches in Great Britain, so some comparisons to the U.S. theater launches are provided.

## Analysis and Challenges

### Format and Clean Data
Before analysis of the data started, some basic formatting and cleanup occurred. Category and Subcategory theater/ plays was provided as a single column of data, so the column was split into two columns, category and subcategory, for more detailed analysis. The dates provided for the start and end launch dates were UNIX timestamped, so were converted to a ledgible date with the Excel formula: =(((timestamp_date)/60)/24)+DATE(1970,1,1). This conversion allowed for analysis of the launch dates to be presented in years and months. Finally, a column was added to the data set to identify the year of the launch date.

### Process for Analysis
Pivot tables and graphs were developed to get an overview of the data. Graphs include Theater Outcomes Based on Launch Date, and Outcomes Based on Goals. Several more graphs were developed and are included in this report as supporting evidence of results. Statistical analysis includes the mean, median, standard deviation and interquartile range for both successful and failed goals, and a box chart to help identify outliers.

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
Using the charts and tables below, the most successful launch dates for the theater category are May and June; however, May, June, July and August all experienced similar failed outcome numbers. The lowest number of successful launch dates occurred in December. Analysis based on the campaign's country of origin shows the U.S. had the most theater campaigns, with Great Britain next highests at 39% of the U.S. number; however, Great Britain experiences much higher campaign success rates than the U.S.

#### Graphs of theater outcomes based on launch:

Number of theater outcomes based on launch dates

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png" width="60%" height="40%">

Percentage of theater outcome success based on launch dates

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/Percentage_Theater_Outcomes_vs_Launch_All.png" width="60%" height="40%">

#### Graph of theater outcome numbers and success rates based on launch month - United States data:

Number of theater outcomes based on launch dates in U.S.

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/Theater_Outcomes_vs_Launch_US.png" width="60%" height="40%">

Percentage of theater outcome success based on launch dates in U.S.

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/Percentage_Theater_Outcomes_vs_Launch_US.png" width="60%" height="40%">

#### Graph of theater outcome numbers and success rates based on launch month - Great Britain data:

Number of theater outcomes based on launch dates in Great Britain

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/Theater_Outcomes_vs_Launch_GB.png" width="60%" height="40%">

Percentage of theater outcome success based on launch dates in Great Britain

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/Percentage_Theater_Outcomes_vs_Launch_GB.png" width="60%" height="40%">

### Analysis of Outcomes Based on Goals
To identify the most successful goal level, an array was created with the goal ranges: Less Than 1000, 1000 to 4999, 5000 to 9999, 10000 to 14999, 15000 to 19999, 20000 to 24999, 25000 to 29999, 30000 to 34999, 35000 to 39999, 40000 to 44999, 45000 to 49999, and Greater than 50000. Using this table with the percentage of outcomes by range, a graph was built that shows where the most successful goals occurred. In the graph, highly successful outcomes (above 70%) are clustered around Less than 1000 and 1000 to 4999. The problem with these results is the percentage successful line drops, but then rebounds between 25000 and 49999, and again at 50000 and greater.

#### Outcome Based on Goals

<img src ="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Resources/Outcomes_vs_Goals.png" width="60%" height="40%">

#### Outcome Based on Goals - Digging Deeper
This unexpected fluctuation required a deeper look at the data and found a number of outliers above $6000 goal levels. The two box charts below show the successful goals for all plays; the first includes outliers; the second excludes outliers above $6000, which provides a better visual distribution of the data around the median. The outliers distort the successful goal range, and suggests goals above $5000 might be successful; removing the outliers shows that is not the case, and that a goal range of $1000 - $3000 is more realistic.

#### Box Charts
The first box chart includes outliers.

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/box_chart_successful_play_goals_with_outliers.png" width="60%" height="40%">

The second box chart excludes goals above $6000 

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/box_chart_successful_play_goals_with_outliers_6000_over_removed.png" width="60%" height="40%">

#### Statistical Comparison of Goals and Pledges by Outcome; includes outliers

<img src ="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Images/descriptive_statistics_theater_plays.png" width="40%" height="40%">

### Challenges and Difficulties Encountered
A challenge in analyzing the data is the goals for theater projects have a range of $1 through $100,000 or more, and that some of these large goals were met. This variance signifies outliers, which surfaced during the development of this report. Although these outliers are not excluded from the data except to identify where they exist and visualize the data without them, further analysis may need to be done without the outliers, and perhaps a deeper dive into the outliers themselves may reveal why some of these higher goals were achieved.

There is also some concern with the data set itself. Although some of the data in the file is intuitive, there are some elements that are not defined, and may or may not have an impact on the results. For example, there was an associated column for all projects labeled Spotlight. This column may have an impact on the success of a project, but since it is unclear what this boolean column represents, it is not used in the analysis.

## Results
Below are the results derived from the analysis of the Kickstarter data related to the clients specific interests.

### Conclusions Based on Launch Dates
1. The most theater launches occur in May, at just under 170 projects launched.
2. The most successful launch month for theater campaigns occurs in May, of which 67% are successful.
3. Great Britain has higher numbers of successful launches in May and June, while the United States' highest successful launch month is May.
5. The least successful launch month for theater campaigns is in October, which has a comparatively higher number of failed lauches; November and December also experience lower success, but also much lower numbers of theater launches.
6. Although Great Britain has only about 40% of the theater campaign market, their campaign success rates run much higher overall; Great Britain campaign success is 73% for all years and months launched, compared to only 58% in the U.S.
7. Although there are fewer theater projects crowd sourced in Great Britain, the higher success rates (73% overall) would suggests it is a good location for theater crowd sourcing campaigns.

### Conclusions Based on Goal Outcomes
1. Goals for play projects experience success rates above 70% in the ranges of Less than $1000 and $1000 - $4999. 
2. The best chance of a successful goal outcome is in the range of $1000 - $3000.
3. The most successful goal level is between $2500 and $3000.

### Limitations of the Data
The data is provided as is, with no definitions included. There may be other factors that determine goal success in the data set, but without a full understanding of those elements, they cannot be used in the analysis. In addition, the goals were assumed to be U.S. dollars; however, a country currency column in the data may suggest the goal value should be converted. If the goal is not U.S. dollars, it could flaw the results.

### Other Possible Analyses
Although outside the scope of this report, it would be interesting to dig deeper into a comparison between goal levels and launch dates to look for trends between the two. If a definition of all data in the data set were provided, there may be other elements that contribute to the success or failure of a project, and would be interesting to explore. It may also be interesting to explore possible correlations between goal levels success and the number of backers.
