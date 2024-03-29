# Pokemon Classifier using CNN:
This project implements a Pokémon classifier using Convolutional Neural Networks (CNNs). The model is capable of classifying images into three categories: Bulbasaur, Squirtle, and Charmander.

# Dataset:
The dataset consists of 45 images, with 15 images for each Pokémon category, and 10 images for testing purposes(3 for each pokemona 1 wrong image i.e. human image in this case). Each image has been preprocessed by resizing to 150x150 pixels and normalizing pixel values to fall within the range [0,1].

# Model Architecture:
The CNN model architecture consists of three convolutional layers followed by max-pooling layers for feature extraction. This is then followed by a fully connected layer with ReLU activation, and finally, an output layer with softmax activation for classification into the respective categories. The model is trained using the Adam optimizer and sparse categorical cross-entropy loss.

# Training:
The dataset is split into training and validation sets using an 80-20 ratio. The model is trained for 20 epochs with a batch size of 4. During training, the model achieved an accuracy of approximately 90% on the validation set.

# Testing:
Testing the model involves providing unseen images to the trained model and evaluating its predictions. The model successfully classifies images into Bulbasaur, Squirtle, and Charmander categories with high accuracy. However, it does not have the capability to detect images that do not belong to any of these classes.

# Implement this model in your device:<br>
**1)** Download 'Model.ipynb', 'Data.zip', 'Test.Zip' in your desired location<br>
**2)** Extract 'Data.zip' and 'Test.Zip' in your desired location<br>
**3)** In *'Model.py'*, make changes in the directory accordingly<br>
**4** Run the code from top to bottom

***Note:*** you may need to install the libraries if not installed already:
pip install numpy<br>
pip install opencv-python<br>
pip install scikit-learn<br>
pip install keras<br>

# Result:
The model demonstrates strong performance in classifying Pokémon images with an accuracy of approximately 90% on the test set. It successfully identifies the Pokémon species in all the test images belonging to the Bulbasaur, Squirtle, and Charmander classes. However, it may misclassify out-of-class images. Overall, the model shows high accuracy and effectiveness in distinguishing between different Pokémon characters.
