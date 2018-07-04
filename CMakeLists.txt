# CMake project for the Project:ROGUE game
# Created by Malachi for JustPlayLabs
# JustPlayLabs is owned in full by Kaprisoft, Inc.
#

# Project declaration
project(projectrogue CXX)

# Project executable
add_executable(projectrogue src/projectrogue.cpp src/projectrogue.h)

# Minimum required CMake version
cmake_minimum_required(VERSION 3.10)

# Compile features
target_compile_features(projectrogue PRIVATE cxx_std_11)

# Header include directories
target_include_directories(projectrogue PRIVATE
inc/
inc/VulkanSDK/1.1.73.0/Include/vulkan/
inc/VulkanSDK/1.1.73.0/Include/shaderc/
inc/VulkanSDK/1.1.73.0/Lib/
)
