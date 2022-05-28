

# Gesture_Hand_Controller
Our project is a navigation controller based on hand gestures working on CPU. Using your webcam to capture your hand, you can move your mouse, left and right click, scroll and zoom. In general, it has a good response, however it may bug sometimes. Know that this is an alpha version.



## How it works
We used Mediapipe Hand Solutions to get the hand landmarks predictions. Later, we generated a dataset with 1894 samples of different hand gestures and used it to train a SVC model. Putting it together with OpenCV, we read each frame from the camera, predict a possible gesture and invoke a routine to treat it. Each routine reproduce the determined action alongside the PyAutoGUI libray.



To run the hand gesture controller, just execute
```
python gesture_controller.py
```

## Quick Execute By Clone this repository
    
    git clone https://github.com/luizhss/Gesture_Hand_Controller
    


## Packages Used

Here are some documentation links:

* [MediaPipe Hands]( https://google.github.io/mediapipe/solutions/hands) (Hand Detect)

* [OpenCV]( https://docs.opencv.org/master/) (Webcam Control)

* [Pyautogui]( https://pyautogui.readthedocs.io/en/latest/mouse.html) (Mouse and Keyboard Control) 

* [Sklearn]( https://scikit-learn.org/0.21/documentation.html) (C-Support Vector Classification Model) 
