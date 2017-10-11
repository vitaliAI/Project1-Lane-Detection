# **Finding Lane Lines on the Road** 

## Writeup Template

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

### Pipeline:

Step 1: Grayscale

Step 2: Gaussian Blur Filter

Step 3: Canny Edge Detection

Step 4: Set Region of Interest

Step 5: Hough Transformation

•	Draw lines

•	Use x1,y1,x2,y2 Data points

•	To filter out lines with low slope classify lines or data points into:

•	Left line, Right line

•	Apply extrapolation to find new x,y values to draw lines on the canvas

Step 6: Apply “weighted_img” function to draw lines on the image.



![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline

I could think of applying more Filters to reduce errors, or errosion filter to stregthen withe lane lines


### How to improve the lane lines detection Software?

Knowing exactly where the camera is positioned. One option could be to draw helper lines. For example, one middle line from 

the driver perspective and other two border lines (left and right from the car). When detecting lane lines, you would need to 

perform:

1. Distance measurement to compute the distance of the detected lane lines to the border line.

2. Have a threshold value for the distance to filter out lines which are too far away.



### 3. Suggest possible improvements to your pipeline

Parameter Tuning 

Drawing, stabilizing the the lane lines, by taking average values, or taking average slope


### Conclusion:

First, it was my first project of this kind. It was very interesting to perform different image processing techniques to find 

the edges and hence detect lane lines on the road.

I think using region of interest to detect lane lines, is surely one possible way to do it. But is has some disadvantages. It 

needs to be specifically defined to the camera position. Settings need always to be performed manually to improve correctness 

of the lane detection system.

In summary, I got myself familiar with OpenCV library. Understanding how to convert and RGB image to grayscale. Applying 

Gaussian blur filter to remove noise from the image. Applying Canny edge algorithm to detect high gradient changes in the 

image and therefore the edges. Also doing some linear algebra, applying extrapolation to find new set of points based on the 

lines which were extracted through Hough transformation.
