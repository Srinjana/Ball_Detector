# Track the trajectory of A ball
### This project tracks the trajectory of a Ball using OpenCV. A part of my Pyimagesearch 17 days into the deep learning program, this code tracks the trajectory of the ball.
---
## How does this work?
In this project we performed ball tracking with OpenCV. The Python script was able to do the following
* Detect the presence of the colored ball.
* Track and draw the position of the ball as it moved around the screen.

The system was quite robust and able to track the ball even if it was partially occluded from view by the hand holding it. It is seen that the program runs more optimally, if there isn't any other object similar to the color of the ball in framde.

The script was also able to operate at an extremely high frame rate (> 32 FPS), indicating that color based tracking methods are very much suitable for real-time detection and tracking.
The script works for both:
1) A prerecorded video file.
2) Webcam Footage 

and both with equal precision.

## Run the code using this command:


```
  python ball_detector.py --video ball_me.mp4
  python ball_detector.py --video ball_adrian.mp4
  python ball_detector.py           //for webcam footage
```

## Necessary Packages:

```
  from collections import deque
  from imutils.video import VideoStream
  import numpy as np
  import argparse
  import cv2
  import imutils
  import time
```

# Screengrab
![Pyimagesearch Gif](https://pyimagesearch.com/wp-content/uploads/2015/09/ball-tracking-tails-comparison.jpg)

### Find the Blog with the in-depth Tutorial [here] (https://www.pyimagesearch.com/2015/09/14/ball-tracking-with-opencv/)
