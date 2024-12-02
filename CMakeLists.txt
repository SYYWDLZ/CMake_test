cmake_minimum_required(VERSION 3.20.0)
project(my_hello)
set(CMAKE_CXX_STANDARD 11)

include_directories(${PROJECT_SOURCE_DIR}/include)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

aux_source_directory(${PROJECT_SOURCE_DIR}/source source_list)

add_executable(my_hello ${source_list})
