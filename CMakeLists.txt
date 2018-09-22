cmake_minimum_required(VERSION 3.8)
project(cspeak_framework)

set(CMAKE_CXX_STANDARD 11)

include(CheckIncludeFile)
include(CheckIncludeFileCXX)
include(CheckIncludeFiles)
include(ExternalProject)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

find_library(ssh REQUIRED)
include_directories(${ssh_INCLUDE_DIR})

set(SOURCE_FILES src/cspeak.cpp include/cspeak.h)
add_library(cspeak_framework SHARED ${SOURCE_FILES})

target_link_libraries(cspeak_framework ssh)

add_subdirectory(examples)