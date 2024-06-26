# Sentiment Analysis of Airbnb Reviews 🏠

## Introduction:

The project is a deep learning work that focuses on conducting sentiment analysis on Airbnb reviews to extract valuable insights regarding guest sentiments and experiences. Sentiment analysis, a branch of natural language processing, enables the classification of text data into positive, negative, or neutral sentiments. Leveraging advanced deep learning techniques, the project aims to uncover nuanced sentiment patterns within the reviews, offering deeper insights into customer sentiments and preferences

## Project Steps

### Requirements:

To run this project successfully, please ensure you have the following dependencies installed:

```
pip install -r requirements.txt
```

And before running the code, make sure to also download NLTK resources:

```bash
python -m nltk.downloader stopwords
python -m nltk.downloader punkt
```

### Instructions for Dataset Access:
To get started, please download the Airbnb reviews dataset available at [Kaggle](https://www.kaggle.com/datasets/abhi8923shriv/sentiment-analysis-dataset) and save it to your local machine. Once downloaded, upload the dataset to your notebook environment using the following code:

```
df_reviews = pd.read_csv("path_to_your_downloaded_dataset/reviews.csv")
```

### Exploratory Data Analysis (EDA):
The project commences with an in-depth exploratory data analysis (EDA) of the Airbnb reviews dataset. Through statistical analyses and visualizations, the EDA phase aims to uncover patterns, distributions, and common themes within the reviews.

### Word2Vec Embedding:
Following the EDA, the project employs Word2Vec embedding to represent words in a continuous vector space. Word2Vec facilitates capturing semantic relationships between words, thereby enhancing the understanding of contextual similarities and differences.

### Clustering (KMeans) for Unlabeled Data:
Given the absence of labeled sentiment data in the dataset, the project utilizes clustering techniques, specifically KMeans clustering, to group similar reviews together based on their semantic similarities. Clustering enables the identification of distinct clusters within the unlabeled dataset, providing a foundation for subsequent sentiment analysis.

### Sentiment Analysis with Sentiment Intensity Analyzer (SIA):
In addition to Word2Vec embedding and clustering, the project incorporates sentiment analysis using the Sentiment Intensity Analyzer (SIA). SIA quantifies sentiment expression within each cluster, assigning sentiment scores to individual reviews and computing an overall sentiment score for the cluster.

### Interpreting the Results:

The numbers represent the average sentiment score for each cluster, both for the training and test datasets. The sentiment score ranges from -1 to 1, where:

A score close to 1 indicates a highly positive sentiment.
A score close to -1 indicates a highly negative sentiment.
A score around 0 indicates a neutral sentiment.

In summary, by analyzing the average sentiment scores for each cluster, we can understand the overall sentiment tendencies within the clusters. This information can provide insights into the sentiment distribution across different segments of the data.


## Conclusion:

The sentiment analysis of Airbnb reviews using Word2Vec embedding, clustering (KMeans), and Sentiment Intensity Analyzer (SIA) yields valuable insights into guest sentiments and experiences. Through the analysis, we were able to categorize reviews into distinct clusters based on semantic similarities and quantify the sentiment expression within each cluster. The project demonstrates the effectiveness of unsupervised learning techniques, particularly clustering, in extracting meaningful patterns from unlabeled text data and providing a comprehensive understanding of sentiment distribution.

## Benefits:

1. **Customer Insights**: The sentiment analysis provides valuable insights into customer sentiments, preferences, and experiences, enabling Airbnb to better understand guest satisfaction levels and identify areas for improvement.

2. **Personalized Recommendations**: By categorizing reviews into clusters, Airbnb can tailor recommendations and suggestions to individual guests based on their preferences and sentiments expressed in similar reviews.

3. **Enhanced Customer Engagement**: Understanding the sentiment distribution across different clusters allows Airbnb to engage with customers more effectively, addressing concerns, and responding to feedback in a timely manner.

4. **Product and Service Enhancement**: The analysis highlights both positive and negative aspects of the Airbnb experience, enabling the company to enhance its offerings, improve service quality, and optimize customer satisfaction.

5. **Data-Driven Decision Making**: Leveraging insights from sentiment analysis, Airbnb can make data-driven decisions regarding marketing strategies, product development, and customer relationship management, leading to improved business outcomes.

In conclusion, the sentiment analysis of Airbnb reviews offers actionable insights and strategic advantages for Airbnb to enhance customer experiences, drive customer loyalty, and optimize business performance in the competitive hospitality industry.
