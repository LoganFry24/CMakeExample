cmake_minimum_required(VERSION 3.0.0)
project(test VERSION 1.0) #nameof the project

#import source files
include_directories(${test_SOURCE_DIR}/src) #the location of the main file
include_directories(${test_SOURCE_DIR}/src/model) # the location of the model files
set(test_SOURCES ${test_SOURCE_DIR}/src/main.c)
#set output binary folder for the exe
include_directories(${test_SOURCE_DIR}/bin)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${test_SOURCE_DIR}/bin)
#create the executable
add_executable(test ${test_SOURCES})

