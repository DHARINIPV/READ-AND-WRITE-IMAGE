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
### Developed By: Dharini PV
### Register Number: 212222240024
```
i) #To Read,display the image
```
import cv2
image=cv2.imread("flower.jpg",1)
cv2.imshow("21222240024_DhariniPV",image)
cv2.waitKey(0)
cv2.destroyAllwindows()
  

```
ii) #To write the image
```
import cv2
image=cv2.imread("flower.jpg",1)
cv2.imwrite("flower.jpg",image)
cv2.imshow("212222240024_DhariniPV",image)
cv2.waitKey(0)
cv2.destroyAllwindows()

```
iii) #Find the shape of the Image
```
import cv2
picture=cv2.imread("flower.jpeg",1)
print(picture.shape)

```
iv) #To access rows and columns

```
import random
import cv2
image=cv2.imread("flower.jpg",1)
for i in range(100):
    for j in range(image.shape[1]):
        image[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("21222240024_DhariniPV",image)
cv2.waitKey(0)
cv2.destroyAllwindows()

```
v) #To cut and paste portion of image
```
import cv2
img = cv2.imread('butterfly.jpg', 1)
tag = img[20:80:, 20:80]
img[90:150, 90:150] = tag
cv2.imshow('212222240024_DhariniPV', img)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image


![Screenshot from 2023-08-22 21-58-27](https://github.com/DHARINIPV/READ-AND-WRITE-IMAGE/assets/119400845/90ec87a0-b0a1-4448-bd4d-6ca9e723f859)


### ii)Write the image


![Screenshot from 2023-08-22 22-18-26](https://github.com/DHARINIPV/READ-AND-WRITE-IMAGE/assets/119400845/0ef1cea4-e077-428d-98c6-95556685cec4)


### iii)Shape of the Image


![Screenshot from 2023-08-22 22-19-02](https://github.com/DHARINIPV/READ-AND-WRITE-IMAGE/assets/119400845/fbaa7c9e-bfa6-4603-9ca4-db6728fc51a1)


### iv)Access rows and columns


![Screenshot from 2023-08-22 22-21-04](https://github.com/DHARINIPV/READ-AND-WRITE-IMAGE/assets/119400845/1a31ef6e-5b6b-4beb-806c-41990b745daa)


### v)Cut and paste portion of image


![Screenshot from 2023-08-22 22-38-44](https://github.com/DHARINIPV/READ-AND-WRITE-IMAGE/assets/119400845/ed7fcb8f-0b68-4af9-8afb-aa45eadd5a22)


## Result:

Thus the images are read, displayed, and written successfully using the python program.
