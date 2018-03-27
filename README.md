# ffmpeg-examples

Examples in C of FFMPEG

## List of examples

* decoding encoding
* muxing
* remuxing
* avio reading
* metadata

## Building

    mkdir -p build
    cd build
    cmake ..
    make

## Examples

    ./build/muxing rtmp://url/video.flv
    ./build/muxing video.mp4
    ./build/muxing udp://ip:port
