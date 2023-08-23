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
### Developed By:IYYANAR S
### Register Number: 212222240036
i) #To Read,display the image
```
import cv2
img = cv2.imread('mobile phone.jpg', 0)
resized_img = cv2.resize(img, None, fx=0.1, fy=0.1)
cv2.imshow('212222240036', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()
  

```
ii) #To write the image
```
import cv2
img=cv2.imread('mobile phone.jpg',0)
cv2.imwrite('writed_walt.png',img)


```
iii) #Find the shape of the Image
```
import cv2
img=cv2.imread('mobile phone.jpg',0)
print(img.shape)
```
iv) #To access rows and columns

```
import cv2
img = cv2.imread('mobile phone.jpg', 0)
resized_img = cv2.resize(img, None, fx=0.1, fy=0.1)
for i in range(100, 250):
    for j in range(10, 50):
        resized_img[i][j] = 255  # Set the pixel to white
cv2.imshow('212222240036', resized_img)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```
import cv2
img = cv2.imread('mobile phone.jpg', 1)
tag = img[300:400, 300:400]
img[50:150, 50:150] = tag
cv2.imshow('212222240036', img)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

![dippp sc1](https://github.com/Iyyanar22009120/READ-AND-WRITE-IMAGE/assets/118680259/9b069157-4834-4544-8ab0-03835e4fa38c)


### ii)Write the image
![dippp sctrue](https://github.com/Iyyanar22009120/READ-AND-WRITE-IMAGE/assets/118680259/a3e93809-6e63-4b8c-b1bb-4444580e55d7)


### iii)Shape of the Image

![dippp scvalue](https://github.com/Iyyanar22009120/READ-AND-WRITE-IMAGE/assets/118680259/b7ac2f12-2429-456d-8021-0b3f65aac17f)


### iv)Access rows and columns
![dippp sc2](https://github.com/Iyyanar22009120/READ-AND-WRITE-IMAGE/assets/118680259/7b7c9fc1-7922-49b7-8431-e0a8d6027606)


### v)Cut and paste portion of image
![dippp sc3](https://github.com/Iyyanar22009120/READ-AND-WRITE-IMAGE/assets/118680259/3bc17f8e-ea4b-47b1-aa0f-37c9bfe97135)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
