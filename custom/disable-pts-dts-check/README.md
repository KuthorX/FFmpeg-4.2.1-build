# disable pts dts check

原 ffmpeg `libavformat/mux.c` 中会检查

- dts 是否单调递增
- pts 是否小于 dts

如果遇到以上任一情况，程序就会强制退出。

去除该检查后，就可以自定义任意时刻的 dts、pts 了。

使用时直接用 `lib` 目录下的 lib 包覆盖原 lib 即可。
