cmake_minimum_required(VERSION 3.15)
project(helloworld)
set(CMAKE_C_STANDARD 99)
set(CURRENT_EXE_NAME helloworld)
set(SOURCE_FILES src/main.c)
include_directories(${CMAKE_CURRENT_SOURCE_DIR})
add_executable(${CURRENT_EXE_NAME} ${SOURCE_FILES})
install(TARGETS ${CURRENT_EXE_NAME} RUNTIME DESTINATION bin)
