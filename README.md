# HCDS-A2-Data-bias
A2 Assignment

Referred from https://wiki.communitydata.science/Human_Centered_Data_Science_(Fall_2019)/Assignments#A2:_Bias_in_data
# Goal
The goal of this assignment is to explore the concept of bias through data on Wikipedia articles - specifically, articles on political figures from a variety of countries. We will combine a dataset of Wikipedia articles with a dataset of country populations, and use a machine learning service called ORES to estimate the quality of each article.
We perform an analysis of how the coverage of politicians on Wikipedia and the quality of articles about politicians varies between countries. 
The analyses consists of:
* the countries with the greatest and least coverage of politicians on Wikipedia compared to their population.
* the countries with the highest and lowest proportion of high quality articles about politicians.
* a ranking of geographic regions by articles-per-person and proportion of high quality articles.
* a short reflection on the project, that focuses on findings from this analysis and the process to reach those findings 


# Data Source
 The Wikipedia politicians by country dataset can be found on Figshare. Unzip and extract the file country which contains the file called page_data.csv.
The population data is available in CSV format in the Files section of Canvas under "A2: bias in data". This dataset is drawn from the world population datasheet published by the Population Reference Bureau.

* Wikipedia dataset:  https://figshare.com/articles/Untitled_Item/5513449 
Contains articles of category 'Politicians by nationality', country, revision_id of the page, Title of the page
* Population dataset:  https://canvas.uw.edu/courses/1319253/files/folder/A2%3A%20bias%20in%20data
Contains country and population info

* API used: The machine learning system Objective Revision Evaluation Service (ORES) API was used, to generate the article scores. Documentation for this API can be found at: https://www.mediawiki.org/wiki/ORES. This API returns one of the six following ratings for each article:

FA: Featured article
GA: Good article
B: B-class article
C: C-class article
Start: Start-class article
Stub: Stub-class article
FA is the highest rating, while Stub is the lowest

# License
MIT License
Wikipedia License: CC-BY-SA 4.0
Population data is copyrighted by the Population Reference Bureau (PRB)
ORES API is subject to the copyright agreement CC-BY-SA 3.0 license 

# Files

# Results

The results in the notebook consists of six tables as follows:
* 10 highest-ranked countries in terms of number of politician articles as a proportion of country population
Bottom 10 countries by coverage: 
* 10 lowest-ranked countries in terms of number of politician articles as a proportion of country population
* 10 highest-ranked countries in terms of the relative proportion of politician articles that are of GA and FA-quality
* 10 lowest-ranked countries in terms of the relative proportion of politician articles that are of GA and FA-quality
* Ranking of geographic regions (in descending order) in terms of the total count of politician articles from countries in each region as a proportion of total regional population
* Ranking of geographic regions (in descending order) in terms of the relative proportion of politician articles from countries in each region that are of GA and FA-quality
