CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

#项目最后可执行文件名称
PROJECT(main)

#包含子目录src,即递归到子目录进行编辑
ADD_SUBDIRECTORY( src )

#添加include文件的目录(直接目录)
INCLUDE_DIRECTORIES( ./src )

#添加链接库的目录
#LINK_DIRECTORIES(${PROJECT_SOURCE_DIR})

#生成可执行文件依赖的文件
ADD_EXECUTABLE(main main.cpp)

#生成可执行文件依赖的库
TARGET_LINK_LIBRARIES(main test)


