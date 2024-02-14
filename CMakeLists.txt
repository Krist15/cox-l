cmake_minimum_required(VERSION 3.28)

project(compiler)

add_executable(compiler ./src/main.cpp)

set_target_properties(compiler PROPERTIES 
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED ON
    CXX_EXTENSIONS OFF
)

set(CMAKE_CXX_FLAGS "-Wall -Wextra -Werror")