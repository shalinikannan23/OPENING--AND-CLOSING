# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:

- Step1: Import the require libraries.
- Step2: Read the image.
- Step3: Create the structuring element or kernal element
- Step4: Use Opening operation.
- Step5: Use Closing Operation.

 ```
DEVELOPED BY: SHALINI K
REGISTER NUMBER: 212222240095
```

## Program:

- Import the necessary packages
  
  ```PY
  import cv2
  import numpy as np
  ```

- Create the Text using cv2.putText

  ```py
  img1=np.zeros((100,500),dtype="uint8")
  font=cv2.FONT_HERSHEY_PLAIN
  cv2.putText(img1,"SHALINI K 212222240095",(5,60),font,2,(255),5,cv2.LINE_AA)
  cv2.imshow("Original Image",img1)
  cv2.waitKey(0)
  ```
  ![image](https://github.com/shalinikannan23/erosion-dilation/assets/118656529/618cfdc2-afef-4532-b4d6-285c8eb90abf)
  
- Create the structuring element

```PY
kernel=np.ones((5,5),np.uint8)
```

- Use Opening operation.

  ```PY
  imgO=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernal)
  cv2.imshow("Opening Operation",imgO)
  cv2.waitKey(0)
  ```
  ![image](https://github.com/shalinikannan23/erosion-dilation/assets/118656529/60f262f0-4d9a-4844-a8c5-04e97ad4db3a)

- Use Closing Operation

  ```PY
  imgC=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernal)
  cv2.imshow("Closing Operation",imgC)
  cv2.waitKey(0)
  ```
  ![image](https://github.com/shalinikannan23/erosion-dilation/assets/118656529/2079c4e8-faaf-4d28-aaa4-b93940d681ec)



## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
