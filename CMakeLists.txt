cmake_minimum_required(VERSION 3.0.0)
project(minimal_cpp VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# Set 3rd party library directories
set(LIB_DIR "${CMAKE_CURRENT_SOURCE_DIR}/libs")

# Add the application
add_subdirectory("app")