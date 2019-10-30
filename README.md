# opencv-tesseract-tutorial  

This is a relatively simple, optical character recognition script. It was built
mostly following the tutorial at [pyimagesearch.com](https://www.pyimagesearch.com/2018/09/17/opencv-ocr-and-text-recognition-with-tesseract/).  

## Installation and Set Up  
Below are the instructions for installing this application.  
*These instructions are valid as of 2019.10.03*

### Environment Set Up  
1. Install python.  
   1. Follow the instructions for python installation at [this link](https://www.python.org/downloads/).  
2. Install OpenCV 4 and Tesseract.  
   1. Follow the instructions for your operating system at [this link](https://www.pyimagesearch.com/2018/09/17/opencv-ocr-and-text-recognition-with-tesseract/).  
3. Clone this repository to your local environment.  
   1. Fork this Github repo.  
      1. In a web browser, visit https://github.com/NFabrizio/opencv-tesseract-tutorial  
      2. Click the Fork button in the upper right corner of the screen  
      3. In the "Where should we fork this repository?" pop up, select your username.
    Github should create a fork of the repo in your account  
   2. Clone your fork of the opencv-tesseract-tutorial repo.  
      1. In the terminal on your local environment, navigate to the directory where
         you want to clone the opencv-tesseract-tutorial repo  
         `cd ~/path/to/your/directory`  
      2. In the terminal, run:  
         `git clone [clone-url-for-your-fork]`  
         The URL should be in the format git@github.com:YourUsername/opencv-tesseract-tutorial.git  
4. Run the script from your local machine.  
   1. Change into the directory where you cloned the repo.  
     `cd ~/path/to/your/directory/opencv-tesseract-tutorial`  
   2. Run the script and pass in the required arguments.  
     `python text_recognition.py --east frozen_east_text_detection.pb --image images/sign-security-camera.jpg`  
     You can provide the name of any image in the image option as long as you update the path to that image.  

## Script Use  
Once you run the script, passing it the path to an image, a separate Python window
should open displaying the image with a red box around any text found within
the image. The text in the image should also be displayed in red next to the red
box. The text should also be displayed on the command line in the terminal from
which the script was initiated.  

Pressing any key while viewing the image in the Python window should move to the
next text area found in the image. Once the script is no longer able to find any
text areas in the image, the Python window will close and the script will exit.  
