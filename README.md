Lung Cancer Detection Using CNN
Author

Chiranjit Sahu

Project Title

Lung Cancer Detection from CT Scan Images Using Convolutional Neural Network (CNN)

Project Description

Lung cancer is one of the most serious and life-threatening diseases worldwide. Early detection can help improve survival rates and assist doctors in making better treatment decisions.

This project uses a Convolutional Neural Network (CNN) to analyze CT scan images of lungs and classify them into different categories of lung cancer or normal lungs.

The model is trained on a dataset of CT scan images and can predict the type of lung cancer or healthy lung condition when a new CT scan image is provided as input.

Methodology

The following steps were followed in this project:

1. Data Collection

A publicly available Chest CT Scan Images dataset was used.
The dataset contains CT scan images of lungs classified into four categories:

Adenocarcinoma

Large Cell Carcinoma

Squamous Cell Carcinoma

Normal Lung

2. Data Preprocessing

Before training the model, the images were preprocessed by:

Resizing images to a fixed size (224 × 224)

Normalizing pixel values

Organizing images into training and validation folders

3. Model Development

A Convolutional Neural Network (CNN) was built using TensorFlow and Keras.

The CNN architecture includes:

Convolution layers for feature extraction

MaxPooling layers for dimensionality reduction

Fully connected dense layers for classification

Softmax output layer for multi-class prediction

4. Model Training

The model was trained using the training dataset for multiple epochs.
Validation data was used to evaluate the performance of the model during training.

5. Prediction

After training, the model can predict the class of a new CT scan image uploaded by the user.

The system outputs:

Predicted lung condition

Confidence score

Display of the input CT scan image

Results

The trained CNN model was able to classify CT scan images into the four lung categories.

Example output:

Detected Condition: Adenocarcinoma Lung Cancer
Confidence: 92.45 %

The results demonstrate that deep learning techniques can assist in identifying lung cancer patterns from CT scan images.

Conclusion

This project demonstrates the use of deep learning and convolutional neural networks in medical image classification. The model can assist in detecting lung cancer patterns from CT scan images and shows the potential of AI in medical diagnostics.


