# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by: BALACHANDRAN S
Register Number: 212222100008
```
### Display the input Image
```python
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'Bala', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
### Create ths structured element
```python
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```python
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```python
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image
![Screenshot 2024-05-08 011430](https://github.com/Balachandran143/OPENING--AND-CLOSING/assets/118886489/36663bb1-c834-4318-8057-bc8cb878a22a)


### Display the result of Opening
![Screenshot 2024-05-08 011512](https://github.com/Balachandran143/OPENING--AND-CLOSING/assets/118886489/ce83d7cb-a60d-44b9-9bc5-90e5480211d0)

### Display the result of Closing
![Screenshot 2024-05-08 011533](https://github.com/Balachandran143/OPENING--AND-CLOSING/assets/118886489/23a417b2-8b04-45ab-9bba-c5fb5e5cfe8a)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
