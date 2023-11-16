FLANN - Fast Library for Approximate Nearest Neighbors
======================================================


# build on windows

## mingw64平台编译

依赖lz4

```bash
> set PKG_CONFIG_PATH=D:\devtools\lz4.1.9.4\lib\pkgconfig;%PKG_CONFIG_PATH%
```

编译

```bash
> cmake .. -G Ninja -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=D:\devtools\flann.1.9.2
```