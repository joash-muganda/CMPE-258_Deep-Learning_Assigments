# Fruit Image Classification Using TensorFlow

## Overview
This project involves classifying fruit images using a Convolutional Neural Network (CNN) built with TensorFlow. The key component of this project is the utilization of TensorFlow's `ImageDataGenerator` for augmenting the dataset to enhance the model's ability to generalize.

## Dataset Preparation
The fruit images are organized into training and testing directories, with subdirectories for each class (e.g., apple, banana). Data augmentation techniques such as rotation, width shift, height shift, shear, zoom, and horizontal flip are applied to the training images to improve model robustness.

## Model Architecture
The CNN model consists of several layers:
- Conv2D layers for feature extraction, with ReLU activation functions.
- MaxPooling2D layers for downsampling.
- A Flatten layer to convert the 2D matrix data to a vector.
- Dense layers for classification, with a softmax activation function in the final layer to classify the fruit images.

## Training
The model is trained using the augmented images from the `ImageDataGenerator`. Parameters such as batch size, image height, and width are configured to fit the model's input requirements.

## Evaluation
After training, the model's performance is evaluated on a separate test set to ensure its accuracy and ability to generalize to new images.

## Usage
To use this project:
1. Prepare your dataset in the required structure.
2. Configure the `ImageDataGenerator` with your desired augmentation parameters.
3. Train the model using the training dataset.
4. Evaluate the model's performance on the test dataset.

## Dependencies
- TensorFlow
- Keras (included with TensorFlow)

## License
This project is released under the MIT License.
