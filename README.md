# EX-10
# OPENING AND CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
- Step1: Import the necessary packages
- Step2: Give the input text using cv2.putText()
- Step3: Perform opening operation and display the result
- Step4: Similarly, perform closing operation and display the result
- 
## Program:
### NAME: DEEPAK RAJ S
### REG.No:212222240023

# Import the necessary packages
```
import numpy as np
import cv2
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```
image = np.zeros((300, 600, 3), dtype="uint8")
text = "DEEPAK RAJ S"
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, text, (50, 150), font, 2, (255, 255, 255), 3)

```
# Create the structuring element
```
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
plt.imshow(image_rgb)
plt.title("Original Image")
plt.axis("off")
```
# Use Opening operation
```
opening_image = cv2.morphologyEx(image, cv2.MORPH_OPEN, kernel)
plt.imshow(opening_image_rgb)
plt.title("Opening Operation")
plt.axis("off")
```
# Use Closing Operation
```
closing_image = cv2.morphologyEx(image, cv2.MORPH_CLOSE, kernel)
plt.imshow(closing_image_rgb)
plt.title("Closing Operation")
plt.axis("off")
```
## Output:
### Display the input Image
![image](https://github.com/user-attachments/assets/19b39ae0-5f61-49ac-bd00-3d45594e9044)

### Display the result of Opening
![image](https://github.com/user-attachments/assets/b51ca3a6-f3ad-4714-8fb3-04cc86859b0f)


### Display the result of Closing
 ![image](https://github.com/user-attachments/assets/3b0c5b3c-ed46-42f3-ad84-75b9f9b8d833)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
