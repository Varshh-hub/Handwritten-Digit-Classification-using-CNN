# Handwritten Digit Classification using CNN

A Deep Learning project that uses a **Convolutional Neural Network (CNN)** to recognize and classify handwritten digits from images.

The project demonstrates the workflow of building, training, evaluating, and saving a CNN-based image classification model using **TensorFlow/Keras**.

The trained model is saved as:

```text
handwritten_digit_cnn.h5
```

## Project Overview

Handwritten digit recognition is a fundamental **Computer Vision and Deep Learning** problem.

In this project, a CNN is trained to learn visual patterns from handwritten digit images and classify them into their corresponding digit classes.

## Objectives

* Understand the fundamentals of Convolutional Neural Networks.
* Perform image preprocessing for deep learning.
* Build a CNN for handwritten digit classification.
* Train the model on handwritten digit images.
* Evaluate the model's classification performance.
* Save the trained model for future inference and deployment.

## Technologies Used

* **Python**
* **TensorFlow**
* **Keras**
* **NumPy**
* **Matplotlib**
* **Convolutional Neural Networks (CNN)**

## Project Workflow

```text
Input Images
     ↓
Image Preprocessing
     ↓
CNN Model
     ↓
Convolution Layers
     ↓
Pooling Layers
     ↓
Flatten
     ↓
Dense Layers
     ↓
Digit Classification
     ↓
Predicted Digit
```

## CNN Architecture

The model follows the typical CNN pipeline:

1. **Convolution Layer**
   Extracts important visual features from the input images.

2. **Pooling Layer**
   Reduces spatial dimensions while retaining important features.

3. **Flatten Layer**
   Converts the extracted feature maps into a one-dimensional vector.

4. **Dense Layers**
   Learns higher-level patterns for classification.

5. **Output Layer**
   Produces the predicted digit class.

## Repository Structure

```text
Handwritten-Digit-Classification-using-CNN/
│
├── CNN1.ipynb
│   └── Complete CNN implementation, training and evaluation
│
├── handwritten_digit_cnn.h5
│   └── Trained CNN model
│
└── README.md
```

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Varshh-hub/Handwritten-Digit-Classification-using-CNN.git
```

### 2. Navigate to the Project

```bash
cd Handwritten-Digit-Classification-using-CNN
```

### 3. Install Dependencies

```bash
pip install tensorflow numpy matplotlib jupyter
```

### 4. Run the Notebook

```bash
jupyter notebook CNN1.ipynb
```

Run the notebook cells sequentially to preprocess the images, build the CNN, train the model, and evaluate its performance.

## Trained Model

The repository includes the trained model:

```text
handwritten_digit_cnn.h5
```

The model can be loaded using TensorFlow/Keras:

```python
from tensorflow.keras.models import load_model

model = load_model("handwritten_digit_cnn.h5")
```

## Prediction

Once the trained model is loaded, an appropriately preprocessed handwritten digit image can be passed to the model to obtain its predicted digit.

Example:

```python
prediction = model.predict(image)

predicted_digit = prediction.argmax(axis=1)[0]

print("Predicted Digit:", predicted_digit)
```

> The input image must be preprocessed to match the format and dimensions expected by the trained model.

## Key Learning Outcomes

Through this project, I gained practical experience with:

* Convolutional Neural Networks
* Image classification
* Image preprocessing
* TensorFlow/Keras model development
* CNN architecture
* Model training and evaluation
* Saving and loading trained deep learning models
* Applying Deep Learning to Computer Vision problems

## Future Improvements

* Add a dedicated prediction script for new handwritten images.
* Build a simple **Flask/Streamlit web application** for real-time digit prediction.
* Add data augmentation to improve model generalization.
* Display confusion matrix and detailed classification metrics.
* Deploy the trained model as a web application.
* Add support for drawing digits directly on a web interface.

## Author

**Varsha A**

AI & ML Graduate | Junior Data Scientist & Machine Learning Engineer | Python | SQL | Excel | Power BI | Prompt Engineer | Front-End Developer
