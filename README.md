# Dog Weight Classification Using Deep Learning
<img width="603" height="215" alt="image" src="https://github.com/user-attachments/assets/5529f4c4-9201-48f5-a20d-76de76ba3d65" />

## Overview

This project explores the use of Deep Learning and Computer Vision to classify dogs into weight categories based on images. Multiple neural network architectures were trained and evaluated, including a custom Convolutional Neural Network (CNN) and several pretrained transfer learning models.

This project was completed as part of EE 267 (Computer Vision & Deep Learning).

### Weight Classes

| Class | Weight Range |
|---------|---------|
| Small | 2 – 22 lbs |
| Medium | 24 – 57 lbs |
| Large | 59 – 99 lbs |
| Giant | 100+ lbs |


## Dataset

**Dataset Source:**
<img width="1284" height="203" alt="image" src="https://github.com/user-attachments/assets/51cc9565-21a0-499d-bf3f-c56222eaebc9" />
- Kaggle: Introducing DCGAN Dogs Images
- Link: https://www.kaggle.com/code/jesucristo/introducing-dcgan-dogs-images 

**Dataset Characteristics:**
- 120 dog breeds
- Originally 20,669 images
- Reduced to approximately 6,055 images for training efficiency
- Organized into Train, Validation, and Test folders

### Folder Structure

```text
Dataset/
├── Train/
├── Validation/
└── Test/
    ├── Small/
    ├── Medium/
    ├── Large/
    └── Giant/
```

## Configuration

This project was originally developed in Google Colab using Google Drive for dataset storage.
Before running the notebook, update the dataset paths to match your local or cloud storage configuration.

## Technologies

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?logo=plotly&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?logo=opencv&logoColor=white)

### Development Environment
- Jupyter Notebook
- Google Colab

### Deep Learning Models
- CNN
- VGG16
- AlexNet
- GoogLeNet (Inception)
- DenseNet201

## Methodology

### Data Preparation

1. Downloaded the Kaggle dog image dataset.
2. Organized all 120 breeds into weight classes.
3. Split images into:
   - Training
   - Validation
   - Testing
4. Applied image preprocessing and augmentation.

### Training Parameters

```python
Batch Size = 32
Epochs = 5
Learning Rate = 0.0001
```

### Models Evaluated

- CNN
- VGG16
- AlexNet
- GoogLeNet
- DenseNet201

## Results

### Overall Accuracy

| Model | Accuracy |
|---------|---------|
| CNN | 42.61% |
| AlexNet | 44.26% |
| VGG16 | 47.54% |
| DenseNet201 | 61.61% |
| GoogLeNet | 69.54% |

### Best Performing Models

#### GoogLeNet
- Highest overall accuracy
- 69.54% accuracy
- Correctly classified 5 of 6 test images

#### DenseNet201
- 61.61% accuracy
- Correctly classified 5 of 6 test images

## Example Test Images

| Test Image | Expected Weight Class |
|------------|----------------------|
| Image00 | Small |
| Image10 | Small |
| Image22 | Small |
| Image74 | Giant |
| The Best | Large |
| Wild | Medium |

---

<p align="center">
  <img width="1152" height="667" alt="image" src="https://github.com/user-attachments/assets/195e5b61-2909-4c78-9380-4c538e3e33ef" />
</p>

<p align="center">
  <em>Neural Network Test Image Match-up Results </em>
</p>

---

## Key Findings

- Transfer learning significantly outperformed the custom CNN.
- GoogLeNet achieved the highest overall accuracy.
- DenseNet201 produced comparable classification performance.
- Larger pretrained models demonstrated improved feature extraction capabilities.
- Increasing training epochs would likely improve classification accuracy.

## Project Demonstration

A video demonstration of the project, model performance, and classification results is available here:

[Watch Project Demonstration](https://youtu.be/EeUCic0kv9o)


## Future Improvements

Potential future enhancements include:

- Dog breed identification
- Mobile application deployment
- Real-time camera classification
- Expanded training dataset
- Additional training epochs
- Non-dog image rejection capability
- Improved subclassification of small dog breeds
- Model optimization for edge devices

## Skills Demonstrated

- Deep Learning
- Computer Vision
- Transfer Learning
- CNN Architecture Design
- Image Classification
- Data Preparation
- Model Evaluation
- Python Development
- TensorFlow/Keras
- Experimental Analysis

## Repository Structure

```text
dog-weight-classification/
│
├── notebooks/
│   └── EE_267_Final_Project.ipynb
│
├── report/
│   └── EE267_Final_Report.pdf
│
├── README.md
├── requirements.txt
└── LICENSE
```

## References


[1] Jesucristo. *Introducing DCGAN Dogs Images*. Kaggle, 2019.
   https://www.kaggle.com/code/jesucristo/introducing-dcgan-dogs-images
   
[2] TensorFlow Documentation.
   https://www.tensorflow.org/

[3] Keras Documentation.
   https://keras.io/

[4] ImageNet Dataset and Pretrained Models.
   https://www.image-net.org/

[5] Simonyan, K., & Zisserman, A. (2014). *Very Deep Convolutional Networks for Large-Scale Image Recognition (VGG16)*.

[6] Krizhevsky, A., Sutskever, I., & Hinton, G. E. (2012). *ImageNet Classification with Deep Convolutional Neural Networks (AlexNet)*.

[7] Szegedy, C., et al. (2016). *Rethinking the Inception Architecture for Computer Vision (InceptionV3)*.

[8] Huang, G., Liu, Z., Van Der Maaten, L., & Weinberger, K. Q. (2017). *Densely Connected Convolutional Networks (DenseNet)*.


## Author

**Justin Ogle**

M.S. Electrical Engineering (Automation & Robotics)

LinkedIn: https://www.linkedin.com/in/justin-ogle-b78233b0

GitHub: https://github.com/jabuujb
