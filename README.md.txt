# RoadVision AI 🚗

A beginner-level computer vision project built with PyTorch and trained to classify vehicle images into two categories: Automobile and Truck.

## Project Overview

RoadVision AI uses a Convolutional Neural Network (CNN) to learn visual patterns and classify vehicle images.

The project was developed using Google Colab with GPU acceleration.

## Technologies Used

- Python
- PyTorch
- Torchvision
- Google Colab
- Matplotlib
- Scikit-learn

## Dataset

The project uses a filtered subset of CIFAR-10:

- 10,000 training images
- 2,000 testing images
- 5,000 training images per class
- 1,000 testing images per class

Classes:
- Automobile
- Truck

Images were resized to 128 × 128 pixels.

## Model Architecture

A custom Convolutional Neural Network (CNN) consisting of:

- Three convolutional layers
- ReLU activation
- Max pooling
- Fully connected layers
- Dropout regularisation
- Two output classes

## Training Results

| Metric | Result |
|---|---:|
| Training accuracy (5 epochs) | 85.30% |
| Test accuracy | 83.55% |
| Test loss | 0.3705 |
| Correct test predictions | 1,671 / 2,000 |

## Classification Report

| Class | Precision | Recall | F1-score |
|---|---:|---:|---:|
| Automobile | 0.87 | 0.79 | 0.83 |
| Truck | 0.81 | 0.88 | 0.84 |

## Model Prediction

The model was tested with uploaded vehicle photographs and successfully returned a predicted class and confidence score.

Note: The CIFAR-10 dataset contains small, low-resolution images. Real-world photograph predictions are exploratory and have not yet been validated as reliable real-world vehicle recognition.

## Model File

`roadvision_cnn.pth` contains the trained model weights.

## Future Improvements

- Train with larger, real-world vehicle datasets.
- Improve generalisation to different lighting, angles and backgrounds.
- Explore object detection with bounding boxes.
- Extend classification to cars, buses, motorcycles and trucks.

## Author

Akintimehin Praise Olajide

- GitHub: https://github.com/ThaPriest2
- Portfolio: https://priestech-vision-forge.vercel.app