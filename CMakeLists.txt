project(qdbmp C)
cmake_minimum_required(VERSION 2.8)

add_library(qdbmp_shared SHARED qdbmp.c)
add_library(qdbmp_static STATIC qdbmp.c)

set_target_properties(
  qdbmp_shared qdbmp_static
  PROPERTIES
  OUTPUT_NAME qdbmp
)
