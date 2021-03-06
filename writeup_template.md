# **Finding Lane Lines on the Road** 

## Writeup Template

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[image1]: ./test_images/processed-whiteCarLaneSwitch.jpg "WhiteCarLane"
[image]: ./Test.png "Tested all step"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. 
First, I made a color selection (yellow and white filters), then I converted the images to grayscale, as a third step I realised de region masking, then I executed the Canny edge detection and finally I aplied the Hough transform. 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by Finding slopes of all lines, Running linear regression to find best fit line for right and left lane lines and Drawing the right and left lines on image

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image]


### 2. Identify potential shortcomings with your current pipeline

I think that the speed could be a potential shortcoming would be what would happen. 


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to work speedly with data image, reducing the region of application of the stages. 

Another potential improvement could be to figure out more accuracy parameter involving Threshold, pixel to identify a line...
