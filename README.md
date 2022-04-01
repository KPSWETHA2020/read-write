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
### Developed By:
Swetha.k.p
### Register Number: 
212220230053
i) #To Read,display the image
```
  import cv2
  image_1=cv2.imread("rose.jpg")
cv2.imshow("rose.jpg",image_1)
cv2.waitKey(0)
```
ii) #To write the image
```
cv2.imwrite("rose1.jpg",image_1)
```
iii) #Find the shape of the Image
```
print(image_1.shape)
```
iv) #To access rows and columns

```
for i in range(70,90):
    for j in range(110,170):
        image_1[i][j]=[0,0,0]
```
v) #To cut and paste portion of image
```
image_1[50:70,110:175]=image_1[70:90,90:115]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

![image](https://user-images.githubusercontent.com/75235209/161278636-488cde09-e79f-4b2d-9637-840f4c116802.png)



### ii)Write the image

![image](https://user-images.githubusercontent.com/75235209/161279533-9a36056d-d661-4183-9689-c0ed105f55b3.png)


### iii)Shape of the Image

![image](https://user-images.githubusercontent.com/75235209/161279732-d5d4e363-2121-4e18-96a1-3e93fba51f0a.png)


### iv)Access rows and columns
![image](https://user-images.githubusercontent.com/75235209/161279981-fb8da9e5-1a4b-49cc-80f0-fd711d67b203.png)


### v)Cut and paste portion of image
![image](https://user-images.githubusercontent.com/75235209/161280049-02a2e879-f724-4dea-afba-3067802e6530.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.
