
# Analysis of Political Opinions Using YouTube Data: A Case Study of the Palestinian-Israeli Conflict

## Overview

Due to high activity on social media, a large amount of data is generated each day, much of which relates to people's discussions, interactions, and attitudes towards events and trends, including political opinions. This project proposes an analytical study that uses a sample of YouTube comments data in different languages to measure and analyse international public opinion towards the Palestinian-Israeli conflict.

## Table of Contents

- Related Works
- Overview of the Proposed Approach
- Data Collection
- Data Pre-processing
- Political Attitude Analysis
- Data Analysis and Results
- Conclusion
- Future Work

## Related Works

Sentiment analysis is a major area of interest in Natural Language Processing (NLP). It involves the computational study of people's opinions, appraisals, attitudes, and emotions towards entities. Due to the vast amount of data related to people's opinions and attitudes on social media, many researches have focused on studying, analyzing, and predicting public opinion about conflicts.

For example, one study  [1] presents an analytical approach using Twitter data to measure political public opinion towards the Palestinian-Israeli conflict. Another work  [2] reports a text mining study on western media analysis to identify patterns and detect media bias towards one side or the other in the Palestine/Israel conflict.

## Overview of the Proposed Approach

The approach consists of the following steps: data collection, data pre-processing, and political sentiment analysis, selecting an appropriate classifier for this task. A case study utilizing the proposed model to analyze international public opinion is presented, along with details on data collection and pre-processing steps. Experiments are conducted to compare sentiment classifiers and train and evaluate a custom classifier.

## Data Collection

Apify, a cloud platform for web scraping, was used to scrape 2606 comments from videos shared by YouTube news channels. These comments were posted by 1981 users during the period from October 7, 2023, to December 24, 2023.

## Data Pre-processing

Comments were preprocessed by removing whitespace, converting to lowercase, normalizing emojis and emoticons, cleaning usernames, numbers, HTML tags, URLs, and punctuation, spell checking, translation, removing stop words, and lemmatization.

## Political Attitude Analysis

A supervised approach was used for sentiment analysis, training different models on a manually labeled dataset of 300 rows. The following table shows the performance of different classifiers:

| Model                    | Accuracy | Precision | Recall | F1-Score |
| ------------------------ | -------- | --------- | ------ | -------- |
| Multinomial Naïve Bayes | 63%      | 67%       | 76%    | 62%      |
| SVM                      | 57%      | 48%       | 58%    | 56%      |
| Xgboost                  | 47%      | 51%       | 58%    | 56%      |
| Bert base                | 50%      | 48%       | 62%    | 48%      |

## Data Analysis and Results

The sentiment classifier was used to measure the sentiments of 1106 English comments in the dataset. The following bar graph shows the distribution of sentiments across different news channels:

! [Sentiment Distribution by Channel](sentiment_distribution.png)

The results showed a high number of pro-Palestinian comments on NBC News, BBC News, and TRT World, indicating a shift in western media and public opinion towards Palestine.

## Conclusion

The study concludes that the October 7 war is a turning point in global public opinion towards the Palestinian-Israeli conflict, especially in western media, where previous bias towards Israel has decreased as people learn more about the history and context of the conflict.

## Future Work

Using YouTube comments for analysis is complex, as the comment is a reaction to the video content. New approaches are suggested, such as clustering videos based on context or classifying videos first based on titles or summaries before classifying comments.
