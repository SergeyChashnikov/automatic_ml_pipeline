# automatic_ml_pipeline
for MLOps homework №1

1. Script data_creation.py generates various temperature data sets, including anomalies and noise, and stores them in the train and test folders.

2. Script model.preprocessing.py performs data preprocessing, using sklearn.preprocessing.StandardScaler.

3. Script model_preparation.py creates and trains a machine learning model using data from the train folder. The model used is logistic regression from the sklearn library. After training, the model is saved in .pkl format for further use.

4. Script model_testing.py tests the performance of a trained model on data from the test folder. The metrics accuracy, precision, recall, F1-score are used to evaluate the performance.

5. Script pipeline.sh sequentially launches all python scripts. The script also creates a virtual environment and installs the necessary dependencies from the requirements.txt file.

6. File requirements.txt contains dependencies that need to be installed.

To run a pipeline, clone the repository and run the command ./pipeline.sh in a terminal. You can changes number of dataset (by default, one dataset is created), for this run the command  with the number of datasets: ./pipeline.sh X, where X = number of datasets you want.

Make sure you have all the required dependencies installed, as specified in the requirements.txt file.