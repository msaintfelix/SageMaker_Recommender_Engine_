# Machine_Learning_SageMaker_Recommender_Engine_








# Objective

The objective of this project is to build a recommender engine with AWS SageMaker. The main goal is to recommend the top 20 movie selection to users that are clustered by preference similarities.

# Environment and tools

Our MovieLens dataset was downloaded from grouplens.org and more specifically we used movies.csv and ratings.csv from the ml-latest-small.zip file and uploaded to our AWS S3 bucket. We are working with a Jupyter Notebook with a conda_python3 framework in an AWS SageMaker environment. We used popular ML libraries such as Pandas, Matplotlib and Scikit-Learn to process the data.

# Project steps

	1. Inspect and visualize the data
	
In this section, we load the input data into dataframes to gain knowledge of it: dimensions and sizes, outliers.

	2. Prepare and transform the data

The next step is to put the data in a format a machine can learn from by combining disjointed data files into one, removing null values, doing some feature engineering.

	3. Train
	
After transforming the data, we can start the training process using the SageMaker built-in K-Means algorithm. The algorithm clusters users so that we can make recommendations. 

	6. Recommend
	
Now that we have identified our clusters, we can make recommendations based on weighted ratings from within each cluster. 
