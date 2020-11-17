cmake_minimum_required(VERSION 3.14)
project(caos_driverJ)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)
include_directories(/opt/java/x64/jdk1.8.0_251/include)
include_directories(/opt/java/x64/jdk1.8.0_251/include/linux)
include_directories(/opt/cima-driver-3.4.0)
add_executable(caos_driverJ
    JNIHelloWorld.cpp
    JNIHelloWorld.h)
