# Book-Genre-Classification
Classification of books into genres using cover and title.

We used the base convolution layers of pre-trained Xception model on ImageNet dataset to extract the cover features and used pre-trained GloVe model to get the feature vectors from pre-processed titles. The Xception model implementation was taken from keras and glove library for Python was used. 

A logistic regression model was used for the final classification. Scikit-learn was used to implement this. Using only the cover features, we got an accuracy of around 67%, using only GloVe around 86% and finally using both of these gave the best accuracy of 87%, beating even human accuracy. 

The main conclusion was that the title of the book tells us a lot more about the contents of the book when compared to it's cover. The entire project was done in Python. 
