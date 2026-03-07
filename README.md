# Lung Cancer Detection using CNN

This project aims to build a Lung Cancer Detection System using Convolutional Neural Networks (CNN). The model classifies lung cancer images into four categories: Normal, Adenocarcinoma, Large Cell Carcinoma, and Squamous Cell Carcinoma.

## Author: Chiranjit Sahu

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Methodology](#methodology)
- [Results](#results)
- [Acknowledgements](#acknowledgements)

## Introduction

Lung cancer is one of the leading causes of cancer-related deaths worldwide. Early detection and accurate classification are crucial for effective treatment and patient survival. This project leverages deep learning techniques to develop a robust lung cancer classification model using chest X-ray images.

## Dataset

The dataset used in this project consists of lung cancer images categorized into four classes:
1. Normal
2. Adenocarcinoma
3. Large Cell Carcinoma
4. Squamous Cell Carcinoma

The dataset should be organized into training (`train`), validation (`valid`), and testing (`test`) folders with the following subfolders for each class:

- `train/`
  - `normal/`
  - `adenocarcinoma/`
  - `large_cell_carcinoma/`
  - `squamous_cell_carcinoma/`

- `valid/`
  - `normal/`
  - `adenocarcinoma/`
  - `large_cell_carcinoma/`
  - `squamous_cell_carcinoma/`

- `test/`
  - `normal/`
  - `adenocarcinoma/`
  - `large_cell_carcinoma/`
  - `squamous_cell_carcinoma/`

Alternatively, you can also download a similar dataset from [Kaggle](https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images) which includes Chest CT scan images.

### Google Colab Link
To replicate and run the project in Google Colab, use the following link: [Lung Cancer Prediction System on Colab]https://colab.research.google.com/drive/1pmhqUX2C-bMWdFf3Na_Pa_kq040kkvSu#scrollTo=lkMToroUaOb5


### Usage

- **Direct Download**: You can download the dataset directly from this repository and store it on your local system.
- **Google Drive**: Alternatively, you can store the dataset in your Google Drive and mount it using the provided code to replicate the environment used in this project.

## Dependencies

The project requires the following libraries:
- Python 3.x
- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn
- tensorflow
- keras

You can install the required libraries using the following command:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn tensorflow keras
```

## Methodology
The project follows these main steps:

1. Data Collection

A publicly available Chest CT Scan Images dataset from Kaggle was used.

2. Data Preprocessing

The images were prepared before training by:

- Resizing images to 350 × 350 pixels

- Normalizing pixel values

- Organizing images into training, validation, and testing folders

- Applying ImageDataGenerator for data augmentation

3. Model Development

- A Transfer Learning approach using the Xception model was used.

Steps include:

- Loading the pretrained Xception model

- Freezing the base layers

- Adding custom classification layers

- Using GlobalAveragePooling2D and Dense layers

4. Model Training

- The model was trained using:

- Training dataset

- Validation dataset

- Adam optimizer

- Categorical cross-entropy loss

- Multiple training epochs

- Callbacks such as EarlyStopping and ModelCheckpoint were used to improve model performance.

5. Prediction

After training, the model can predict the class of new CT scan images uploaded by the user.

The output includes:

- Predicted lung condition

- Confidence score

- Display of the CT scan image


## Results

After training and evaluating the lung cancer prediction model, the following results were obtained:

- Final training accuracy: `history.history['accuracy'][-1]`
- Final validation accuracy: `history.history['val_accuracy'][-1]`
- Model accuracy: 90%


### Example Predictions


<img width="889" height="671" alt="image" src="https://github.com/user-attachments/assets/94a510cb-88bb-4d48-84c1-2fb93d6d3654" />

## After training, the model can be used to predict the class of a new CT scan image.
<img width="865" height="751" alt="image" src="https://github.com/user-attachments/assets/56f2aa5f-cfae-4852-ad9c-a89a1d695ac2" />



## Acknowledgements

We acknowledge and thank the contributors to the [Chest CT Scan Images Dataset](https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images) on Kaggle for providing the dataset used in this project.







