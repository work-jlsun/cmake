project(test)
#添加当前目录下的所有文件
AUX_SOURCE_DIRECTORY(. DIR_TEST1_SRCS)
#生成库
ADD_LIBRARY( test ${DIR_TEST1_SRCS})
