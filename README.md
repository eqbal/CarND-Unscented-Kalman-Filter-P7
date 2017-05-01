# Unscented Kalman Filter Project


## Introduction

[This Project](https://github.com/udacity/CarND-Unscented-Kalman-Filter-Project) is the seventh project (Project 2 / Term 2) of the Udacity Self-Driving Car Nanodegree program.

The main goal of the project is to apply Unscented Kalman Filter to fuse data from LIDAR and Radar sensors of a self driving car using C++. This is a more advanced and more accurate method than the one used in the previous Extended Kalman Filter project.

The code will make a prediction based on the sensor measurement and then update the expected position. See files in the 'src' folder for the primary C++ files making up this project.

## Dependencies

* cmake >= v3.5
* make >= v4.1
* gcc/g++ >= v5.4

## Structure and Files

  - `scr`: a directory with the project code:
  - `main.cpp`: reads in data, calls a function to run the Kalman filter, calls a function to calculate RMSE
  - `ukf.cpp`:  initializes the filter, calls the predict function, calls the update function
  - `tools.cpp`: a function to calculate RMSE.
  - `data`: a directory with an input file, provided by Udacity
  - `output`: a directory which contains the output for running ukf
  - `playground.ipynb`: a python notebook for experimenting the data and output and generate some graphs.

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./UnscentedKF path/to/input.txt path/to/output.txt`. You can find
   some sample inputs in 'data/'.
    - eg. `./UnscentedKF ../data/obj_pose-laser-radar-synthetic-input.txt`

## Sample Output

```
CarND-Unscented-Kalman-Filter-Project [master●●] % ./build/UnscentedKF data/obj_pose-laser-radar-synthetic-input.txt output/output.txt
RMSE
0.0690774
0.0796665
 0.167352
 0.200159
Done!
```

## Editor Settings

We've purposefully kept editor configuration files out of this repo in order to
keep it as simple and environment agnostic as possible. However, we recommend
using the following settings:

* indent using spaces
* set tab width to 2 spaces (keeps the matrices in source code aligned)

## Code Style

Please stick to [Google's C++ style guide](https://google.github.io/styleguide/cppguide.html) as much as possible.

## Generating Additional Data

This is optional!

If you'd like to generate your own radar and lidar data, see the
[utilities repo](https://github.com/udacity/CarND-Mercedes-SF-Utilities) for
Matlab scripts that can generate additional data.

## Project Instructions and Rubric

This information is only accessible by people who are already enrolled in Term 2
of CarND. If you are enrolled, see [the project page](https://classroom.udacity.com/nanodegrees/nd013/parts/40f38239-66b6-46ec-ae68-03afd8a601c8/modules/0949fca6-b379-42af-a919-ee50aa304e6a/lessons/c3eb3583-17b2-4d83-abf7-d852ae1b9fff/concepts/f437b8b0-f2d8-43b0-9662-72ac4e4029c1)
for instructions and the project rubric.
