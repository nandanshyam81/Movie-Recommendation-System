# Movie-Recommendation-System
Developed a content based movie recommendation system that recommends movies to the user. If a user watches movie a movie, similar movies to that would be recommended.
For example, if a user watches a comedy movie starring Adam Sandler, the system will recommend them movies in the same genre or starring the same actor, or both. </br>

![image](https://user-images.githubusercontent.com/109072424/208283821-2c3883cb-dafc-48c4-91f2-b2ef2888d373.png)

## Overview 
The movie recommendation is based on the content of the movie searched for or wactched.Recommendation is done on te basis of genre,director and top 3 actors of the movie. </br>

> TF-IDF algorithm was used, TF stands for Term Frequency and IDF stands for Inverse Document Frequency.This algorithm is used to transform text into meaningful representation of numbers which is used to fit machine learning algorithm for prediction.  </br>

### TERM FREQUENCY </br>
Term frequency is how many times a particular term occurs in the document among the total number of terms in the document. </br>
>  tf=&nbsp; Number of times the term appears in the document</br>
&ensp;----------------------------------------------------------</br>
&emsp;Total number of terms in the document. </br>

### INVERSE DOCUMENT FREQUENCY </br>
The Inverse Document Frequency is a mesaure of whether a term is common or rare in a given document corpus.  </br>
The IDF of the word is the number of times documents in the corpus seperated by the frequency of the text. </br>
> idf=log(number of documents in the corpus/number of documents in the corpus containing the term). </br>
(Here log is said to be used because it dampens the effect of IDF).</br>

* The TF-IDF of a term is calculated by multiplying the TF and IDF scores.
> TF-IDF=tf*idf

### Note:
TF-IDF is better than Count Vectorizers because it not only focuses on the frequency of words present in the corpus but also provides the importance of the words.We can then remove the words that are less important for analysis, hence making the model building less complex by reducing the input dimenions.</br>

### How to decide which item is most similar to the item the user likes? 
> Similarity Score does the right job. </br>
> It is used to measure how similar are two items. It ranges between 0 and 1. Values which are  near to 1 or 1 are said to be highly similar where as values near to 0 are said to dissimilar. This can be done by cosine-similarity. </br>

### Cosine-Similarity 
Cosine similarity is used to measure how similar the documents are.It measures the angle between the vectors in a multidimensional space.The cosine similarity is benificial because of the size, they could still have a smaller angle between them.Smaller the angle, higher the similarity. </br>


