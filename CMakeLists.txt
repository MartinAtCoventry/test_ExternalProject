cmake_minimum_required(VERSION 3.9)

project(jascontrol C)

add_library(jascontrol STATIC IMPORTED)
set_target_properties(jascontrol PROPERTIES IMPORTED_LOCATION static_lib/libjascontrol.a)
set_target_properties(jascontrol PROPERTIES INTERFACE_INCLUDE_DIRECTORIES include)

install(TARGETS ${PROJECT_NAME}
        LIBRARY DESTINATION ${PROJECT_SOURCE_DIR}/lib)
