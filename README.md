# Detection-of-face-mask
Detecting face masks using Python, Keras, OpenCV on real video streams
Problem Statement
To detect whether or not a person is wearing a mask or not.

Dataset
This dataset contains a data folder which contains 2 subdirectories namely

1 without_mask - which contains 686 images without mask.
2 with mask- which contains 690 images with masks.
Image Preprocessing
All the images are not of the same size, and neural networks often expect images that are standardized; a fixed size. Therefore, the following preprocessing steps are performed:

1.Gray scaling
2.Normalize
3.Resize
4.Reshape

Model Building and Training :

1.Here a basic model is built using CNN and Keras library.
2.Model is first trained on both with and without masks images.
3.Then model is tested on sample test data. Whichever model is giving the good accuracy that model is saved for further use.

Model Prediction

The following steps are performed here:

1.Loading the previously saved model(best model) from training phase.
2.Using webcam to generate test images and prediction is made.
