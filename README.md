# Pizza vs Not-Pizza Classifier
# Overview
This project uses a simple feedforward neural network to classify images as either "pizza" or "not pizza".
The dataset consists of images of pizzas and non-pizzas.it is also provided as a zip file
The neural network model is trained on this dataset using binary cross-entropy loss, and its performance is evaluated on separate training and test sets.

# Dependencies
Google Colab (for accessing Google Drive)
Python
NumPy
PyTorch
Matplotlib
# Code Structure
1. Import Libraries and Mount Google Drive
The code begins by importing necessary libraries and mounting the Google Drive to access the dataset.

2. Data Loader
The getdata function reads images from the specified path. This function assumes all images are of shape 64x64x3.

3. Data Paths
The paths for "pizza" and "not pizza" images are specified.

4. Load and Visualize Data
Images are loaded into tensors. A sample image is displayed using matplotlib.

5. Preprocess Data
The data is split into training and test sets. Images are reshaped and normalized to values between 0 and 1.

6. Create Labels
For supervised learning, labels are created for the images. "Pizza" images are labeled as 1 and "not pizza" images are labeled as 0.

7. Model Architecture
A simple neural network with two hidden layers and ReLU activations is defined. The output layer uses a sigmoid activation to produce a value between 0 and 1.

8. Train Model
The model is trained using binary cross-entropy loss. Gradient descent is applied to update the model's weights. The training loss is printed periodically.

9. Save Model
After training, the model is saved to disk.

10. Test Model
A sample test image is displayed, and the model's prediction for this image is shown. Additionally, the overall accuracy of the model on the training and test data is printed.

Final Notes
This simple neural network provides a basic approach to classifying images. The performance can be improved by increasing the complexity of the model, augmenting the dataset, and fine-tuning hyperparameters.

