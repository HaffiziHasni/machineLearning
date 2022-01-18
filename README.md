# machineLearning

This project essentially predicts whether or not a definition in the urban dictionary to be misogynist or not. The ML follows a random forest classifier (RFC) model approach with an accuracy score of 98.69% on the training data set and 87.11% on the test data set.

Initially a decision tree classifier was used as the prediction score on the train data sets was 99.89% however since the accuracy was 86.68% on the test data sets, RFC was chosen.

The finalized model was tested against testdata and it was 100% accurate although the unseen data has only 3 texts.

First, data was cleaned by removing any null value in the "is_misogyny" column in the ManualTag_Misogyny.csv file. Then to ease the model building, puncuations were removed. This can be seen at cleaning data file.

Next is only doing word clouding to give a graphical representation of word frequency in the cleaned_definition column and then it was separated according to whether or not the definitions are misogynistic or not.

take note to always ensure to vectorize unseen data with the previously used vectorizer. 
