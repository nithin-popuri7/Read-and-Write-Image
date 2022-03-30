# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```
### Developed By: P.Siva Naga Nithin
### Register Number: 212221240037
### To Read,display the image

import cv2
color=cv2.imread('th.jpg',1)
cv2.imshow('212221240037',color)
cv2.waitKey(0)

### To write the image

import cv2
color=cv2.imread('th.jpg',1)
cv2.imwrite('th.jpg',color)
cv2.waitKey(0)


### Find the shape of the Image

import cv2
color=cv2.imread('th.jpg',1)
print(color.shape)

### To access rows and columns

import cv2
color=cv2.imread('th.jpg',1)
import random
for i in range (100):
    for j in range(color.shape[1]):
        color[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240037-AccessingRowsAndColumns',color)
cv2.waitKey(0)


### To cut and paste portion of image

import cv2
color=cv2.imread('th.jpg',1)
tag = color[20:80,20:80]
color[90:150,90:150] = tag
cv2.imshow('212221240037-AccessingRowsAndColumns',color)
cv2.waitKey(0)
```
## Output:

### i) Read and display the image

<img width="172" alt="Reading" src="https://user-images.githubusercontent.com/94154780/160879809-b262b96e-19e4-42b2-85e6-0b1a0c185a0c.png">


### ii)Write the image

<img width="175" alt="write" src="https://user-images.githubusercontent.com/94154780/160880178-cf076db7-b4aa-4c7d-b8b5-559c4616834d.png">


### iii)Shape of the Image

<img width="960" alt="shape" src="https://user-images.githubusercontent.com/94154780/160880203-d3815043-1158-4362-b5a5-981797826757.png">


### iv)Access rows and columns
<img width="193" alt="Accessing" src="https://user-images.githubusercontent.com/94154780/160880535-83c8bae4-e8e7-44c1-a654-f9fc72477fa6.png">


### v)Cut and paste portion of image
<img width="194" alt="Accessingrowsandcolumns" src="https://user-images.githubusercontent.com/94154780/160880318-f91bba5b-548b-4585-b3ea-be4102663dbc.png">


## Result:
Thus the images are read, displayed, and written successfully using the python program.


