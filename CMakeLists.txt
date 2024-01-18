cmake_minimum_required (VERSION 2.8)
project (encoding)

#version number
set (encoding_VERSION_MAJOR 1)
set (encoding_VERSION_MINOR 0)

#include the subdirectory containing our libs
add_subdirectory (src)
include_directories(src)
#indicate the entry point for the executable
add_executable (encoding src main.cpp)

# Indicate which libraries to include during the link process.
target_link_libraries (encoding EncodingLib)

install (TARGETS encoding DESTINATION bin)
