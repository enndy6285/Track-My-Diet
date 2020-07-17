# Track My Diet - Food Image Classifier

## Overview
What foods we eat is vital to our personal health, especially in regards to chronic health conditions. Unfortunately, current methods for diet tracking can be cumbersome and unreliable, often based on self-recall surveys. This project explores using computer vision for food classification to see if this can be applied to diet tracking.

## Objective
Build a food image classifer using convolutional neural networks

## Methodology
### Data
Data was obtained from the Food-11 image dataset developed by the Multimedia Signal Processing Group at the Swiss Federal Institute of Technology. It is available for download on [Kaggle](https://www.kaggle.com/vermaavi/food11). It consists of 16,643 food images grouped into 11 food categories.
### Preprocessing
Image augmentation was performed on training images.
### Modeling
A multi-class classifer was built with 8 target food category classes - Dairy/Egg, Dessert, Fried foods, Fruits/Vegetables, Grains, Meat, Seafood, Soup. The model was based on a convolutional neural network using Keras/Tensorflow. Transfer learning and then fine-tuning was performed on the pre-trained InceptionV3 model. 

## Results
An image classifier using convolutional neural networks was trained on the Food-11 dataset to achieve an accuracy rate of 89%.

## Project Files
1. readme.md - project summary
2. tmd_data.ipynb - Jupyter notebook for dataset preparation
3. tmd_model.ipynb - Jupyter notebook for training classification model
4. tmd_apps.ipynb - Jupyter notebook for applying model to real world data
5. track_my_diet_slides.pdf - Google slides presentation
6. food11_train.pkl - pickle file used for reading training images into Keras
7. food11_val.pkl - pickle file used for reading validation images into Keras
8. food11_test.pkl - pickle file used for reading test images into Keras
9. food11_all.pkl - pickle file used for reading additional training images into Keras

## Additional instructions
The notebook tmd_model.ipynb is the primary notebook for training the image classifier in this project. It was written to be run in Google Colab to take advantage of GPU processing. To reproduce results, it is recommended that the .pkl files and the food-11 dataset be saved in your local Google drive which can then be mounted to Google Colab. 
