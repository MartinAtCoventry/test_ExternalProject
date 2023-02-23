cmake_minimum_required(VERSION 3.9)

project(jaslib C)

add_library(jaslib STATIC IMPORTED)
set_target_properties(jaslib PROPERTIES IMPORTED_LOCATION static_lib/libjascontrol.a)
set_target_properties(jaslib PROPERTIES INTERFACE_INCLUDE_DIRECTORIES include)
