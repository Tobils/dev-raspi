# Minimum CMake version required to generate
# our build system
cmake_minimum_required(VERSION 3.0)
SET(CMAKE_C_COMPILER $ENV{HOME}/Documents/develope-tobil/pi/tools/arm-bcm2708/gcc-linaro-arm-linux-gnueabihf-raspbian/bin/arm-linux-gnueabihf-gcc)
SET(CMAKE_CXX_COMPILER $ENV{HOME}/Documents/develope-tobil/pi/tools/arm-bcm2708/gcc-linaro-arm-linux-gnueabihf-raspbian/bin/arm-linux-gnueabihf-g++)
SET(CMAKE_FIND_ROOT_PATH $ENV{HOME}/Documents/develope-tobil/pi/rootfs)

# Name of our Project
project(hello)

# add_executable creates an executable with
# The given name. In our case it is "Hello"
# Source files are given as parameters. In our
# Case we only have one source file Hello.cpp
add_executable(Hello main.cpp)
