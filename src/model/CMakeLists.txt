#create library from the folder
add_library(model model.c)
#make the folder public
target_include_directories(model PUBLIC "$CMAKE_CURRENT_SOURCE_DIR")