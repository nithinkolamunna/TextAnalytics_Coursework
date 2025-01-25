This tweet collection was done using a web crawler developed by John Baker Fish which crawled the twitter website to collect the data. It had over 100,000 tweets but since they were not annotated, had to cut down to just 3200 tweets which was randomly selected out of the dataset and manually annotated using a basic criterion:

Criteria for Labelling of tweets:
Tweet Class 1 - Comparing iphone x with other phone and telling other phone are better? No
Tweet Class 2 - Talking about good features of iphone x? Yes
Tweet Class 3 - Talking about negative features of iphone x? No 
Tweet Class 4 - Liked video on Youtube about iphone x? Yes
Tweet Class 5 - Anything else - Undefined

Intention to purchase was defined as a tweet having an action word such as (buy, want, desire) associated with it. Each tweet was read by 3 people and final class was decided by majority voting.

The tweets were preprocessed using these techniques in chronological order. First, by converting my text into lower case, to get case uniformity. Then removing punctuations and special characters. A negation handling technique described by Dan Jurafsky in Natural Language Processing was applied. It basically adds NOT_ to every word between a negation and following punctuation. Next stop words were removed for words that do not contribute to the meaning of the sentence. In addition the top 2 most common words were removed because their recurrence does not contribute to the meaning in the sentence. Some rare words were also removed such as proper names, brand words (except iphone x), and some html tags removal was done. Finally, words were stemmed using the Porter Stemmer. After preprocessing there are approx 2100 tweets in the dataset.


