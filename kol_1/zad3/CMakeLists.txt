cmake_minimum_required(VERSION 3.5.1)

project (myProgram)
set(CMAKE_BINARY_DIR ${CMAKE_BINARY_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR}/lib)

include_directories("${PROJECT_SOURCE_DIR}")

add_executable(myProgram ${PROJECT_SOURCE_DIR}/employee.cpp ${PROJECT_SOURCE_DIR}/address.cpp ${PROJECT_SOURCE_DIR}/main.cpp ${PROJECT_SOURCE_DIR}/employee.h ${PROJECT_SOURCE_DIR}/address.h)
