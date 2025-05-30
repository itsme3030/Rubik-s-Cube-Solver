cmake_minimum_required(VERSION 3.10.0)
project(main VERSION 0.1.0 LANGUAGES C CXX)

add_executable(main main.cpp 
    Model/RubiksCube.cpp 
    Model/RubiksCube.h 
    Model/RubiksCube1dArray.cpp 
    Model/RubiksCube3dArray.cpp 
    Model/RubiksCubeBitboard.cpp
    Solvers/DFSSolver.h
    Solvers/BFSSolver.h
)

include(CTest)
enable_testing()

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
