Improvement on Document Retrieval Using Various Tolerant Retrieval Methods

Implementation: (Steps)
(1) Bi-grams postings are build for both English as well as Hindi separately. Then using the Jaccard coefficient the list of the relevant word for each query term using Bi-gram posting with a threshold of 0.75 are selected. (Here the bi-gram posting is made of list of words {i.e. list of index of words} in which that bi-gram occurs)
(2) In order to resolve the conflict among selected words for a query term, edit distance is applied and put the closest word as the replacement for getting the final correct word.
(3) Updated query is fed as input to Boolean Retrieval Model to retrieve relevant docs.


-Queries here are words concatenated with conjuctions like and, or, not.
