#link the include paths to this folder
include_directories(${test_SOURCE_DIR}/src/model) # the location of the model files
include_directories(${test_SOURCE_DIR}/src/view) # the location of the view files
#set output binary folder for the exe
include_directories(${test_SOURCE_DIR}/bin)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${test_SOURCE_DIR}/bin)
#make executable from the entry file
add_executable(${PROJECT_NAME} main.c)
#link the libraries for the exe
target_link_libraries(${PROJECT_NAME} LINK_PUBLIC view)
target_link_libraries(${PROJECT_NAME} LINK_PUBLIC model)