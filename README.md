# information-retrieval-search-engine


In-memory information retrieval system using a HashMap based inverted index and tf-idf scoring system that assigns weighted scores to documents based on their term frequency and inverse document frequency. 

Documents are indexed by a tokenizer and stored in an inverted index. After entering a query of words to search the set of documents for, an inverted index is constructed. The inverted index is composed of search words and the corresponding documents they appear in. 

Documents are scored and ranked based on the sum of their tf-idf scores.
tf-idf weighting is calculated as follows:

![tfidf formula](https://user-images.githubusercontent.com/55144676/82619598-6171a100-9ba4-11ea-8751-ac9216e9249a.PNG)

where
tf: term frequency of term t in document d
N: total number of documents
df: number of documents the term appears in 

Documents are sorted and a list of the documents with the top scores are returned.


