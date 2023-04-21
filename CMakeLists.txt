CMAKE_MINIMUM_REQUIRED(VERSION 3.20)
project(Tetris)

include_directories(project/include)

find_package(SFML 2.5 COMPONENTS graphics audio REQUIRED)

add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} sfml-graphics sfml-audio)

