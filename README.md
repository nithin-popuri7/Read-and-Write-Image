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

```python
# Developed By: P.Siva Naga Nithin
# Register Number: 212221240037
# To Read,display the image

import cv2
color=cv2.imread('th.jpg',1)
cv2.imshow('212221240037',color)
cv2.waitKey(0)


# To write the image

import cv2
color=cv2.imread('th.jpg',1)
cv2.imwrite('th.jpg',color)
cv2.waitKey(0)


# Find the shape of the Image

import cv2
color=cv2.imread('th.jpg',1)
print(color.shape)


# To access rows and columns

import cv2
color=cv2.imread('th.jpg',1)
import random
for i in range (100):
    for j in range(color.shape[1]):
        color[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240037-AccessingRowsAndColumns',color)
cv2.waitKey(0)


# To cut and paste portion of image

import cv2
color=cv2.imread('th.jpg',1)
tag = color[20:80,20:80]
color[90:150,90:150] = tag
cv2.imshow('212221240037-AccessingRowsAndColumns',color)
cv2.waitKey(0)

```
## Output:

### i) Read and display the image

<br>
![Output](Reading.jpg)
<br>

### ii)Write the image

<br>
<br>

### iii)Shape of the Image

<br>
<br>

### iv)Access rows and columns
<br>
<br>

### v)Cut and paste portion of image
<br>
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


