cmake_minimum_required(VERSION 3.10)

project(Game)

set(CMAKE_CXX_STANDARD 17)

add_executable(chess
    src/main.cpp
    src/game.cpp
    src/board.cpp
    src/pieces.cpp
)

target_link_libraries(chess raylib GL m pthread dl rt X11)