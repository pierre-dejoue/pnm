add_executable(unicolor unicolor.cpp)
if(MSVC)
set_target_properties(unicolor
    PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/sample
)
else()
set_target_properties(unicolor
    PROPERTIES
    COMPILE_FLAGS "-std=c++11 -O2 -Wall -Wpedantic -Wextra"
    RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/sample
)
endif()

add_executable(mandelbrot mandelbrot.cpp)
if(MSVC)
set_target_properties(mandelbrot
    PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/sample
)
else()
set_target_properties(mandelbrot
    PROPERTIES
    COMPILE_FLAGS "-std=c++11 -O2 -Wall -Wpedantic -Wextra"
    RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/sample
)
endif()
