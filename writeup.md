# Writeup: Track 3D-Objects Over Time

Please use this starter template to answer the following questions:

### 1. Write a short recap of the four tracking steps and what you implemented there (filter, track management, association, camera fusion). Which results did you achieve? Which part of the project was most difficult for you to complete, and why?

In this task I implemented Extended Kalman Filter for 3D objects, track management system 
including track score, track state, track initialization and deletion implementation,
association of a new measurements with existing/new tracks and transformation of coordinates for camera sensor.

Intermediate exercises covered all topics, so in general I didn't struggle with implementation.
However it wasn't clear for me how to fill Q matrix for 3D objects(I found some hints in knowledge database).
Also I spend a lot of time fighting with ghost tracks on step 4.
In the end I realized that I forgot to use gating function.

Charts for all steps and tracking movie are available in final_submission folder.

### 2. Do you see any benefits in camera-lidar fusion compared to lidar-only tracking (in theory and in your concrete results)? 

In my results RMSE values are similar for lidar-only tracking system and both sensor tracking system.
In theory using of two sensors should increase accuracy of tracking system in edge cases
like tricky weather conditions, night driving, intersections with low visibility.


### 3. Which challenges will a sensor fusion system face in real-life scenarios? Did you see any of these challenges in the project?

tricky weather conditions(e.g. for), night driving, intersections with low visibility, surfaces with different reflectivity.

I didn't observe(or test this tracking system) with described scenarios.

### 4. Can you think of ways to improve your tracking results in the future?

1. Using multiple cameras/lidars to observe tracks with 360 views.
2. track objects on longer distance

