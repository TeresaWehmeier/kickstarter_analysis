# An Analysis of Kickstarter Campaigns
## Overview of Project

An analysis of crowd sourcing goal outcomes conducted over a period of two days utilizes data provided by Kickstarter. The data includes over 4,000 crowd sourcing campaigns broken down into 9 different categories and over 40 sub-categories. This project focuses on the “theater” category, which represents 38% of the entire data set and is the most popular project category at nearly double the next closest category.

### Purpose
A Kickstarter client requests a deeper analysis of campaign outcomes based on crowd source launch dates and funding goals. The client’s crowd sourcing interest area is the category of theaters and specifically with the sub-category of plays.

## Analysis and Challenges
The following actions were taken:
### Format and Cleaning Data
The targeted data in the Kickstarter data set was Category and Subcategory theater/ plays. Because this data was provided as a single column of data, the data was split into a category and subcategory for more detailed analysis. The dates provided for the start and end launch dates were timestamped, so the dates were converted to a ledgible date with the Excel formula: =(((timestamp_date)/60)/24)+DATE(1970,1,1). This conversion allowed for analysis of the launch dates to be presented in years and months.

### Overall Analysis
Pivot tables and chart were developed to get a snapshot of the entire data set. Initial findings include:
* Of the nearly 1400 theater campaigns, over 900 occurred in the US.
* Great Britain is a distant second behind the US in theater crowd sourcing campaigns at just under 360.
* There are three sub-categories within the theater category; “plays” represents a majority at just under 76%.
* 66% of all “play” crowd sourcing campaigns met the goal and none were canceled.

#### Parent Category by Outcomes

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/parent_category_by_outcomes.png" width="60%" height="40%">

#### Subcategories of Theater Campaign by Outcomes

<img src = "https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/theater_subcategories_by_outcomes.png" width="60%" height="40%">

Mean, median and Interquartile Ranges (IQR) were developed to determine the median of the data and to identify successful goal ranges. The image below is a statistical comparison of goals and pledges by outcome:

<img src ="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/descriptive_statistics_theater_plays.png" width="40%" height="40%">

### Analysis of Outcomes Based on Launch Date
Using the charts and tables below, launch date trends were evaluated. The most successful launch dates for the theater category were in May and June. Least successful launch dates occurred in December. Further analysis based on the campaign's country of origin shows the U.S. had the most theater campaigns, with Great Britain next highests at 39% of the U.S. number; however, Great Britain experiences much higher campaign success rates than the U.S.

#### Graph of theater outcomes based on launch:

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Theater_Outcomes_vs_Launch.png" width="60%" height="40%">

#### Graph of theater outcome success rates based on launch month - United States data:

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Theater_Outcomes_vs_Launch_US.png" width="60%" height="40%">

#### Graph of theater outcome success rates based on launch month - Great Britain data:

<img src="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/Theater_Outcomes_vs_Launch_GB.png" width="60%" height="40%">

#### Conclusions Based on Launch Dates
1. The most successful launch month for theater campaigns occurs in May, of which 67% are successful.
2. June also experiences above average campaign success.
3. Great Britain has a higher success rate in June, while the United States' highest successful launch month is May.
4. The least successful launch month for theater campaigns is in December at only 49% successful; these results are consistent across both countries.
5. Although Great Britain has only about 40% of the theater campaign market, their campaign success rates run much higher overall; Great Britain campaign success is 73% for all years and months launched, compared to only 58% in the U.S.

### Analysis of Outcomes Based on Goals
To determine the most successful goals, an array was created with the following goal ranges:


Statistical Comparison of Goals and Pledges by Outcome:

<img src ="https://github.com/TeresaWehmeier/kickstarter_analysis/blob/main/descriptive_statistics_theater_plays.png" width="40%" height="40%">



### Challenges and Difficulties Encountered

## Results


