MNIST Handwritten Digit Recognizer
This project uses a Convolutional Neural Network (CNN) to recognize handwritten digits from the MNIST dataset. The model is trained using TensorFlow/Keras and achieves high accuracy on the test set.

Features
Recognizes digits (0–9) from 28x28 grayscale images
Trained using a simple CNN model
Achieves around 98–99% accuracy
Includes saved model file for reuse
Demo code to test the model with any image

Dataset
The MNIST dataset contains 60,000 training and 10,000 testing handwritten digit images.
Files in this repository
MNIST_Digit_Recognizer.ipynb
mnist_digit_recognizer.h5 (saved CNN model)

How to run the project
Install required libraries:
pip install tensorflow numpy matplotlib
Open the notebook
Run all cells to train or load the model
test predictions on sample images

Model Summary
The model includes convolution layers, pooling layers, and dense layers to classify digits accurately.

Example prediction code
sample = x_test[index].reshape(1, 28, 28, 1)
pred = model.predict(sample)
print("Predicted Digit:", pred.argmax())
