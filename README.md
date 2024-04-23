# OPENING-AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages
### Step2:
Create the Text using cv2.putText
### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by: PRAVEEN S
Register Number:212222240078
```
### Display the input Image
```py
import cv2
import numpy as np

img=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'PRAVEEN S',(5,70), font,2,(255),5,cv2.LINE_AA)
cv2.imshow('Sample', img)
cv2.waitKey(0)
```
### Create the structured element
```py
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```py
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```py
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image

![Screenshot 2024-04-23 110255](https://github.com/Praveen0500/OPENING--AND-CLOSING/assets/120218611/6b2a2bac-06e0-4dfe-8d03-9d8935664695)


### Display the result of Opening

![Screenshot 2024-04-23 110316](https://github.com/Praveen0500/OPENING--AND-CLOSING/assets/120218611/0c893a18-2ccc-46fe-8d6e-f050e985ed88)


### Display the result of Closing

![Screenshot 2024-04-23 110331](https://github.com/Praveen0500/OPENING--AND-CLOSING/assets/120218611/a55d7c7d-7bda-4877-85bd-bbd9649b8424)


## Result

### Thus the Opening and Closing operation is used in the image using python and OpenCV.
