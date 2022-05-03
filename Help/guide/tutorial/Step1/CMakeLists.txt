cmake_minimum_required(VERSION 3.10)

# set the project name
project(Tutorial VERSION 1.0)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# project version
configure_file("${PROJECT_SOURCE_DIR}/TutorialConfig.h.in" "${PROJECT_SOURCE_DIR}/TutorialConfig.h")
include_directories(${PROJECT_BINARY_BIN})

# add the executable
add_executable(Tutorial tutorial.cxx)