# CUDA-at-Scale-Independent-Project
## NPP Grayscale Converter
This project was created by KISHORE.S

It aims to create a simple converter that transforms an input image (Emerald_Lakes_New_Zealang.jpg) to grayscale (greyscale_output.ipg) using NVIDIA Performance Primitives (NPP) instead of manually coding GPU kernels.

## Requirements
  CUDA Toolkit (tested with CUDA 12+)
  NPP (comes with CUDA)
  C++17 or higher compiler (g++ / clang++)
  CMake or Make for building (Makefile provided)

## How it works
  The program loads an RGBA PNG image (Emerald_Lakes_New_Zealand.jpg) into host memory.
  The image is copied to device memory.
  The NPP function nppiBGRAToGray_8u_C4C1R converts the image to grayscale.
  The grayscale image is copied back to host memory.
  The result is saved as greyscale_output.jpg.
  
## Usage
Place your input image as Emerald_Lakes_New_Zealand.jpg in the same folder as the executable.

## Build the project using the provided Makefile:
```
make
```
Note: the output image is uploaded as a demonstration that the code runs
