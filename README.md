# [Analysis of more than 515 thousand reviews for European hotels - Regression task - Project Overview:](https://t-ded.github.io/t-ded-portfolio/projects/project-1/)


## Project Summary

- Comprehensively <b>explored and visualized</b> the data, followed up by predicting score given by the reviewer with **RMSE of 0.73** points on 1-10 review scale.
- **Engineered multiple features** from the data, such as country of each hotel from address and length of stay from tags of each review.
- Performed **sentiment analysis** on text for each review, managed to find the most impactful pairs of words and how they affected the reviewer.
- Implemented **Regressive Histogram Gradient Boosting**, Linear Regression, and Random Forest algorithms, extracted **feature importance and performed feature selection**.
- Might actually bring **meaningful business implementation** for a company in a related field (both the algorithms and findings of my EDA).
- In the future, the continuous target variable may be transformed into an ordinal categorical one, enabling me to try classification algorithms.
- Also, a **clustering analysis** may be performed onto the reviewers, giving us even more precious insight into their demands and behaviour.

## Project Background

- This dataset has been chosen as it revolves around a topic which is close to almost anyone; apart from that it offers a possibility of an impactful business implementation.
- The [initial dataset](https://www.kaggle.com/jiashenliu/515k-hotel-reviews-data-in-europe) consists of 515738 reviews and 34 features, one of them being the reviewer score which is the dependent variable.
- For this project, EDA, visualisation and data interpretation have been given priority over algorithms as it seemed to me that for this particular dataset, it would be much easier to actually implement the results in the form of graphs, charts and plots into business, rather than estimator predictions and their coefficients.

## Project Outline

- State the initial hypotheses.
- Make necessary imports, take first look at the dataset.
- Extract country of each hotel from review and analyse hotel countries and reviewer nationalities.
- Find the best and worst hotels, analyse these extremes in relation to country of each hotel.
- Analysis of reviews in relation to time.
- Dive into tags - length of stay, with whom, purpose of the trip etc.
- Analyse reviews - positive, negative, lengths of each, sentiments.
- Inspect correlation.
- Implement models for regression tasks (multivariate linear regression, decision tree regressor, random forest reg.).

## Initial Hypotheses

- Long negative review will correspond to worse rating (vice versa for positive).
- Newer reviews of the same hotel will be better (improvements based on the reviews).
- Reviewer nationality influences the average given score.
- Some countries will have better hotels in general.
- People will prefer to visit hotels in their country and will give them better rating.
- Some words in positive/negative review will have big impact.
- Some tags will have an impact.

## Hypotheses after examination

- Length of negative (positive) reviews did have an impact; a feature of their mutual ratio has been engineered.
- Date of each review was not impactful, however in some months the individual hotels show similar review average pattern.
- Reviewer Nationality seemed impactful, nevertheless it is hard to say whether the reviewers from some countries tend to rate better in general or just pick better hotels.
- On average, there was not much of a difference between the individual hotel countries. However, some countries performed much better in terms of the extreme cases (top and worst 50 hotels).
- Apart from the increased number of reviewers, there is no correlation betweeen reviewer score and corresponding country of the reviewer and his or her hotel.
- Certain keywords in both negative and positive review have had a meaningful impact on the reviewer score, e.g. "air conditioning" or "nothing" in reviewers negative review.
- Specific features have been extracted from tags of each review; these features have been shown to have some effect on the reviewer score.

## Possible next steps

- Re-shaping the target variable into ordinal categorical one; this would allow me to inspect the data in terms of multivariate classification.
- Analysing the data from the perspective of clustering; that would enable us to dive deep into the reviewers, their demands and behaviour; this may have a massive impact on the business applicability of the project
