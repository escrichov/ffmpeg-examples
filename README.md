# ffmpeg-examples

# Building

    mkdir -p build
    cd build
    cmake ..
    make

# Examples

    ./build/muxing rtmp://url/video.flv
    ./build/muxing video.mp4
    ./build/muxing udp://ip:port
