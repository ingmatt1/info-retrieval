# information-retrieval-search-engine

In-memory information retrieval system using a HashMap based inverted index and tf-idf scoring system that assigns weighted scores to documents based on their term frequency and inverse document frequency. 

Using Java, documents are indexed by a tokenizer and stored in an inverted index. After entering a query of words to search the set of documents for, an inverted index is constructed. The inverted index is composed of search words and the corresponding documents they appear in. 

Documents are scored and ranked based on the sum of their tf-idf scores.
tf-idf weighting is calculated as follows:

![capture](https://user-images.githubusercontent.com/55144676/82721131-90f9d980-9c88-11ea-9458-16561654f37d.png)

where
* tf: term frequency of term t in document d
* N: total number of documents
* df: number of documents the term appears in 

Documents are sorted and a list of the documents with the top scores are returned.


<img src="https://user-images.githubusercontent.com/55144676/87736692-d9c0a100-c7a6-11ea-8f77-625e5c5b34a9.png" width="400" height="500">

*Search query with set of scored documents.*
