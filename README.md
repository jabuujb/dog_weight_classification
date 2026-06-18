# Dog Weight Classification Using Deep Learning

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

---

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

---

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

---

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

---

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

---

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

## Key Findings

- Transfer learning significantly outperformed the custom CNN.
- GoogLeNet achieved the highest overall accuracy.
- DenseNet201 produced comparable classification performance.
- Larger pretrained models demonstrated improved feature extraction capabilities.
- Increasing training epochs would likely improve classification accuracy.

---

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

---

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

---

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
├── images/
│   ├── sample_predictions/
│   ├── model_architectures/
│   └── results/
│
├── README.md
├── requirements.txt
└── LICENSE
```

---

## References

1. Jesucristo (2019). Introducing DCGAN Dogs Images. Kaggle.
2. TensorFlow Documentation.
3. Keras Documentation.
4. ImageNet Pretrained Networks.

---

## Author

**Justin Ogle**

M.S. Electrical Engineering (Automation & Robotics)

Areas of Interest:
- Artificial Intelligence
- Machine Learning
- Computer Vision
- Robotics
- Defense Analytics

LinkedIn: https://www.linkedin.com/in/justin-ogle-b78233b0

GitHub: https://github.com/jabuujb
