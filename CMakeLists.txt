cmake_minimum_required(VERSION 3.0)
project(tetris_SJH)

add_executable(tetris_SJH src/main.c src/display_menu.c src/display_tetris.c)
target_include_directories(tetris_SJH PUBLIC include)

install(TARGETS tetris_SJH DESTINATION / usr/local/bin)
install(DIRECTORY ${CMAKE_SOURCE_DIR}/include DESTINATION / usr/local/include)
install(DIRECTORY ${CMAKE_SOURCE_DIR}/src/ DESTINATON / usr/local/src)