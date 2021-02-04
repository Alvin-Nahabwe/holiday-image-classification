# HackerEarth Deep Learning Holiday Season Challenge
(https://www.hackerearth.com/challenges/competitive/hackerearth-deep-learning-challenge-holidays)

Task:
You are given the following six categories. You are required to classify the images in the dataset based on these categories.
- Miscellaneous
- Christmas_Tree
- Jacket
- Candle
- Airplane
- Snowman

Approach:
- Pre-trained NASNetLarge model with fine-tuning
- Adam optimizer for initial fit and SDG optimizer with a low learning rate for fine-tuning
- Custom weighted loss function based on frequency of the classes
- Custom f1_score function using keras Precision and Recall metrics
- Early stopping and Dropout regularization to manage overfitting
- 20 epochs for initial fit, 50 epochs fine-tuning
- 90:10 train-validation split
- Batch size 32

Feature engineering:
- Manually one-hot encoded the class column to create columns for each class label in the train dataset
- Image augmentation

Tools:
- Google Colaboratory
- Tensorflow
- Keras
- Pandas
- Numpy
- Matplotlib
- Seaborn

Model f1_score:
- 81.5

Public leaderboard score:
- 90.5
