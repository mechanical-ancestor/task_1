# 1. 指定CMake最低版本（Ubuntu一般3.10以上够用）
cmake_minimum_required(VERSION 3.10)

# 2. 给项目起个名（随便起，这里叫HelloMA）
project(HelloMA)

# 3. 设置C++标准（用C++11，兼容性好）
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 4. 生成可执行文件：
# 第一个参数「HelloMA_EXE」是最终生成的程序名；
# 第二个参数「main.cpp」是要编译的源文件
add_executable(HelloMA_EXE main.cpp)