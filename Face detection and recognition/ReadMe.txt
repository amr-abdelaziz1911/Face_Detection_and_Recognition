## Face Detection and Recognition Project

# Objective
This project aims to build a face detection and recognition system using deep learning. The system:

- Detects faces in images from a large dataset of celebrity photos.
- Crops detected faces and preprocesses them.
- Uses transfer learning with a deep neural network (InceptionV3) to classify faces.

# Dataset Description
The dataset consists of celebrity images, structured into folders by celebrity name. Images are extracted from a zip file, organized for processing, and stored for use in face detection and recognition tasks.

- Original Dataset: Contains images organized by celebrity name, with each folder representing a class.
- Processed Dataset: Images are cropped to contain only faces, normalized, and resized to fit the model's input requirements.

# Instructions for Running the Code in Jupyter Notebook
1- Notebook 1 - Face Detection and Cropping:

- Reads images from the dataset zip file.
- Detects faces in each image using OpenCV's DNN model.
- Crops detected faces and saves them in a new directory (cropped_faces).
- [Run Notebook 1 in Jupyter Notebook]

2- Notebook 2 - Data Preprocessing and Model Training:

- Loads cropped face images, normalizes, and resizes them.
- Encodes class labels (celebrity names) and performs one-hot encoding.
- Loads a pre-trained InceptionV3 model, with modifications for face classification.
- Trains the model on the processed dataset, using early stopping and regularization to avoid overfitting.
- [Run Notebook 2 in Jupyter Notebook]

3- Notebook 3 - Evaluation and Testing:

- Evaluates the trained model on test images.
- Displays model performance metrics like accuracy and classification report.
- [Run Notebook 3 in Jupyter Notebook]

# Dependencies and Installation Instructions
Install the required dependencies using pip. Here are the main libraries needed:
'pip install numpy opencv-python-headless matplotlib tensorflow scikit-learn'

# Expected Results and Model Performance
- Model Accuracy: The expected accuracy is above 85% on validation data.
- Output: The model outputs the predicted celebrity name for each input image.
- Evaluation Metrics: Accuracy, classification report, and training/validation curves are used to assess model performance.