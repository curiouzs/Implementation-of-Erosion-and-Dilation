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

```python

# Import the necessary packages
import numpy as np
import cv2
import matplotlib.pyplot as plt
# Load the Image
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
# Create the Text using cv2.putText
cv2.putText(img1,'LOKESH KRISHNAA',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')
# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
# Erode the image
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')

# Dilate the image
img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')


```
## Output:

### Display the input Image
![1](https://user-images.githubusercontent.com/75234646/169662542-c781197d-0cea-442f-bbfe-173fa70289e6.PNG)


### Display the Eroded Image
![2](https://user-images.githubusercontent.com/75234646/169662545-04dc265d-ac29-4e76-8329-432efd50944e.PNG)


### Display the Dilated Image
![3](https://user-images.githubusercontent.com/75234646/169662552-8e8fda7b-52d0-4b6f-a044-3e0c2d6369f1.PNG)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
