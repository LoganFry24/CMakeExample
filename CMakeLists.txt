cmake_minimum_required(VERSION 3.0.0)
project(test VERSION 1.0) #name of the project

#import source files
#include_directories(${test_SOURCE_DIR}/src) #the location of the main file
#include_directories(${test_SOURCE_DIR}/src/model) # the location of the model files
#include_directories(${test_SOURCE_DIR}/src/view) # the location of the view files
#set(test_SOURCES ${test_SOURCE_DIR}/src)
add_subdirectory(src/model)
add_subdirectory(src/view)
add_subdirectory(src) #entry point
#create the executable
#add_executable(test ${test_SOURCES})

