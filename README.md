# String-Search

## Salient Features:

* *Multiple Word Searching*
* *Stemming of Words* (Eg:- Spelling -> spell; heroes -> hero). This feature helps us to ignore the form of verbs.
* *Exact Searching*:- If the query is contained in quotes then the results will contain exactly those results otherwise it may be in some other order. ( Eg:- searching for good boy will show both good boy as well as boy good, but when exact search is selected “good boy” only results of good boy will be shown.
* *Indexing of Words*:- Words present in stopword.dat files are not indexed as they are commonly used words and doesn't need indexing. Stemming of words is done before indexing them. Also, all words are indexed in lower case so that it is easy to search regardless of case of letters.
* *Saving of Indexes*:- Once you have indexed a file we save the indexes of it so that we don’t have to wait again for indexing it.
* Ranking is done by *TF-IDF* algorithm.
* Searches for txt files only.


## Data Structures:

The data structures used in the project are Dictionary, Lists and Sets.
* Main Index Dictionary = { Word : { Book : { Page/Line : [occurrences] } } }
* Individual File Dictionary(The one that is saved) = { Word : { Page/Line : [occurrences] } }
* Answer = { Book : [Page/Line Numbers] }


## Future Improvements:

This is currently an ongoing project and I am planning to improve it further by adding some features like:
* *Did You Mean*:- If a particular word is not found then we apply did you mean to get results (This will be done using Peter Norvig's Did You Mean [Implementation](norvig.com/spell-correct.html))
* *GUI*:- I am planning to make a GTK+ User Interface for this ([GTK+ Documentation](https://python-gtk-3-tutorial.readthedocs.io/en/latest/))
* *Recent Searches*:- Add option to store the Recent searches in a file
* *Opening Files*:- On click of a particular result the file opens from that particular Page Number or Line Number of File where the occurrence is present.
