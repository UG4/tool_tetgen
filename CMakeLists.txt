# Set  the minimum  required version  of cmake  for a  project.
cmake_minimum_required(VERSION 2.8.12)

# Add an executable to the project using the specified source files.
add_executable(tetgen tetgen.cxx predicates.cxx)

#Add a library to the project using the specified source files. 
# In Linux/Unix, it will creates the libtet.a
add_library(tet STATIC tetgen.cxx predicates.cxx)
target_include_directories(tet PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
set_target_properties(tet PROPERTIES COMPILE_DEFINITIONS TETLIBRARY)

if (UNIX)
    set_target_properties(tet PROPERTIES COMPILE_FLAGS -fPIC)
endif ()

option(LINK_TETGEN "Link GPL licensed tetgen to ug4. Only for development builds." OFF)

message(STATUS "Info: Additional options for the tetgen tool:")
message(STATUS "Info:   LINK_TETGEN: ${LINK_TETGEN}   Link GPL licensed tetgen to ug4. Only for development builds.")
