Lung Cancer Prediction using CNN and Transfer Learning
Author

Chiranjit Sahu

Project Title

Lung Cancer Prediction Using Convolutional Neural Networks (CNN) and Transfer Learning

Project Description

Lung cancer is one of the leading causes of cancer-related deaths worldwide. Early detection and classification of lung cancer are important for improving patient survival rates.

This project develops a deep learning model using Convolutional Neural Networks (CNN) and transfer learning to classify lung CT scan images into four categories:

Normal

Adenocarcinoma

Large Cell Carcinoma

Squamous Cell Carcinoma

The model is trained on a dataset of lung CT scan images and can predict the type of lung condition when a new CT scan image is provided.

Methodology

The following steps were followed in this project:

1. Data Collection

A publicly available Chest CT Scan Images dataset from Kaggle was used.

Dataset Link:
https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images

The dataset contains CT scan images divided into four classes.

2. Data Preprocessing

Before training the model, the images were preprocessed by:

Resizing images to 350 × 350 pixels

Normalizing pixel values

Organizing images into train, validation, and test folders

Using ImageDataGenerator for augmentation

3. Model Development

The project uses Transfer Learning with the Xception model.

Steps include:

Load the pretrained Xception model

Freeze base model layers

Add custom layers for classification

Use GlobalAveragePooling2D and Dense layers

4. Model Training

The model is trained using:

Training dataset

Validation dataset

Adam optimizer

Categorical cross-entropy loss function

Multiple training epochs

Callbacks such as EarlyStopping and ModelCheckpoint are used to improve performance.

5. Prediction

After training, the model can predict the class of new CT scan images uploaded by the user.

The system outputs:

Predicted lung condition

Confidence score

Visualization of the input CT scan image

Results

After training the CNN model, the following results were obtained:
Final training accuracy: history.history['accuracy'][-1]
Final validation accuracy: history.history['val_accuracy'][-1]
Model accuracy: 90%
Example prediction output:

Detected Condition: Adenocarcinoma Lung Cancer
Confidence: 92.45 %

The model successfully classifies CT scan images into different lung cancer types with good accuracy.

Conclusion

This project demonstrates the use of deep learning and transfer learning techniques for lung cancer detection from CT scan images. The results show that CNN-based models can effectively assist in medical image classification and support early diagnosis.

Acknowledgements

Dataset provided by:

Chest CT Scan Images Dataset (Kaggle)
https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images
