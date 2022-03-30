<img width="193" alt="Accessing" src="https://user-images.githubusercontent.com/94154780/160878970-0a38bdb7-a99c-4d85-ad6f-fd96117751ef.png">
<img width="194" alt="Accessingrowsandcolumns" src="https://user-images.githubusercontent.com/94154780/160878982-49222d31-c5d7-4476-ba06-6b0243b1fb42.png">
<img width="172" alt="Reading" src="https://user-images.githubusercontent.com/94154780/160878987-d8d90f0d-9f00-453b-9347-333f21941bda.png">
<img width="960" alt="shape" src="https://user-images.githubusercontent.com/94154780/160878990-de3a826b-0267-44bb-ab92-95a7c8bb2ef7.png">
<img width="175" alt="write" src="https://user-images.githubusercontent.com/94154780/160878996-dd2598b8-ee4d-442c-8c95-af3303157d89.png">
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

![output](<img width="172" alt="Reading" src="https://user-images.githubusercontent.com/94154780/160879338-bc218f22-72f3-4450-b768-15b6fd477ffe.png">
Reading.png)

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


