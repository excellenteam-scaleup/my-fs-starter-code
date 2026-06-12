cmake_minimum_required(VERSION 3.10)
project(myfs)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(myfs
    myfs_main.cpp
    myfs.cpp
    vfs.cpp
    blkdev.cpp
)

target_compile_options(myfs PRIVATE -Wall -g)
