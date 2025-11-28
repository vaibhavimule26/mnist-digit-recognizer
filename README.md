MNIST Handwritten Digit Recognizer
This project builds a Convolutional Neural Network (CNN) model to recognize handwritten digits using the MNIST dataset. The model is trained on 60,000 images and tested on 10,000 images, achieving high accuracy. It can correctly classify digits from 0 to 9 based on image input.

Project Features
• Uses MNIST dataset for training and testing
• CNN architecture with Conv2D, MaxPooling2D, Flatten, and Dense layers
• Achieves close to 99 percent accuracy
• Includes visualization of predictions
• Saved trained model file for reuse and deployment

Tech Stack
• Python
• TensorFlow / Keras
• NumPy
• Matplotlib
• Google Colab

Project Structure
mnist-digit-recognizer/
│── MNIST_Digit_Recognizer.ipynb
│── mnist_digit_recognizer.h5
│── README.md

How the Model Works
The MNIST dataset is loaded and normalized
Data is reshaped for the CNN input layer
A CNN is created and trained for 5 epochs
Model performance is evaluated using test images
The trained model is saved in .h5 format
Predictions are visualized using sample test digits

Sample Prediction Code
Use this code inside your notebook to test any digit:

sample = X_test[index].reshape(1,28,28,1)
pred = model.predict(sample)
print("Predicted Digit:", pred.argmax())

Model Accuracy
Test Accuracy: approximately 98 to 99 percent

Author
Vaibhavi Mule
AI Intern at Codec Technologies
