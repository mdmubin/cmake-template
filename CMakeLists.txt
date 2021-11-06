cmake_minimum_required(VERSION 3.18)

# project name
project(template VERSION 1.0.0 LANGUAGES CXX)

# c++ standard
set(CMAKE_CXX_STANDARD 20)

# configure src directory
add_subdirectory(src)
# configure test directory
