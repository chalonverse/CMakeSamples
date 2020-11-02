# Comments begin with a #

# This is just an absolute minimal project to add many subdirectories.
# The interesting stuff mostly happens in each subdirectory.

# The minimum required version of CMake
# (in this case we're asking for 3.16 or higher)
cmake_minimum_required(VERSION 3.16)

# Name of this top-level project.
# This doesn't have to correlate to any specific executable name.
# When using a generator like Xcode or Visual Studio, this will be the project file.
project(CMakeSamples)

# This adds subdirectories to look at for this project
add_subdirectory(Ex01)
add_subdirectory(Ex02)
add_subdirectory(Ex03)
add_subdirectory(Ex04)
add_subdirectory(Ex05Lib)
add_subdirectory(Ex05Exe)
add_subdirectory(Ex06)
