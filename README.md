# Product_Review_Sentiment_Analysis
This analysis develops a sentiment classification framework for automatically categorizing
product reviews into positive, neutral and negative sentiments. The objective is to extract
actionable insights from customer feedback that can support product development, customer
service and brand communication. The dataset contains 1,007 product reviews with three
variables, with no missing values and two duplicate records that are removed during
preprocessing. Exploratory analysis shows a strong imbalance, with approximately 850 positive
reviews and around 75 reviews each in the neutral and negative categories. A pre-trained
Sentence Transformer all-MiniLM-L6-v2 is used to convert product reviews into sentence-
level embeddings. The embeddings are divided into training and testing sets using an 80:20
stratified split. Random Forest and Gradient Boosting classifiers are then trained and evaluated
using accuracy and F1-score. Random Forest achieves approximately 86.5% test accuracy and
81.8% F1-score, while Gradient Boosting achieves 84.07% accuracy and 80.3% F1-score.
Although both models achieve very high training performance, the difference between training
and testing results indicates some generalization gap. Random Forest is selected as the preferred
model because of its better test performance and lower generalization error. The analysis
demonstrates that transformer-based embeddings provide an effective representation of customer
reviews for multi-class sentiment classification.
