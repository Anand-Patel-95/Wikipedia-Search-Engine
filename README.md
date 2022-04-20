# Wikipedia-Search-Engine
Designed a custom PageRank algorithm in PySpark to find the most important Wikipedia pages for search results, with no error and within milliseconds, using parallel computing in Databricks and MapReduce in Spark to solve the graph problem.


# Files of Interest
- [iPython Notebook of Wikipedia PageRank](): Walks through the development of this PageRank algorithm. This code is customized to handle unbalanced edge weights and decimal edge weights. This PageRank implementation is packaged and used in other projects such as creating a flight delay network to find the most delay heavy airports in the United States: see [Notebook here](https://github.com/Anand-Patel-95/Predicting-Flight-Delays-for-Airlines/blob/main/EDA_anand_PageRank_starter.ipynb).
  - Note that the algorithm was run on a 2 GB subset, but is designed to run at scale in Spark on the entire 500GB dataset and will scale linearly in time with the dataset size.

# About the Data
The main dataset for this data consists of a subset of a 500GB dataset released by AWS in 2009. The data includes the source and metadata for all of the Wikimedia wikis. You can read more here: 
> https://aws.amazon.com/blogs/aws/new-public-data-set-wikipedia-xml-data. 

We'll be using a 2GB subset of this data, which is available to you in this dropbox folder: 
> https://www.dropbox.com/sh/2c0k5adwz36lkcw/AAAAKsjQfF9uHfv-X9mCqr9wa?dl=0. 
