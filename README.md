🫁 Lung Cancer Detection Using CNN
📌 Project Overview

Lung cancer is one of the leading causes of cancer-related deaths worldwide. Early detection can significantly improve survival rates.

This project uses a Convolutional Neural Network (CNN) to analyze CT scan images of lungs and predict whether the lung is healthy or affected by different types of lung cancer.

The system is trained on a CT scan image dataset and can predict the class of a new CT scan image uploaded by the user.

🎯 Objectives

Detect lung cancer from CT scan images using deep learning.

Classify lung images into different cancer categories.

Provide user-readable prediction results.

Allow users to upload their own CT scan image for prediction.

🧠 Technologies Used

Python

TensorFlow / Keras

CNN (Convolutional Neural Network)

NumPy

Matplotlib

OpenDatasets

Google Colab / Jupyter Notebook

📂 Dataset

Dataset used in this project:

Chest CT Scan Images Dataset from Kaggle.

The dataset contains 4 classes of CT scan images:

Adenocarcinoma

Large Cell Carcinoma

Squamous Cell Carcinoma

Normal Lung

Dataset link:

https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images

⚙️ Project Workflow
1️⃣ Dataset Download

The dataset is downloaded using OpenDatasets from Kaggle.

2️⃣ Data Preprocessing

Image resizing

Normalization

Data augmentation

3️⃣ Model Building

A CNN model is built using TensorFlow/Keras including:

Convolution layers

MaxPooling layers

Fully connected layers

4️⃣ Model Training

The model is trained using:

Training dataset

Validation dataset

Multiple epochs

5️⃣ Prediction

Users can upload a new CT scan image, and the model will predict:

Cancer Type

Confidence Score

🏗 Model Architecture

The CNN model consists of:

Conv2D Layer

MaxPooling Layer

Flatten Layer

Dense Layers

Softmax Output Layer

Output classes = 4

▶️ How to Run the Project
1️⃣ Install Required Libraries
pip install tensorflow
pip install opendatasets
pip install numpy
pip install matplotlib
2️⃣ Download Dataset
import opendatasets as od

dataset_url = "https://www.kaggle.com/datasets/mohamedhanyyy/chest-ctscan-images"
od.download(dataset_url)
3️⃣ Train the Model

Run the training cells in the notebook to train the CNN model.

4️⃣ Predict Using a New CT Scan
predict_uploaded_image("ctscan_input.jpg")

The model will output:

Detected Condition: Adenocarcinoma Lung Cancer
Confidence: 94.23 %
📊 Output

The system displays:

CT scan image

Predicted cancer type

Prediction confidence

🚀 Features

Automatic dataset download

CNN-based classification

Image upload prediction

User-readable output

Visualization of predictions

⚠️ Limitations

Accuracy depends on dataset size and quality.

The model is intended for educational purposes only and not for clinical diagnosis.

🔮 Future Improvements

Use Transfer Learning (EfficientNet / ResNet)

Improve dataset size

Deploy as a web application

Add Grad-CAM visualization for tumor detection

👨‍💻 Author

Chiranjit Sahu# Lung-Cancer-Detection-using-CNN
