
# Necessary CMake
project(XTextureExtractor CXX)
cmake_minimum_required(VERSION 2.8)

# Include the SDK. Adjust this path to wherever you have the SDK repository
add_subdirectory(SDK/ bin/)

# Set up the plugin
add_xplane_plugin(XTextureExtractor 300
  lodepng/lodepng.cpp
  XTextureExtractor.cpp
  XTextureExtractorNetwork.cpp
)

