cmake_minimum_required(VERSION 3.10)
project(TestClangLLVM)

#set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD 14)
#set(CMAKE_CXX_STANDARD 17)
set(CMAKE_TOOLCHAIN_PREFIX=llvm-)
set(CMAKE_C_COMPILER=C:/msys64/mingw64/bin/clang.exe)
set(CMAKE_CXX_COMPILER=C:/msys64/mingw64/bin/clang++.exe)
#set(CMAKE_CXX_FLAGS -m32)
set(CMAKE_CXX_FLAGS -m64)

add_executable(TestClangLLVM main.cpp Animal.h Cat.cpp Cat.h Dog.cpp Dog.h Rabbit.cpp Rabbit.h)
