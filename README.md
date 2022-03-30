# Cityscape-Semantic-segmentation
This is a project done in a group for Advanced Machine Learning course at Sapienza University.
### Introduction
The goal of this project is to create a semantic segmentation-based model to detect with good accuracy the objects captured by the car. The images are captured in different cities in Germany and Switzerland. The original dataset is composed of 30 classes which include road, human, signs, etc. We introduced a novel model called super-resolution to check whether the accuracy of our models would improve. Another method we used is transfer learning which allows us to train models that are already pretrained.
### Dataset
Cityscapes data contains labeled videos taken from vehicles driven. The dataset has still images from the original videos, and the semantic segmentation labels are shown in images alongside the original image. It has 2975 training images files and 500 validation image files. Each image file is 256x512 pixels, and each file is a composite with the original photo on the left half of the image, alongside the labeled image (output of semantic segmentation) on the right half. The benchmarks that we are referring are the ones on the Kaggle competition.
### Models
We applied the UNet model for semantic segmentation. Actually we used it with different strate- gies as below:
1) Using the original images
2) Applying Super Resolution technique on the images and feeding the model with these images 3) Applying some data augmentation such as resizing, flipping vertically and horizontally, and feeding the model with the new images.
4) Using transfer learning. Important benchmarks that we used were mainly Dice Coefficient, Dice Loss, Jaccard distance, IoU.
