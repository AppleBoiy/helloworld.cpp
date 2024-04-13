# Basic setup for a CMake project
cmake_minimum_required(VERSION 3.5)
project(HELLOWORLD)

# Set the C++ standard to use
set(CMAKE_CXX_STANDARD 11)

# set the output directory
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

# set the source directory
set(SOURCE_DIR ${CMAKE_SOURCE_DIR}/src)

# Add the executable
add_executable(helloworld ${SOURCE_DIR}/main.cpp)

# Add custom command to clean up the build directory
add_custom_target(clean-all
    COMMAND ${CMAKE_COMMAND} -E remove_directory ${CMAKE_BINARY_DIR}/bin
    COMMENT "Clean up build directory"
)
