cmake_minimum_required(VERSION 3.0.0)

## SETTINGS START

# Set the project name:

set(PROJECT_NAME uavccan-templae-c)

# Set the name of the executable

set(EXECUTABLE_NAME can-node)

# Set the inlude include directories

set(INLUDE_DIRS libcanard socketcan)

# Set the sources {include the headers}

set(MAIN_SOURCE ./src/main.c)
set(LIBCANARD_SRC libcanard/canard.c libcanard/canard.h) 
set(SOCKETCAN_SRC socketcan/socketcan.h socketcan/socketcan.c)

## SETTINGS END

project(${PROJECT_NAME} VERSION 0.1.0)
include(CTest)
enable_testing()

include_directories(${INLUDE_DIRS})
add_executable(${EXECUTABLE_NAME} ${MAIN_SOURCE} ${LIBCANARD_SRC} ${SOCKETCAN_SRC})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
set(CMAKE_C_STANDARD 11)
include(CPack)
