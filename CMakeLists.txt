#设置最小cmake版本
cmake_minimum_required(VERSION 3.16)
project(cppstudent VERSION 0.1.0)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

include(CTest)
enable_testing()

add_executable(cppstudent main.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
