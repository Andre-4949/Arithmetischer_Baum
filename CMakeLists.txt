cmake_minimum_required(VERSION 3.22)
project(LaborRechenBaum)

set(CMAKE_CXX_STANDARD 17)

file(GLOB_RECURSE SRC "include/*.h" "include/*.hpp" "src/*.cpp")

add_executable(LaborRechenBaum ${SRC})
