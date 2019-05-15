cmake_minimum_required(VERSION 3.14)

project(spdlog_cmake)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(external/spdlog)

find_package(spdlog)

add_executable(spdlog_cmake main.cpp)

target_link_libraries(spdlog_cmake
  spdlog
)