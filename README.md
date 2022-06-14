# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.

### Step2:
Create the text image using cv2.putText.

### Step3:
Then create the structuring image for dilation/erosion.

### Step4:
Apply erosion and dilation using cv2.erode and cv2.dilate.

### Step5:
Plot the images using plt.imshow.

 
## Program:
```
Developed by : Balaji N
Registeration Number:212220230006
```

``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
text_image = np.zeros((100,440),dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX = 3
cv2.putText(text_image," Gowri",(5,70),font,2,(255),5,cv2.LINE_AA)
plt.title("Original Image")
plt.imshow(text_image,'magma')
plt.axis('off')

# Create the structuring element
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
image_erode = cv2.erode(text_image,kernel)
plt.title("Eroded Image")
plt.imshow(image_erode,'magma')
plt.axis('off')

# Dilate the image
image_dilate = cv2.dilate(text_image,kernel)
plt.title("Dilated Image")
plt.imshow(image_dilate,'magma')
plt.axis('off')



```
## Output:

### Display the input Image
![Screenshot_666](https://user-images.githubusercontent.com/75235455/169960805-ea40f555-969b-4183-9752-c43b502a7de0.png)


### Display the Eroded Image
![Screenshot_664](https://user-images.githubusercontent.com/75235455/169960860-28e090d9-0b9e-48f9-b8cf-b533c1cd4a64.png)


### Display the Dilated Image
![Screenshot_665](https://user-images.githubusercontent.com/75235455/169960884-6b972f2a-d1dc-4744-a5cc-c230e81d99f2.png)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
