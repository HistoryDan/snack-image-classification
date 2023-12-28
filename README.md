# snack-image-classification🍪
## Classifying snack images via CNN & ResNet for the visually impaired 
This repository conatins codes and descriptions of the snack image classification project. Note that all code has been executed in the Google Colab environment. Below are the frameworks used for the project. 

<div align="left">
   <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=Python&logoColor=white"/>
   <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=Jupyter&logoColor=white"/>
   <img src="https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=Selenium&logoColor=white"/>
   <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=OpenCV&logoColor=white"/>
   <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=NumPy&logoColor=white"/>
   <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white"/>
   <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=TensorFlow&logoColor=white"/>
   <img src="https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=Keras&logoColor=white"/>
</div>

## 📄Code Description
### snack-image-crawling.ipynb
This script utilizes Selenium, a web automation tool, to **crawl and download images from Google Images** based on a list of popular snack names.
Two essential functions are defined:
  1. **createDirectory**: This function attempts to create a specified directory and prints an error message if the creation fails.
  2. **crawlingImg**: This function performs the actual crawling of images from Google Images based on the provided search query `name`. It uses a Chrome webdriver to automate the process, scrolling dynamically to load additional images.

-----

### data-preprocessing.ipynb
This script focuses on **preprocessing and augmenting** image data for a snack classification task. The script uses various libraries, including OpenCV, PIL (Pillow), and Matplotlib, to perform tasks such as file sorting, renaming, image visualization, train-test splitting, and data augmentation.
   1. **Sorting files**: organizes image files into folders based on snack types
   2. **Image example visualization**: Randomly selected images are visualized to provide an overview of the dataset.
   3. **Train test split**: The dataset is split into training and testing sets.
   4. **Data augmentation**: Images in the training set undergo various augmentations, including left-right inversion, rotation, top-bottom inversion, black-and-white conversion, and brightness adjustment. These augmented images are then saved to enrich the training dataset.

This script serves as a comprehensive preprocessing and augmentation pipeline, ensuring the dataset is well-organized, balanced, and ready for training deep learning models.

-----

### classification-via-dnn.ipynb
This script demonstrates a snack classification task using an DNN with the Keras library.
   1. **Modeling and training**: The script defines and trains an DNN for classifying snack images. It uses a dataset organized into categories, loads and preprocesses the images, defines the model architecture, compiles the model, and trains it. The training process is monitored, and a checkpoint is set to save the best model.
   2. **Training history**: The training history, including accuracy and loss, is visualized using Matplotlib. Two graphs are displayed: one for loss and another for accuracy over epochs. These graphs provide insights into the model's learning progress.

-----

### classification-via-cnn-resnet.ipynb
This script demonstrates the classification of snack images using Convolutional Neural Network (CNN) and ResNet architectures with the Keras library.
   1. **CNN modeling and training**: The script loads and preprocesses snack images, defines a CNN architecture, compiles the model, and trains it. The training process is monitored, and a checkpoint is set to save the best model.
   2. **CNN training history**: The training history, including accuracy and loss, is visualized using Matplotlib. Two graphs are displayed: one for loss and another for accuracy over epochs.
   3. **Resnet moeling and training**: The script defines ResNet blocks, a ResNet model, compiles it, and trains it. The training process is monitored, and a checkpoint is set to save the best model.
   4. **Resnet training history**: The training history, including accuracy and loss, is visualized using Matplotlib. Two graphs are displayed: one for loss and another for accuracy over epochs.








