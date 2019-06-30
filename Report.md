This report come as part of the Udacity Nanodegree on Self Driving Car Engineering.

### Introduction
  In this project the goal is to use the OpenCV library to perform lane line recognition. We will begin by testing our algorithm on pictures and then directly on video.


### Description


### Reflexion
  Curently, the algorithm is good enough to recognize left and right lanes on verry simple environment. Though, it is still not efficient enough for the optional challenge video given at the end of the `P1.ypnb` Notebook.
  
  I think there at least 3 points on which we could improve the efficience of the algorithm:
  
    - At first, of course we could still try to optimize the variables of the image manipulation (kernel_size, low_threshold, high_threshold, rho, min_line_length, etc). For that, as explain in the Udacity course, we could create a simple interface to modify each value in real time in order to gain time.
    
    - Then, in the algorithm, I choose to separate the lines from the left side to the ones from the right side. To improve that at first, we should maybe try to have a better separation between the lines for the left lane and those for the right lane because if the road turn to fast, the algorithm won't be able to have a good anderstanding of the images. Then we could delete the lines with absurd slopes in comparison to the slope mean of all the lines of the left or right lane.
    - Finally, 
