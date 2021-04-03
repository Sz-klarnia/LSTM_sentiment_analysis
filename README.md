# Classifying toxic comments with LSTM

# Data source:  
https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge

# Project info:  
Using data provided in Kaggle competition linked above I created a two step toxicity classifier for short web comments. In the first step, I classify the comments in two classes: toxic and non-toxic. In second step I train multiple binary classifiers for each type of toxicity in the set. I use multiple classifiers as opposed to single, multi-label classifier because some data needed resampling. For classes with imbalance close to 1:10 I augumented data using SMOTE and random undersampling to create better results. Still, some inbalanced classes only reach unsatisfactory levels of accuracy, measured by F1-score around 0.35 (raise from 0.0). More balanced classes produce better results, around F1-score of 0.8. Best solution to this problem would probably be feeding the model with additional data for inbalanced classes

# Further plans:
In the future I would like to use different techniques of oversampling to research if any of them create better results. I would also like to compress the models to smaller size.

# Additional info:  
Trained models can be accessed here: https://drive.google.com/drive/folders/1bR_7J8wmHQme6MDhkIYNOxvCG0AmXImx?usp=sharing
