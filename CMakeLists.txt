cmake_minimum_required(VERSION 3.9)

project(jasdrone C)

add_library(jasdrone STATIC IMPORTED)
set_target_properties(jasdrone PROPERTIES IMPORTED_LOCATION static_lib/libjascontrol.a)
set_target_properties(jasdrone PROPERTIES INTERFACE_INCLUDE_DIRECTORIES include)
