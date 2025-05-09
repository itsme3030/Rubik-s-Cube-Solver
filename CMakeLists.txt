cmake_minimum_required(VERSION 3.10.0)
project(main VERSION 0.1.0 LANGUAGES C CXX)

add_executable(main main.cpp RubiksCube.cpp RubiksCube.h RubiksCube1dArray.cpp RubiksCube3dArray.cpp RubiksCubeBitboard.cpp)

include(CTest)
enable_testing()

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
