# Movie-recommender

A movie advisory program written in python using jupyter notebooks. 
The code imports the data, separates them from the csv file  in numpy arrays, one for each variable (i.e. title, genre,category and summary). I decided to use tf-idf for the assingment of weights in my context(list of the summaries of my movies) cause the bag words model is much less efficient, using the “Tfidfvectorizer()” function.

The code preprocesses the data(i.e. lemming and stemming) and filtering them (i.e. cutting of punctuation)  to use as a word tokenizer in my vectorizer

Finally the content_recommender was created as follows. The input the program asked was Id of target movie and number of max recommendations. Then an array is created using the cosine similarity metric between the target and all the other movies from the dataset, from best to worse. The printout is, the max_recommendations for said target movie. 
