# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.
 
## Program:
```
/*
Developed by   : Balaji N
Register Number: 212220230006
*/
```
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((300,700),dtype='uint8')
font=cv2.FONT_ITALIC=3
img2=cv2.putText(img1,"Dineshkumar",(10,150),font,3,(255),5,cv2.LINE_AA)
cv2.imshow("Original",img2)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Create the structuring element
kernel=np.ones((5,5),np.uint8)
kernal1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
erode=cv2.erode(img2,kernel)
cv2.imshow("Erosion1",erode)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Dilate the image
dilute=cv2.dilate(img2,kernel1)
cv2.imshow("Dilution",dilute)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### Display the input Image

![Screenshot (218)](https://user-images.githubusercontent.com/75234946/175252198-173b8908-a5d1-4eea-9d13-ead349c43c55.png)



### <br><br>Display the Eroded Image
![Screenshot (222)](https://user-images.githubusercontent.com/75234946/175252302-641e0499-cc84-4e5f-baba-fceb5c2a4805.png)



### Display the Dilated Image
![Screenshot (223)](https://user-images.githubusercontent.com/75234946/175252378-bab5924a-6143-4aaa-8a53-390cbc01140e.png)


## <br><br><br><br>Result
Thus the generated text image is eroded and dilated using python and OpenCV.
