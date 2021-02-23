# uniquemerchants

My approach for finding the Unique Merchants from the list:

1. First, data preprocessing is done by removing the special characters and changing every number to "NUM" string
2. Tokenizing each merchant name
3. Found set of unique words with their number of occurence in the whole list of Merchants
4. Then calculated the term frequency and inverse-document-frequency
5. With the help of tf-idf, each unique merchant name converted to vectors
6. Calculated the cosine similarity between each merchant name vectors
7. Names having cosine similarity > 0.9(hit and trail) are considered as same merchant.


**Note:**
1. Not much preprocessing was required like stemming, lemmatization & stopword removal since they are already in Unique Name format i.e. no grammar was involved in this task.
2. I have tried not to make much use of existing libraries except few places.
