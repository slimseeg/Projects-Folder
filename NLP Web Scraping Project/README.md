# Project 3: Subreddit NLP Prediction

![Image of a house made of books](bookhouse.jpg)

### Problem Statement

**Business Context**:

Book House publishing is a children's book publisher. They're looking to rebrand their image and publish books that appeal to a larger, more mature audience. Two very popular genres are Horror Literature and Fantasy Literature. Book House Publishing wants to better understand these audiences and how to appeal to readers of these genres. 

Reddit is a popular social media platform where users can submit content, engage in discussions and participate in communities of like-minded individualts know as "subreddits." Reddit is also know as "the front page of the internet" because of the vast and diverse collection of user-generated content. For this reason its a good place to scrape data for this research that can be used for trageted marketing.

---


### Data Dictionary:

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**subreddit**|*int*|subreddits|Fantasy Lit: 0, Horror Lit: 1|
|**self_text**|*object*|subreddits|main body of text in a given post|
|**title**|*object*|subreddits|user assigned title for their given comment|
|**created_utc**|*float*|subreddits|unique identifier determined by when a comment was added|


#### Project Datasets
fantasy_data.csv
fantasy2_data.csv
final-fantasy-data.csv
horror_data.csv
horror2_data.csv
final-horror-data.csv
subreddits.csv

---

### Executive Summary

#### Conclusion and Recommendations

**Conclusions**
SpaCy lemmatization wasn't as effective as I thought it would be on this project.
In most models TfidfVectorizer had the greatest impact on improving the model scores, though not in all. Also, to achieve the best feature selection and prediction, robust gridsearching was necessary. 

Both Fantasy Literature and Horror Liturature subreddits had positive sentiment with respect to their preferred genre. Positive descripters were a key factor in every model correctly identifying which comment came from which subreddit. 

**Recommendations**
We have several trained models predicting at 94% accuracy. From here, I would suggest, as it pertains to the problem statement, that either genre would be favorable for Book House to branch into. Both genres have robust fan bases, with positive sentimentality towards their preferred genre.


