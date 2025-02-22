cmake_minimum_required(VERSION 3.30)
set(CMAKE_CXX_STANDARD 20)

project(ssd1306)

add_library(ssd1306 INTERFACE ssd1306.c)
