#设定cmake最低版本，important
cmake_minimum_required(VERSION 2.8)
#设定project名字
project(hello)
#设定变量，如果多个文件，可以罗列，比如set(SRC_LIST main.c hello.c)。不需要列出.h文件。
set(SRC_LIST main.c hello.c)
#指定可执行文件的名称(比如说hello)和source文件的名字 
add_executable(hello ${SRC_LIST})
