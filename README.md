# Movie-Genre-Prediction-from-Subtitles

# Problem/Business Motivation
Predicting movie genre by going through their subtitle scripts .

# Formulating The Problem
The subtitle scripts were tagged with the time stamps during which the dialogues happened , the scripts had to be pre - processed and cleaned in such a way that they contained only the dialogues, scripts for 100 movies were obtained and added to a list data structure. Eventually we ended up with a list of lists datastructure , where each list conatined dialogues from a particular movie.

# Approach
Carried out Topic Modeling on each of the movie scripts , obtained the percentage distribution of each movie for each of the six genres namely , 0 : Drama , 1 : Mystery / Adventure , 2 : Action , 3 : Thriller , 4 : Comedy / Romance , 5 : Science Fiction. Picked the genre for which the movie had the highest perecntage distribution. 

Topic Modeling was done after removing the stop words , a list of words that did not add  meaning to the dialogue and also Proper nouns(Plural and Singular). These words put together were added into a list and were passed into the tfidf vectorizer to carry out topic modeling . Also carried out a Doc2Vec approach to obtain the clusters , similarly Kmeans on LDA(Latent dirichlet Allocation) was also carried out.

Machine learning models such as ensemble models , Logistic Regression , Knn as well as SVM models were carried out , ROC curves and confusion matrices were used to show the results.

# Results 

Predictive analysis of the above mentioned approaches were carried out , among the NLP approaches LDA topic modeling and obtaining the percentage distribution of the movies in each of the genres produced the best accuracy , the results were encouraging it was twice as more compared to the baseline performance.

Among the Machine learning models , Logistic Regression and KNN produced the best results , both of which were able to triple the baseline performance.

# Future Work

- Over time the results could be improved further , by choosing the right set of words, distinct words that would differentiate topics as well as the words that belong to a particular part of speech that would be relevant to the genre,  by modeleing on these words  , we could predict most of the genres , hence produce a very high accuracy

- Identifying if a scene was emotional by carrying out sentiment analysis on dialogues that occur within a 20 minute interval, assuming each dialogue is roughly half a minute long

- Identifying the most important characters in the film , using n-grams as well as pos- tagging


