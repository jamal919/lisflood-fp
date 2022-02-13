cmake_minimum_required(VERSION 3.0)

set(CMAKE_DISABLE_SOURCE_CHANGES ON)
set(CMAKE_DISABLE_IN_SOURCE_BUILD ON)

set(CMAKE_BUILD_TYPE Release)

project(lisflood)

# Output directories
# Replaces the CMAKE_INSTALL_PREFIX option
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR})
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR})
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${PROJECT_BINARY_DIR})

# Add for compilation
add_executable(lisflood lisflood.cpp lisflood.cpp pars.cpp input.cpp iterateq.cpp boundary.cpp fp_flow.cpp fp_acc.cpp
            fp_trent.cpp ch_flow.cpp util.cpp output.cpp chkpnt.cpp por_flow.cpp weir_flow.cpp sgc.cpp infevap.cpp
            initialize.cpp finalize.cpp update.cpp)