# STEM Fellowhip Research Program 2021

Participants:  
Jatin Mehta  
Keval Patel  
Philip D'Costa  
Hibah Hussain  
Florence Ho  

Mentors:  
Jackie Peng  
Afnan Rahman  

Our team worked on a project to train machine learning models for sentiment classification of Twitter data (using the Sentiment 140 dataset). Then we applied the trained models to draw insights into the [D&G chopsticks ad controversy](https://www.cnn.com/style/article/dolce-and-gabbana-model-zuo-ye/index.html).  

The D&G Twitter data used for the project can be found in the Google Drive (not made public to those outside the project). The Sentiment 140 dataset was curated by a previously published paper and can be downloaded [here](http://help.sentiment140.com/for-students/).

`create_feature_matrices.ipynb` creates feature matrices from the tweets that are subsequently used to train the machine learning models. We trained four models to predict/classify the sentiment of a tweet (as negative, neutral, or positive): support vector machine, random forest, naive Bayes, and logistic regression. The code for model training can be found in `train_models.ipynb`. `aggregate_model_predictions.ipynb` uses the four classifiers' predictions to generate one overall prediciton. 

Finally, we applied the models on tweets related to the D&G chopsticks controversy (D&G chopsticks) and tweets related to D&G but not necessarily specific to the chopsticks controversy (D&G all). `create_time_series_figure.ipynb` creates figures that help visualize the sentiment towards D&G over time and `create_word_cloud_figure.ipynb` creates word clouds that highlight words used in the D&G tweets with a large positive or negative association. Figures are outputted in the `figures/` directory.    

`environment.yml` can be used to recreate the Conda environment (see https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file) and it lists all the required Python packages for this project.
