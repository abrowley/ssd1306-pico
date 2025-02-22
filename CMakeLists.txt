cmake_minimum_required(VERSION 3.30)
set(CMAKE_CXX_STANDARD 20)

include(pico_sdk_import.cmake)


project(ssd1306-pico)

pico_sdk_init()

add_library(${PROJECT_NAME} src/ssd1306.c)
target_include_directories(${PROJECT_NAME} PRIVATE include)
target_link_libraries(${PROJECT_NAME} pico_stdlib hardware_i2c)
