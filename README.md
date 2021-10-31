# Information Retrieval Tool for a collection of Financial Times articles

Goals:

- Implement appropriate pre-processing without external libraries: tokenisation, stemming, stop-word removal
- Create a positional inverted index for fast search
- Boolean Search
- Proximity Search
- Phrase Search
- Ranked IR based on TF-IDF

Files:

- trec.5000.xml : 5000 Financial Times articles in xml format
- englishST.txt : a list of english stop words to be ignored during indexing
- queries.boolean.txt : set of queries for boolean search
- results.boolean.txt : results corresponding to boolean queries, format: query_number, docID
- queries.ranked.txt : set of queries for ranked (TF-IDF) search
- results.ranked.txt : results corresponding to ranked queries, format: query_number, docID, score
- index.txt : positional inverted index, format: term, document frequency, then for each document: list of positions within document where term is located
