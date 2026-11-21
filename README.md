# samsung-s26-launch-sentiment-analysis
## --- Executive Summary ----

This sentiment analysis was conducted to evaluate the consumer perception of Samsung smartphone launch. The data is from comments of the following youtube video "https://youtu.be/2gYqEi8-am4?si=-LiqYmAXNNEB1zBc". After the cleansing and preparing the data, 2669 comments analyzed by using VADER sentiment scoring and aspect-based text mining.

Overall distribution of the sentiments were found as 41.96% Positive, 39.42% Neutral, and 18.62% Negative comments with an Average Compound Score of 0.137. Even though the avarage compound score seems neutral, we can say that the overall launch performance is still looking positive because of the two-to-one ratio between positive and negative sentiments.

To get a deeper insights from the comments we decided to look up to the sentiment distributions of 6 categories(Camera, Ai & Software, Design & Display, Competitor, Price & Value, and lastly Battery & Performance). Most positively mentioned aspect was Camera(60.95%) quality and the customers mostly mentioned Battery & Performance(26.95%) as a complaint. 

An interesting part is that most liked negative comments had the design & display aspect. That is not surprising, though, because when we look at the 15 most frequently used negative phrases table, we see that two of the top three negative feedback items are related to privacy display and privacy screen. The reason for this is that the built-in privacy screen of the Galaxy S26 raised some questions among consumers.

Additionally, we see that the loyal customers of Samsung are complaining about the Galaxy S26 not having an S-pen which customers belive that one thing that makes the brand so unique. 


## ----Recommendations----

A: Samsung should immediately release a short-form FAQ video to clarify how the Privacy Display works and address consumers' questions and concerns.

B: For the loyal S-Pen community, Samsung should relay feedback to the product team and take it into consideration for future product iterations. Even a limited-edition Galaxy model equipped with an S-Pen could help Samsung win back the hearts of its most loyal customers.

## ----Tools----
**Language & Environment:** Python 3, Jupyter Notebook
* **Data Manipulation & Cleaning:** `Pandas`, `Regex (re)` — Used for JSON ingestion, deduplication, noise/spam filtering, and aspect explosion.
* **Language Detection:** `langdetect` — Used to filter the dataset to 2,669 English-language comments for consistent sentiment scoring.
* **Natural Language Processing (NLP) & Sentiment Analysis:** 
  * `NLTK (VADER)` — Used to compute compound sentiment scores (`-1` to `+1`) while preserving punctuation and emoji intensity.
  * `Scikit-Learn (CountVectorizer)` — Used for N-gram (bi-gram) extraction and custom stop-word filtering to uncover recurring complaint themes.
* **Data Visualization:** `Matplotlib`, `Seaborn` — Used to generate aspect-based stacked bar charts and negative phrase frequency visualizations.
