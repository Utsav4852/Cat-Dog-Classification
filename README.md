# Cat-Dog-Classification

In this exerceise we have to perform classification with the help of CNN on the Cats-Vs-Dogs dataset. We will also perform preprocessing as we haven't provided with the split dataset. Download dataset from <a href='https://download.microsoft.com/download/3/E/1/3E1C3F21-ECDB-4869-8368-6DEBA77B919F/kagglecatsanddogs_3367a.zip'>Here</a>. This exercise will gives you basic knowledge of loading the data with image data generator, train the model with created from scratch and with the transfer learning technique.

## Cat-dog-dataset
This dataset contains total 25k images 12500 for each categories. This dataset is created by microsoft team and available on <a href='https://www.kaggle.com/c/dogs-vs-cats'>Kaggle</a> for competition. 

## Problem
We have given 2 classes 'Dog' and 'Cat' with total 25k images. Train the model that can classify the images within given class.

## Solution
I have splitted 90% images for training and 10% for testing purpose. Then with the help of <a href='https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/image/ImageDataGenerator'> ImageDataGenerator</a> load train and test data with standerdizing the data. Train the simple model created from scratch over those data. After successfully completing this task we will make some changes  like providing shear_range, width_shift_range, height_shift_range, zoom_range, horizontal_range, etc. in ImageDataGenerator to imrove the accuracy of model and we will pass these data to he model created from scratch and transfer learning model InceptionV2 with **imagenet** weight. At the end of the training we will try some images to check how well our model is performing with the unknown data.

![alt text](https://github.com/Utsav4852/Cat-Dog-Classification/blob/main/model_plot.png)

![alt_text](https://github.com/Utsav4852/Cat-Dog-Classification/blob/main/prediction.png)
