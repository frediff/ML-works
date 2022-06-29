## HAC ##
We use the attached dataset `Twitter_data.csv`. The dataset contains the usage data of twitter along with the days of the week (Friday-Sunday). The columns present in the dataset are ‘TweetID’, ‘Day’, ‘Hour’, ‘Lang’, ‘IsReshare’, ‘Reach’, ‘RetweetCount’, ‘Likes’, ‘Sentiment’, ‘text’, ‘LocationID’, ’UserID’. We will use the data to cluster them according to the days of a week. 

Since the dataset might contain some missing values so in such cases we drop the rows. 
We drop the redundant columns if needed.

Now we separate the target column(‘Day’) from the dataset and convert it from categorical to integer.

We then visualize the dendogram of the data. 

After this we implement (from scratch) ***Hierarchical Agglomerative*** clustering with single and complete linkage both to cluster the dataset. 

Then we plot the resultant clusters in scatter plot. 

Finally we report the percentage accuracy of the clustering. 
