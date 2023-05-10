# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
## Step 1:
Load the necessary packages requiured for the implemtation of erosion and dilation on an image.

## Step 2:
Create the text image for the implemtation of erosion and dilation using cv2.putText function.

## Step 3:
Create the structuring image for the implemtation of erosion and dilation on the text image.

## Step 4:
Apply the erosion and dilation to the text image using cv2.erode and cv2.dilate.

## Step 5:
Display the images of the erosion and dilation applied using the plt.imshow.

## Step 6:
End the program.

 
## Program:
## Developed by :R BRINDHA
## Register Number: 21222223023
# Program to implement Erosion and Dilation using Python and OpenCV.

# Import the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

# Create the Text using cv2.putText
```
text_image = np.zeros((100,300),dtype = 'uint8')
font = cv2.FONT_HERSHEY_SCRIPT_COMPLEX = 7
cv2.putText(text_image,"Brin",(7,70),font,2,(275),5,cv2.LINE_AA)
plt.title("Original Text Image")
plt.imshow(text_image,'magma')
plt.axis('off')
```
# Create the structuring element
```
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
```
# Erode the image
```
image_erode = cv2.erode(text_image,kernel)
plt.title("Eroded Text Image")
plt.imshow(image_erode,'magma')
plt.axis('off')
```

# Dilate the image
```
image_dilate = cv2.dilate(text_image,kernel)
plt.title("Dilated Text Image")
plt.imshow(image_dilate,'magma')
plt.axis('off')
```
## Output:
### Display the input text Image:
![Screenshot 2023-05-10 135045](https://github.com/Brindha77/Implementation-of-Erosion-and-Dilation/assets/118889143/c258d9ae-1131-44d3-b987-f37d8ffc64bf)

### Display the Eroded Image
![Screenshot 2023-05-10 135054](https://github.com/Brindha77/Implementation-of-Erosion-and-Dilation/assets/118889143/2d9361cc-ebe1-4579-b876-85d42dec85b7)

### Display the Dilated Image
![Screenshot 2023-05-10 135100](https://github.com/Brindha77/Implementation-of-Erosion-and-Dilation/assets/118889143/c6d02199-58e8-4374-ac6e-f94352680ccd)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
