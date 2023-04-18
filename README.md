Project Overview
The project aims to build a movie recommendation system using K-Means clustering and PCA. The system will cluster users based on their movie preferences and recommend movies based on their cluster's preferences.

Tools and Libraries Used
Pandas
Scikit-learn (sklearn)
NumPy
Matplotlib
Seaborn
Data Collection
The data used in this project is obtained from the MovieLens 100K dataset. Two datasets were used:

u1.base: Contains 80,000 movie ratings by 943 users
u.item: Contains information about 1,682 movies
Data Preprocessing
The movie ratings dataset was loaded into a Pandas DataFrame, and the first few rows, shape, data types, and summary statistics of the data were printed.
The distribution of ratings was plotted using a histogram and a heatmap was plotted to show the correlation between the different movie ratings.
The movie dataset was also loaded into a Pandas DataFrame, and the first few rows, shape, data types, and summary statistics of the data were printed.
The number of movies released each year was plotted using a line plot.
A new DataFrame was created by merging the movie and rating datasets and pivoting the table to have the user ID as the index, movie titles as columns, and ratings as values.
The missing values in the new DataFrame were filled with zeros, and the movie ratings were normalized.
Clustering and Recommendation
K-Means clustering was applied to the normalized movie ratings DataFrame to group users based on their movie preferences.
The cluster labels were added to the DataFrame, and recommendations were made to a specific user based on their cluster's preferences.
The precision of the recommendations was calculated based on the number of correctly recommended movies.
Principal Component Analysis (PCA) was applied to the normalized movie ratings DataFrame to reduce the dimensionality of the data.
K-Means clustering was applied to the PCA-transformed data to group users based on their movie preferences.
Conclusion
In this project, a movie recommendation system was built using K-Means clustering and PCA. The system clusters users based on their movie preferences and recommends movies based on their cluster's preferences. The system's precision can be improved by using a larger dataset, improving the clustering algorithm's performance, and considering more factors, such as the users' demographic information.
