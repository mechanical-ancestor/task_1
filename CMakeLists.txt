# 1. 告诉CMake：你至少得是3.10版本才能用（Ubuntu自带的CMake够这个版本）
cmake_minimum_required(VERSION 3.10)

# 2. 给你的项目起个名字（叫HelloMA，和文件夹名一致，好记）
project(HelloMA)

# 3. 用C++11标准编译（兼容性最好，不会报错）
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON) # 强制要求用C++11

# 4. 生成可执行文件：
# 第一个参数「HelloMA_EXE」= 最终编译出来的程序名（随便起，比如叫abc也能行）
# 第二个参数「main.cpp」= 要编译的C++源文件（就是刚才写的代码文件）
add_executable(HelloMA_EXE main.cpp)