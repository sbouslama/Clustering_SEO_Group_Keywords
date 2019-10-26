# Case Study: Determination of Short Tail Keywords for Marketing
##data Set
AAAI 2013 Accepted Papers Data Set downloable from: https://archive.ics.uci.edu/ml/datasets/AAAI+2013+Accepted+Papers  

## features
Title: Free text; title of the paper   
Keywords: Free text; author-generated keywords   
Topics: Categorical; author-selected, low-level keywords from conference-provided list  
Groups: High-level keywords: Categorical; author-selected, high-level keywords from conference-provided list  

## Features exploration
The strategy for the determiation of short tail keywords for marketing is to cluster the papers in 10 different SEO keyword groups. We initally break the research papers into segments. We noticed that a given research paper can fall into more than one group and keyword.In clustering, the more the number of features fed in, the higher the chances to discover features that influence during the cluster discovery process. To be able to use the k-means algorithm, we also need to convert textual data into numerical data and use the existing four features to generate more features.

### Generation of features 
To make it simple, we are going to use the feature ''groups'' to generate features since it's composed of many values. So, we converted the “groups” feature into Boolean, such that a research paper that falls within a group will have 1 marked next to it, and 0 otherwise.
thus, we are going to have a matrix where the  columns will represent the different groups and rows will represent the research papers.
