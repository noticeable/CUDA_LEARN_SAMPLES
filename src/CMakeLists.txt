CMAKE_MINIMUM_REQUIRED(VERSION 2.8)
PROJECT(zxy)


find_package(CUDA QUIET REQUIRED)

# Specify binary name and source file to build it from
CUDA_ADD_LIBRARY(zxy matrix.cu matrix.cuh square.cu square.cuh add.cuh add.cu math.cpp math.h)
