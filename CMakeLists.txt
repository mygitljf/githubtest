cmake_minimum_required(VERSION 3.12)
project(c22v1)

# set(CMAKE_CXX_STANDARD 17)
set(CMAKE_C_STANDARD 99)


#调用flex将auto_lex.l  在cmake-build-debug目录下面生成对应文件

#debug必备
add_compile_options(-g -O0)
#生成可以执行文件
add_executable(compiler
        hello.cpp )
set(CMAKE_BUILD_TYPE Debug)
#aux_source_directory(. DIR_SRC)

# file(GLOB_RECURSE DIR_LIB_SRC "third_party/*.cpp")
# add_compile_options(-g -O0)
# include_directories(src)
# include_directories(third_party/antlr4-runtime)
# add_executable(compiler ${DIR_SRC} ${DIR_LIB_SRC})
#add_executable(xiaolin main.cpp)