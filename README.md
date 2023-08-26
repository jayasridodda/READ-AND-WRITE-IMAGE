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
## Program
### Developed By : JAYASRI DODDA
### Register Number : 212222240028 
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('ex3.jpg',1)
cv2.imshow('212222240028_JAYASRI',color_img)
cv2.waitKey(0)  

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('ex3.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212222240028_JAYASRI',color_img)
cv2.waitKey(0) 

```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('ex3.jpg',1)
print(color_img.shape)

```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('exx.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222240028_JAYASRI',color_img)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('exx.jpg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212222240028_JAYASRI',color_image)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image
![Screenshot from 2023-08-24 20-11-21](https://github.com/jayasridodda/READ-AND-WRITE-IMAGE/assets/123259278/961ddbfb-1b0a-4f8f-879b-c334e6d133d2)
### ii)Write the image
![Screenshot from 2023-08-25 20-38-07](https://github.com/jayasridodda/READ-AND-WRITE-IMAGE/assets/123259278/e92244cf-1dbd-490a-b801-f89728e2f02d)

### iii)Shape of the Image
![Screenshot from 2023-08-25 21-34-00](https://github.com/jayasridodda/READ-AND-WRITE-IMAGE/assets/123259278/9c137025-49a1-4b0e-8f85-ac63d0ebef25)

### iv)Access rows and columns
![Screenshot from 2023-08-25 21-36-39](https://github.com/jayasridodda/READ-AND-WRITE-IMAGE/assets/123259278/37e7c1a9-740d-4788-8b29-92803969304c)

### v)Cut and paste portion of image
![Screenshot from 2023-08-25 21-40-38](https://github.com/jayasridodda/READ-AND-WRITE-IMAGE/assets/123259278/bc093113-4247-46b3-8975-05d551d9ad44)



## Result:

Thus the images are read, displayed, and written successfully using the python program.
