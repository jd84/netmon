cmake_minimum_required(VERSION 3.10)
project(netmon)

option(BUILD_EXAMPLE "Enable building example" OFF)

add_library(netmon STATIC src/network.cxx src/network.hxx)

if(BUILD_EXAMPLE)
    add_subdirectory(example)
endif()

install(TARGETS netmon DESTINATION .)