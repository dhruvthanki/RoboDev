# define minimum cmake version required
cmake_minimum_required(VERSION 3.10.2)

# set the project name
project(RoboDev VERSION 1.0)

# specify the C++ standard
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# specify the main source file
set(SOURCE main.cpp)

# add the executable
add_executable(${PROJECT_NAME} ${SOURCE})