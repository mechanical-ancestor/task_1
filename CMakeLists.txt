cmake_minimum_required(VERSION 3.10)  # 最低 CMake 版本要求

# 项目名称和支持的语言（C/C++）
project(MyProject 
    VERSION 1.0.0
    LANGUAGES C
)

add_executable(${PROJECT_NAME} src/main.c)