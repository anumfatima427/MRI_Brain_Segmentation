# 🧠 MRI Segmentation using UNET 

This repository contains code for preparing an MRI dataset, splitting it into train and test sets, and training a UNET model for brain segmentation.

## Table of Contents

- 📝 [Introduction](#introduction)
- 📂 [Dataset Preparation](#dataset-preparation)
- 🔄 [Dataset Splitting](#dataset-splitting)
- 🚀 [Model Training](#model-training)
- 📦 [Dependencies](#dependencies)


## Introduction

This project aims to perform brain segmentation on MRI images using a UNET model. It includes three code files that handle different steps of the segmentation process.

- 📄 `1-Dataset Preparation.ipynb`: Converts 3D MRI volumes into 2D slices (coronal, axial, sagittal) to create the input data for the UNET model.
- 📄 `2- Train and Test Split.ipynb`: Splits the dataset into training and testing subsets to evaluate the model's performance.
- 📄 `3- Volume Segmentation Using U-Net.ipynb`: Trains a UNET model on the prepared dataset for brain segmentation.

## Dataset Preparation

Before using the code, you need to have an MRI dataset with corresponding brain masks. Place the MRI volumes and masks in separate directories and ensure that their filenames are consistent (e.g., image_001.nii.gz for MRI and image_001_mask.nii.gz for the corresponding mask). The `1-Dataset Preparation.ipynb` allows you to convert the 3D MRI into 2D slices in png format that can be used to train 2D segmentation models.

## Dataset Splitting

The `2- Train and Test Split.ipynb` script allows you to split the prepared dataset into training and testing sets. It randomly selects a portion of the data for testing, and the rest is used for training the model.

## Model Training

The `3- Volume Segmentation Using U-Net.ipynb` script trains a UNET model on the prepared dataset. The UNET architecture is widely used for image segmentation tasks, including brain segmentation. The trained model can be used to predict brain masks on new MRI images.


## Dependencies

- 🐍 Python 3.x
- 🧠 TensorFlow

