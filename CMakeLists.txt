cmake_minimum_required (VERSION 3.5)

LIST(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")

project(cpp_parser)

set(CMAKE_DISABLE_SOURCE_CHANGES ON)
set(CMAKE_DISABLE_IN_SOURCE_BUILD ON)

set(VENDOR_DIR "${CMAKE_SOURCE_DIR}/../vendor")

message("Vendor: ${VENDOR_DIR}")

add_subdirectory(src)
