# Book-Genre-Classification
Classification of books into genres using cover and title.

We used the base convolution layers of pre-trained Xception model on ImageNet dataset to extract the cover features and used pre-trained GloVe model to get the feature vectors from pre-processed titles. The Xception model implementation was taken from keras and glove library for Python was used. 

A logistic regression model was used for the final classification. Scikit-learn was used to implement this. Using only the cover features, we got an accuracy of around 67%, using only GloVe around 86% and finally using both of these gave the best accuracy of 87%, beating even human accuracy. 

The main conclusion was that the title of the book tells us a lot more about the contents of the book when compared to it's cover. The entire project was done in Python. 

Xcetion+Glove1 jupyter notebook has the necessary code. Many features were extracted using on the fly code and saved into pickle files, which are being imported in the give jupyer notebook. Since some of these saved pickle files are pre-trained GloVe vectors, they are around 250 MB, which exceed GitHub's requirment that each file be less than 25 MB. Because of this, we are not able to provide them right now, but the repository will be updated with a external link to download them. 
