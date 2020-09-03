# Smart-Fridge


### First: we check (Height < width) ?
* If the height is bigger we rotate the image by 90 degree, otherwise do nothing.
We do this because our final destiny it to fit the image in height 480 and width 640
With minimum lost data.


### Second: we check ( x ? y) ?
* X - The difference between the original width of the image and the wanted.
Y -  The same difference but of the height.
Here we are looking for the smallest difference because this value we will use for
scaling the image.
The scale value is blocked from above with the value 2, its mean that we never
scale the image more then in 2 times no matter what is the value 
(to prevent lost data).
If the image is bigger then the wanted we scale down by the biggest difference.


### Third: after we scaled the image we are doing padding so the image will fit the 
* Desired Height and width (480,640) .
We pad the image randomly from all the sides because we don’t want to have 
all images to be with the same boxing location (for example we don’t want 
all boxing to be in the down right sight).


### Final result: 
* all the pixels that are out of the yellow frame were created with
 random padding.


![Algorithm schema](Снимок.PNG)


## General info
This project is simple Lorem ipsum dolor generator.
	
## Technologies




* Ipsum version: 2.33
* Ament library version: 999
	
## Setup
To run this project, install it locally using npm:

```
$ cd ../lorem
$ npm install
$ npm start
```


## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Setup](#setup)



