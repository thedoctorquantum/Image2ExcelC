cmake_minimum_required(VERSION 3.16.3)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project("Image2Excel" VERSION 1.0.0)

add_subdirectory("Image2ExcelC")
add_subdirectory("Image2Editor")