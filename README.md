# FFmpeg-4.2.1-build

注意 extra 文件下的为本项目的 ffmpeg-build 后需要依赖的 lib 和 include，需要放到机器的相应目录下。

本 build 使用的 configure 参数：

```
./configure --enable-shared --prefix=/usr/local --disable-x86asm --enable-libx264 --enable-libx265 --enable-filters --enable-openssl --enable-nonfree --enable-gpl --enable-static --enable-libfdk-aac --enable-libmp3lame
```

## `custom` folder

为了实现一些特殊推流，需要对 ffmpeg 源码做改动并重新 build ，详情可进入每个子目录的 README.md 查看。