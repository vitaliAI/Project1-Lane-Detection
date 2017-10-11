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


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
