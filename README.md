
# Movie Industry Research Report For Microsoft

## Overview
Microsoft, as one of the technology giant heads, is planning to expand its business territory to the movie industry by creating movies. To obtain initial understanding over the movie industry, Flatiron School Research Group is assigned with a project of using exploratory data analysis methods to gain insights over the movie industry to guide Microsoft to have a successful pivot into the movie industry. 

## Business Understanding

Launching a new business line by entering in a brand new industry takes lots of research. Initially, the research group has considered multiple factors that make a successful movie and eventually decided to narrow the deciding factors down to "Popularity in Genres" and "Return on Investment". For Microsoft's first movie, Flatiron School research group believes that it's critical to meet the taste of the majority of the audiences to broaden market share and to build brand recognition, which it also establishes a solid starting point for long term growth and expansion. Although popularity is critical, the research group has also conducted a return on investment research to explore the financial aspect of different genres within the movie market. By the end of the research, recommendations are provided to guide the Microsoft business team to formulate a business strategy for a successful entry to the movie industry.

## Data Understanding and Analysis

__Data Sources:

Flatiron Iron research group has collected the datasets from the following sources: 
1. Bom Movie movie_gross - not used in the research, too many missing values
2. IMdb Movie
3. Rotten Tomato - not used in the research, too many missing values
4. TMdb Movie
5. TN Movie

Other than the dataset, the research group has downloaded a Genre Glossary to help with data cleaning over movie “Genre” from Reddit: https://www.reddit.com/r/radarr/comments/70egj8/tmdb_genre_id_values/


__Data Constraints:

Missing data in the data set
Upon the initial observation of all the dataset, the research group found out that there are many missing data points. Strategy for fixing this issue: the research group has decided to drop the missing values as the final result doesn’t show a significant difference after comparing the median/mean before and after dropping the missing data points.
Timeframe of the data collection

Due to certain limitations, all the datasets downloaded captured the data prior to 2019. Therefore, some of the research findings may not be applicable to 2022. Further analysis may be required following the initial research project. 

__Data Preparation:

-In order to align the key data (Genre) for mapping the values, the research group use the Genre Glossary from Reddit to interpret to the “Genre id” from TMdb movie (through adding a genre_names):

<img width="984" alt="Screen Shot 2022-11-18 at 12 45 32 PM" src="https://user-images.githubusercontent.com/117051182/202781625-fb18c6ea-52ae-4c6a-a176-e99b53c32a36.png">

-Nans (null values) are cleaned up from all dataset through dropping for analysis. 

-As the research group is conducting analysis over the trend in years and months, columns for dates are reformatted to “Year” or “Month” depending on the study purpose. 

<img width="1021" alt="Screen Shot 2022-11-18 at 12 51 40 PM" src="https://user-images.githubusercontent.com/117051182/202781777-af6a50c2-0ea1-4665-8114-742b0691d722.png">

-Groupby function is used to construct and grasp key information for producing visual graphs. 


__Data analysis: 

The dataset that was used to study the population trend: TMdb. The research group started with pulling a popularity chart for all the values in the dataset (from year 1930 - 2019).

![bar plot](https://user-images.githubusercontent.com/117051182/202777454-99f3512e-2152-4d3c-ad11-a19d7c925c2e.png)

And the dataset for yearly trend from 1930 - 2019:

![popularity line chart](https://user-images.githubusercontent.com/117051182/202782050-6ad2ef35-724e-4c47-b060-3b201459fae1.png)

The insights from these results are not ideal due to unnecessary data points - it does not need to cover all the years to learn the move popularity trend in the analysis. Also, due to Covid 19 in 2019, which has caused the data to represent the value during extreme time periods. Therefore, the research group has decided to remove the years before 2012 and after 2018 to gain information over the trend for a five year timeframe from 2012- 2017. 

New charts for popularity distribution:

![download (1)](https://user-images.githubusercontent.com/117051182/202782189-1bb54ce1-f16b-480c-81f1-3686f5db4ffa.png)


Yearly popularity trend:

![line chartt](https://user-images.githubusercontent.com/117051182/202782225-4d21d461-5c70-41f7-b319-b9a2ad16a78c.png)


Based on the two graphs, the __top five popular genres are Adventure, Action, Fantasy, Crime, and War.


Another consideration is that overall movie ratings of the genres, the research group wonders if there are certain genres that get higher overall ratings. 

![boxplot ratings](https://user-images.githubusercontent.com/117051182/202782478-7ca208ca-0582-4707-8d27-45293bc50d14.png)

The results are Documentary, War, Music, Action, and History. This chart was then decided to NOT be used for making recommendations because of the sacrifices of return on investment in the next section for these genres. 

[Arun inserts]


Finally, after the top directors for the two genres are identified, the research group pulled a chart to find out the best month for releasing the movies in the recommended genres - Adventure and Fantasy.

![adventure fantasy](https://user-images.githubusercontent.com/117051182/202782805-c9ceb3ce-594b-40bc-99da-0d69d6e8447b.png)


## Conclusion
[Arun inserts]
