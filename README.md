# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>


### Step2:
<br>

### Step3:
<br>

### Step4:
<br>

### Step5:
<br>

 
## Program:

``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt


# Create the Text using cv2.putText
img=np.zeros((100,200), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'Gowri M',(5,70),font,2,(255),5,cv2.LINE_AA)


# Create the structuring element



# Erode the image




# Dilate the image





```
## Output:

### Display the input Image
![Screenshot (186)](https://user-images.githubusercontent.com/75234946/169677580-f0bc23c8-2d36-4ffd-afdd-115b018ece03.png)

<br>
<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image
![Screenshot (189)](https://user-images.githubusercontent.com/75234946/169677668-821e095d-fad6-4150-b442-db1a540de93f.png)

<br>
<br>
<br>
<br>
<br>
<br>

### Display the Dilated Image
![Screenshot (186)](https://user-images.githubusercontent.com/75234946/169677610-4d9922cf-0a05-44d5-a3f7-0bfc923afb44.png)

<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
