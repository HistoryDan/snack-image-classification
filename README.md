# snack-image-classification🍪
## Classifying snack images for the visually impaired 
This repository conatins codes and descriptions of the snack image classification project. Below are the frameworks used for the project. 

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
This script utilizes Selenium, a web automation tool, **to crawl and download images from Google Images** based on a list of popular snack names.
Two essential functions are defined:
  1. createDirectory: This function attempts to create a specified directory and prints an error message if the creation fails.
  2. crawlingImg: This function performs the actual crawling of images from Google Images based on the provided search query ₩name₩. It uses a Chrome webdriver to automate the process, scrolling dynamically to load additional images.
