# LittleSLAM

## About LittleSLAM

LittleSLAM is a program for learning SLAM. Enter a file containing 2D laser scanner data (scan) and odometry data, The trajectory of the robot position and the 2D point cloud map are output on gnuplot.

LittleSLAM is a combination of alignment based on scan matching, sensor fusion of laser scanner and odometry, It consists of elemental technologies such as loop closure based on graph-based SLAM.

LittleSLAM is a program created as a teaching material for reference books [1]. A simple algorithm is used in favor of clarity. Therefore, the performance is lower than that of a full-spec SLAM program. The content is easy to understand.

## Execution environment

LittleSLAM is written in the programming language C++. The execution environment that has been confirmed to work is as follows. Both are 64-bit versions.

| OS | C++ |
|:--:|:---:|
| Windows 7 | Visual C++ 2013 (Visual Studio Community 2013)|
| Windows 10 | Visual C++ 2015 (Visual Studio Community 2015)|
| Linux Ubuntu 14.04 LTS | gcc 4.8.4|
| Linux Ubuntu 16.04 LTS | gcc 5.4.0|

We have not tested it on a 32-bit OS, so please try it yourself if you need it.

## Required Software
The following software is required to run LittleSLAM.

| software | content | version |
|:--------:|:-------:|:-------:|
| Boost | C++ Generic Library | 1.58.0|
| Eigen3 | Linear Algebra Library | 3.2.4|
| gnuplot | Graph drawing tools | 5.0|
| CMake | Build Assistance Tools | 3.2.2|
| p2o | Graph-based SLAM Solver | beta|

The version is the one used in the development of LittleSLAM, not a definite condition. Higher versions usually work. It may work with earlier versions.

## use
[Click here](doc/install-win.md) for how to use it on Windows

[Here's](doc/install-linux.md) how to use it on Linux

## Dataset
Six data files are available for experiments. The list is shown in the table below. You can [download it here](https://furo.org/software/little_slam/dataset.zip).

| File Name           | content |
|:--------------------|:--------|
| corridor.lsc        | Corridor (single loop)|
| hall.lsc            | Hall (single loop)|
| corridor-theone.lsc | Under the corridor (degraded)|
| hall-the-one.lsc    | Hall (degenerate)|
| corridor-loops.lsc  | Corridor (multiple loops)|
| hall-loops.lsc      | Hall (multi-loop)|

## customization
LittleSLAM is a learning program that has undergone several improvements from its basic form. It can be customized to complete.
For more information, please [see here](doc/customize.md).

## Reference Books
The following books are manuals on SLAM. In addition to a general explanation of SLAM, As a specific example, LittleSLAM is used as a teaching material and its source code is explained in detail.

[1] Masahiro Tomono, "Introduction to SLAM -- Self-Localization and Map Construction Technology for Robots", Ohmsha, 2018

## license
- LittleSLAM is based on the MPL-2.0 license.
