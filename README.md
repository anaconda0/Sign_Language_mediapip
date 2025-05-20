🧠 Sign Language Recognition using CNN
This project implements a Convolutional Neural Network (CNN) for recognizing American Sign Language (ASL) gestures from images. It's an important step toward improving communication for individuals who are deaf or hard of hearing by using hand gesture classification.

🗂️ Dataset
The dataset is similar to MNIST in structure:

Each image is a 28x28 grayscale representation of a hand gesture.

Labels are integers from 0–25, representing A–Z (excluding J and Z due to dynamic gestures).

Training set: 27,455 samples

Test set: 7,172 samples

Preprocessing steps:

Normalized pixel values (0 to 1 range)

One-hot encoding of labels using LabelBinarizer

Data augmentation using Keras ImageDataGenerator for better generalization.

🧰 Model Architecture
The CNN used in this project includes:

Three convolutional layers with ReLU activations and MaxPooling

One dense layer with 512 units

Output layer with 24 nodes and softmax activation

The model is compiled using:

Loss function: categorical_crossentropy

Optimizer: adam

Metrics: accuracy

🎯 Objective
To build a reliable gesture recognition system for American Sign Language that can help bridge communication gaps between deaf/dumb individuals and others.

🧪 How to Use
Once the notebook is loaded:

Load the dataset (CSV files).

Preprocess and augment the images.

Train the CNN model.

Evaluate its performance on the test dataset.

(Optional) Integrate webcam-based live predictions.

📚 Requirements
You'll need the following Python libraries:

TensorFlow / Keras

Pandas

NumPy

Matplotlib

Scikit-learn

You can install them via:


pip install tensorflow pandas numpy matplotlib scikit-learn
