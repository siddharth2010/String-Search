# String-Search

## Salient Features:

* Multiple Word Searching
* Stemming of Words (Eg:- Spelling -> spell; heroes -> hero). This feature helps us to ignore the form of verbs.
* Exact Searching:- If the query is contained in quotes then the results will contain exactly those results otherwise it may be in some other order. ( Eg:- searching for good boy will show both good boy as well as boy good, but when exact search is selected “good boy” only results of good boy will be shown.
* Indexing of Words:- Words present in stopword.dat files are not indexed as they are commonly used words and doesn't need indexing. Stemming of words is done before indexing them. Also, all words are indexed in lower case so that it is easy to search regardless of case of letters.
* Saving of Indexes:- Once you have indexed a file we save the indexes of it so that we don’t have to wait again for indexing it.
* GUI:- GTK+ has been used to make User Interface for this application, the key benefit of using this is it adapts to the theme you are using on your desktop
* Recent Searches:- Recent searches are stored in a file so that whenever you run you have them with you.
* Searches for txt files only.
* On click of a particular result the file opens from that particular Page Number or Line Number of File where the occurrence is present.
* Ranking is done by TF-IDF algorithm.
