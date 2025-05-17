# Netflix-Movies-and-TV-Shows-Clustering-Unsupervised-ML



![wed-may-3-2023-2-08-pm12906](https://github.com/user-attachments/assets/313f2e39-1838-477b-88d2-c55d5e743e2b)


## **Project Summary -**
This dataset consists of TV shows and movies on Netflix as of 2019. The dataset is collected from Flixable which is a third-party Netflix search engine. In 2018, they released an interesting report that shows that the number of TV shows on Netflix has nearly tripled since 2010. The streaming service’s number of movies has decreased by more than 2,000 titles since 2010, while its number of TV shows has almost tripled. It will be interesting to explore what all other insights can be obtained from the same dataset.

This project applies unsupervised machine learning techniques to analyze and cluster the Netflix Movies and TV Shows dataset. By **leveraging NLP-based textual preprocessing and clustering algorithms like K-Means and Agglomerative Hierarchical Clustering**, we uncover meaningful groupings within the content based on metadata such as titles, descriptions, country, rating, genres, and cast. The project also includes the development of a basic **content-based recommendation system to enhance user experience and engagement on the platform**.

* **show_id** : Unique identifier ID for every Movie / TV Show
* **type** : Identifier - A Movie or TV Show
* **title** : Title of the Movie / TV Show
* **director** : Name of the Director of the Movie or TV Show
* **cast** : Actors involved in the movie/show
* **country** : Country where the movie/show was produced
* **date_added** : Date the Movie or TV Show was added to it was added on Netflix
* **release_year** : Actual release year of the movie/show
* **rating**: TV Rating of the movie/show
* **duration** : Total Duration - in minutes or number of seasons
* **listed_in** : Genre(s) the title belongs to (like., Drama, Comedy)
* **description**: The summary of the Movie or TV Show


# **Conclusion**



**Insights from EDA**


* 🎬 **Content Composition:-** In this dataset, there are two types of contents.
    * The has **Movies for approximately 69.1% (5372)** of the content.
    * The has **TV Shows for approximately 30.9% (2398)** of the content.

* 🌍**Country-wise Contribution:-** 📍The **United States is the largest** contributor of content with **1,847 movies and 699 TV shows**.
    * **India follows as the second-largest** contributor, providing **852 movies/TV Shows**.
    * Other countries have a **medium to low level of contribution** compared to the United States and India, highlighting a significant content gap.
* 📺**Content Ratings**:- The Movie/TV Shows highlighting content ratings, Young Adults, and Family data are available.
* 🏷️**Genre Trends**:- Top **genres: International Movies, Dramas, Comedies, and Documentaries**. A clear audience interest in diverse, global, and emotionally engaging genres.
* 🕒 **Duration and Seasons:-** Movies mostly range between 80–120 minutes, peaking at **~90 minutes88. TV Shows often last 1–2 seasons, with **1 season being the most frequent**.

* 📅 **Release Trends:-** A most content year 2007 to 2021 Movies/TV shows.
* 📈 **Content Growth Over Time:-** A sharp increase in content additions **began in 2015, peaking between 2016 and 2020**.

* **These insights can guide content strategy, regional expansion, and offering business impact in terms of audience retention, content investment, and market penetration.**


**Insights from Machine Learning Model**

* Text data for analysis or modeling (NLP), textual data preprocessing. I used stop words, removed punctuation, stemming & TF-IDF vectorizer and other functions of NLP.

* Implemented **K-Means Clustering and Agglomerative Hierarchical Clustering**, to cluster the Netflix Movies TV show dataset.
* The optimal number of clusters we are getting from **K-means is 6**, whereas for **Agglomerative Hierarchical Clustering, the optimal number of clusters is found out to be 6**.
* We chose **Silhouette Score as the evaluation metric** over the distortion score because it provides a more intuitive and interpretable result. Also Silhouette score is less sensitive to the shape of the clusters.

*  Built a **Recommendation system** content-based recommendation system leveraging cosine similarity scores computed on TF-IDF vectors.

* Improve user experience by suggesting similar shows/movies based on previous interactions.
