cmake_minimum_required(VERSION 3.14)
project(caos_driverJ)

include_directories(/opt/java/x64/jdk1.8.0_251/include)
include_directories(/opt/java/x64/jdk1.8.0_251/include/linux)
link_directories(/opt/java/x64/jdk1.8.0_251/include)
link_directories(/opt/java/x64/jdk1.8.0_251/include/linux)

add_library(CHDriver SHARED IMPORTED)
set_target_properties(CHDriver PROPERTIES IMPORTED_LOCATION "/opt/Cima DriverC 3.4.0/Release arm-linux/libCHDriver.so")

set(CMAKE_CXX_STANDARD 14)

add_library(caos_driverJ SHARED JNIHelloWorld.cpp JNIHelloWorld.h)