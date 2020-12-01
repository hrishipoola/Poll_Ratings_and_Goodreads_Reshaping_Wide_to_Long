# Poll_Ratings_and_Goodreads_Reshaping_Wide_to_Long

Data is commonly in wide format, with rows being unique individual observations (no repeated records) and columns being features for each observation. However, long format, with each row being a single feature and multiple rows for each observation, is tidier as it's structured in key-value pairs and can be better for summarizing data and advanced analysis and plotting. Today, we'll work with the melt method and pd.wide_to_long function to reshape data from wide to long.

First, we'll work with FiveThirtyEight's ratings of 453 pollsters, used to weight polls with higher quality more than those with lower quality in forecasts (https://projects.fivethirtyeight.com/pollster-ratings/). We'll use the melt method to reshape the data from wide to long, focusing on the variables 538 grade, mean-reverted bias, and mean-reverted advanced plus minus. You can learn more about how FiveThirtyEight calculates pollster ratings here (https://fivethirtyeight.com/features/how-fivethirtyeight-calculates-pollster-ratings/).

Next, we'll work with Goodreads data on 50,000+ books. Since it has similar column names that can be broken down into suffixes and prefixes, we'll use the pd.wide_to_long function to reshape it from wide to long format, focusing on book title, page count, rating, and review count. Keep in mind that pd.wide_to_long creates a new multilevel index for the long dataframe.

The purpose is to reshape data from wide to long format so that it's tidier and can be used later for summary, analysis, and plotting.
