
cmake_minimum_required(VERSION 3.4.1)
#定义一个NO_CRYPTO宏 忽略openssl的错误
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -DNO_CRYPTO")
add_library(
        rtmp
        STATIC
        amf.c
        hashswf.c
        log.c
        parseurl.c
        rtmp.c
)





