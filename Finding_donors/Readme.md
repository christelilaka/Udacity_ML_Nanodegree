# Project: Finding Donors for CharityML

In this project, we will employ several supervised algorithms to accurately model individuals' income using data collected from the 1994 U.S.Census. We will then choose the best candidate algorithm from preliminary results and further optimize this algorithm to best model the data.

Our goal with this implementation is to construct a model that accurately predicts wheter an individual makes more than \$50,000. This sort of task can arise in a non-profit setting, where organizations survive on donations. Understanding an individual's income can help a non-profit better understand how large of a donation to request, or whether or not they should reach out to begin with. While it can be difficult to determine an individual's general income bracket directly from public sources, we can (as we will see) infer this value from other publically available features.

The dataset for this project originates from the UCI Machine Learning Repository. The dataset was donated by Ron Kohavi and Barry Becker, after being published in the article "Scaling Up the Accuracy of Naive-Bayes Classifiers: A Decision-Tree Hybrid". The article by Ron Kohavi can be found online. The data we investigate here consists of small changes to the original dataset, such as removing the 'fnlwgt' feature and records with missing or ill-formatted entries.

Exploring the Data
We start by loading necessary Python libraries and the census data. As we can note that the last column from this dataset, 'income', will be our target label (whether an individual makes more than, or at most, $50,000 annually). All other columns are features about each individual in the census database.
