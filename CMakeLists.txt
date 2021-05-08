cmake_minimum_required(VERSION 3.0)
enable_testing()
project(pnm++)

if(MSVC)
    add_compile_options("/Zc:__cplusplus")
endif()

include_directories(${PROJECT_SOURCE_DIR})

add_subdirectory(sample)
add_subdirectory(test)
