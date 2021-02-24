# Data-Wrangling

Data wrangling involves processing the data in various formats like - merging, grouping, concatenating etc. for the purpose of analyzing or getting them ready to be used with another set of data. Python has built-in features to apply these wrangling methods to various data sets to achieve the analytical goal. In this repo, I will show few examples describing these methods. For more info: [Wikipedia](https://en.wikipedia.org/wiki/Data_wrangling)

Data wrangling is part of nearly every machine learning project. It arguably presents the biggest risk if done incorrectly and is one of the more subjective aspects in the process. Several common techniques include:
 - Handling missing values: Some machine learning algorithms are capable of handling missing values, but most would rather not.  Options include:
 - Removing observations with missing values: This works well if only a very small fraction of observations have incomplete information.
 - Removing features with missing values: This works well if there are a small number of features which have a large number of missing values.
 - Imputing missing values: Entire [books](https://www.amazon.com/Flexible-Imputation-Missing-Interdisciplinary-Statistics/dp/1439868247) have been written on this topic, but common choices are replacing the missing value with the mode or mean of that column's non-missing values.
 - Converting categorical to numeric: The most common method is one hot encoding, which for each feature maps every distinct value of that column to its own feature which takes a value of 1 when the categorical feature is equal to that value, and 0 otherwise.
 - Oddly distributed data: Although for non-linear models like Gradient Boosted Trees, this has very limited implications, parametric models like regression can produce wildly inaccurate estimates when fed highly skewed data.  In some cases, simply taking the natural log of the features is sufficient to produce more normally distributed data.  In others, bucketing values into discrete ranges is helpful.  These buckets can then be treated as categorical variables and included in the model when one hot encoded.
 - Handling more complicated data types: Mainpulating images, text, or data at varying grains is left for other notebook templates.
