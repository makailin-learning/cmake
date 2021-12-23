cmake_minimum_required(VERSION 3.0)
project(SWAP2)

include_directories(include) # 对应g++中的-Iinlcude参数
aux_source_directory(MAIN .)
aux_source_directory(SRC src)
add_executable(trt main.cpp src/swap2.cpp) # 这里面的斜杠采用反斜杠！！！，与g++命令行中的.\src\swap2.cpp不对应
