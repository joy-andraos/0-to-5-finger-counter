# Project Description
This is a simple project that aims to practice my skills in Artificial Intelligence, namely the Computer Vision field, which derives meaningful information from visual inputs such as images and videos. In this project, running the main python code will open the camera and once the hand is detected, the finger counter will identify which number is displayed by the hand. 
All the codes were taught by Murtaza's Workshop on Youtube.
# How Does It Work ?
2 python codes were written in order to achieve the Finger Counter. 

The first one is a HandTracking module that detects and tracks the hand position in video frames from the web cam. The reason for seperating this module from the actual code is to allow the ease of reusing this code for other similar projects that may require to detect and track the hand instead of rewriting it every time. For this project, the HandTracking module will be used to determine the number of fingers being held up by the hand in the frame.

The second code begins by setting up the camera with the desired height and width. Next, it loads a set of finger images from 0 to 5 from a folder previously prepared, and stores them in a list. For the main loop, it captures frame from the webcam and uses the hand detector previously written to find the positions of the hands in the frame. The coordinates of the specific landmarks on the hand are used to determine which fingers are extended. Finally, the finger count will overlay the corresponding finger image on the frame and diplay the finger count, all in real-time video.

In this project, we set the maximum number of allowed hands to 2. Therefore, the user can count from 0 to 5 by using 2 hands.
# How To Run The Codes ?
1- Open either PyCharm (Python IDE) or Visual Studio Code (which supports Python) depending on your preferences.

2- Download the necessary packages: Mediapipe and OpenCv (use any version between Python 3.7 to 3.10 since the new versions do not support Mediapipe yet). 

3- Write first the HandTracking module, and then the main code.

4- Check for errors and test.

5- Have fun with it and make it better!
# Possible Improvements
Of course this project can be scaled up by making it count to 10 or even more (leading to increasing the maximum number of allowed hands). Stay tuned for future imporvements! 
