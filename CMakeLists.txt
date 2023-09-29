cmake_minimum_required(VERSION 3.27 FATAL_ERROR)

project(cmake
    VERSION         0.0.1
    DESCRIPTION     "wangbairu's cmake demo"
    HOMEPAGE_URL    "xxxx"
    LANGUAGES       C CXX
)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(BuildInfo)

add_subdirectory(external)

add_subdirectory(src)

add_subdirectory(docs)

add_subdirectory(test)

add_subdirectory(packaging)

