# Install-OpenCV-on-Ubuntu
a shell script to help you install OpenCV on Ubuntu easily

OpenCV version: 2.4.11

OS: Ubuntu 16.04 LTS 

Note:

1. For C/C++ and python library only.

2. Ubuntu 16.04 LTS and OpenCV need about 7.3 GB disk space.

# How to Install
    wget https://raw.githubusercontent.com/johnson18404/Install-OpenCV-on-Ubuntu/master/installopencv.sh
    sh installopencv.sh

# Test
    $ python
    >>> import cv2
    >>> print(cv2.__version__)


# Compile C/C++ OpenCV program
### C
    gcc  -o motempl motempl.c -lm  -ggdb `pkg-config --cflags opencv` `pkg-config --libs opencv`


### C++
It is similiar to .c file, but need to add "-lstdc++" parameter.

    gcc  -o OpenCV_ViolaJones2 OpenCV_ViolaJones2.cpp -lm  -ggdb `pkg-config --cflags opencv` `pkg-config --libs opencv` -lstdc++


# Reference
[https://gist.github.com/dynamicguy/3d1fce8dae65e765f7c4](https://gist.github.com/dynamicguy/3d1fce8dae65e765f7c4)

[http://hanmajor.blogspot.tw/2013/10/linux-ubuntu-opencv.html](http://hanmajor.blogspot.tw/2013/10/linux-ubuntu-opencv.html)
