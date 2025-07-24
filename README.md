Instagram Influencers Data Analysis Report

1. Introduction
This report provides a brief summary and analysis of the top_insta_influencers_data.csv dataset. The dataset contains information on 200 top Instagram influencers, including their performance metrics and geographical details.

2. Data Overview
The dataset comprises 10 columns and 200 rows. The columns include:

rank: Influencer's rank.

channel_info: Instagram handle/channel name.

influence_score: A score indicating influence.

posts: Number of posts.

followers: Number of followers.

avg_likes: Average likes per post.

60_day_eng_rate: 60-day engagement rate.

new_post_avg_like: Average likes on new posts.

total_likes: Total likes across all posts.

country: Country of origin.

Data Cleaning and Preprocessing
The initial inspection revealed that several numerical columns (posts, followers, avg_likes, new_post_avg_like, total_likes, 60_day_eng_rate) were stored as object (text) due to the presence of suffixes ('k' for thousands, 'm' for millions, 'b' for billions) and '%' signs.

The following cleaning steps were performed:

Suffix Removal and Numeric Conversion: For columns like posts, followers, avg_likes, new_post_avg_like, and total_likes, 'k', 'm', and 'b' suffixes were removed, and the values were converted to their corresponding numeric scale (e.g., '3.3k' became 3300, '475.8m' became 475,800,000).

Percentage Conversion: The 60_day_eng_rate column had '%' signs removed, and values were converted to decimal form (e.g., '1.39%' became 0.0139).

Missing Value Imputation:

One missing value in 60_day_eng_rate was imputed with the median of the column.

62 missing values in the country column were imputed with 'unknown'.
After cleaning, all relevant columns were successfully converted to appropriate numeric data types, and missing values were handled.

4. Key Findings and Analysis
Here's a closer look at the numbers that describe these Instagram influencers:

|   | Metric              | `rank` | `influence_score` | `posts`      | `followers`  | `avg_likes`  | `60_day_eng_rate` | `total_likes` |          |   |
|---|---------------------|--------|-------------------|--------------|--------------|--------------|-------------------|---------------|----------|---|
|   | :----------------   | :----- | :---------------- | :----------- | :----------- | :----------- | :---------------- | :------------ |          |   |
|   | **Count**           | 200    | 200               | 200          | 200          | 200          | 200               | 200           |          |   |
|   | **Mean**            | 100.5  | 81.82             | 3            | 499.85       | 77.41 M      | 1.79 M            | 1.90%         | 3.66 B   |   |
|   | **Min**             | 1      | 22                | 10           | 32.8 M       | 65           | 100               | 0.01%         | 18.3 M   |   |
|   | **Max**             | 200    | 93                | 17           | 500          | 475.8 M      | 15.4 M            | 26.41%        | 57.4 B   |   |

Observations:

Followers: The number of followers varies significantly, with a maximum of 475.8 million (Cristiano Ronaldo) and an average of approximately 77.4 million. This indicates a long tail distribution with a few highly followed accounts.

Engagement Rate: The average 60-day engagement rate is about 1.90%, but there's a wide range, from a very low 0.01% to a high of 26.41%, suggesting that follower count doesn't always directly correlate with engagement.

Posts: Influencers have a diverse posting frequency, from very few posts (min 10) to a high volume (max 17,500).

Geographical Distribution:
The country column shows a clear concentration of top Instagram influencers:

|   | Country                                       | Count |   |
|---|-----------------------------------------------|-------|---|
|   | :------                                       | :---- |   |
|   | United States                                 | 128   |   |
|   | Brazil                                        | 13    |   |
|   | India                                         | 12    |   |
|   | Indonesia                                     | 7     |   |
|   | France                                        | 6     |   |
|   | Spain                                         | 5     |   |
|   | United Kingdom                                | 4     |   |
|   | Colombia                                      | 3     |   |
|   | Canada                                        | 3     |   |
|   | *(Other countries with 1-2 influencers each)* | 18    |   |<img width="1133" height="636" alt="Instagram Influencers snapshot" src="https://github.com/user-attachments/assets/c2cda59b-a2a3-4bab-9d40-09af3830bc2c" />
<img width="1133" height="636" alt="Instagram Influencers snapshot" src="https://github.com/user-attachments/assets/2f7803b1-2ff1-4c1b-aa10-d932c81e4134" />


Observations:

Dominance of the United States: The vast majority of top influencers in this dataset are from the United States, accounting for 64% of the total.

Emerging Markets: Brazil and India also show a strong presence, highlighting their growing importance in the influencer landscape.

5. Conclusion
This dataset provides valuable insights into the top Instagram influencers, their reach, and engagement. The cleaning process was crucial to convert raw text data into a usable numeric format. The analysis reveals the significant scale of these influencers, the wide variance in their engagement, and the geographical concentration of influence, particularly in the United States. Further analysis could explore correlations between influence score, follower count, and engagement rate, or delve deeper into country-specific trends.

6. Recommendations
Based on this analysis, here are some key recommendations:

Prioritize Engagement: Focus on engagement rates and average likes over just follower count for better partnership results.

Target Key Geographies: Consider the U.S., Brazil, and India for primary marketing efforts.

Optimize Content: Experiment with posting frequency and content types to boost audience engagement.

Data-Driven Selection: Use engagement and audience data for more impactful collaborations.
