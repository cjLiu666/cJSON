cmake_minimum_required(VERSION 3.15)
project(cjson)

add_executable(test test.c cJSON.c)

link_directories(/usr/lib/x86_64-linux-gnu) #添加动态连接库的路径
target_link_libraries(test -lm)