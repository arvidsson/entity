cmake_minimum_required(VERSION 3.11)

project(entity VERSION 1.0.0 LANGUAGES CXX)

add_library(entity
  entity/world.cpp
  entity/system.cpp
  entity/event.cpp
  entity/entity.cpp
  entity/component.cpp
)

target_compile_features(entity PRIVATE cxx_std_17)

target_include_directories(entity
  PUBLIC
  ${CMAKE_CURRENT_SOURCE_DIR}
)
