cmake_minimum_required(VERSION 2.8)

SET(COMPILE_DEFINITIONS -Werror)

include_directories(/usr/local/include)

LINK_DIRECTORIES(/usr/local/lib)

add_executable(muxing muxing.c)
add_executable(decoding_encoding decoding_encoding.c)

SET(AV_LIB pthread avdevice avfilter postproc avformat avcodec xcb-shm xcb X11 asound x264 pthread rtmp gnutls mp3lame freetype fdk-aac z swresample swscale avutil rt m) 
target_link_libraries(muxing ${AV_LIB}) 
target_link_libraries(decoding_encoding ${AV_LIB})
