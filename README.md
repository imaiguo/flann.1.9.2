# FLANN - Fast Library for Approximate Nearest Neighbors

1. 依赖lz4

2. msys64

## Build with MSVC

### 编译Release

```bash
> cmd
> "C:\Program Files\Microsoft Visual Studio\2022\Community\VC\Auxiliary\Build\vcvars64.bat"
> set PKG_CONFIG_PATH=D:\devtools\lz4.1.9.4\lib\pkgconfig
> set PATH=%PATH%;D:\devtools\msys64\usr\bin
> pip install setuptools -i https://pypi.tuna.tsinghua.edu.cn/simple
> mkdir build & cd build
> cmake .. -G Ninja -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=D:\devtools\flann.1.9.2
> ninja & ninja install
```

### 编译Debug
```bash
> cmake .. -G Ninja -DCMAKE_BUILD_TYPE=Debug -DCMAKE_INSTALL_PREFIX=D:\devtools\flann.1.9.2\debug\
```

## mingw64平台编译

依赖lz4

```bash
> set PKG_CONFIG_PATH=D:\devtools\lz4.1.9.4\lib\pkgconfig;%PKG_CONFIG_PATH%
```

编译

```bash
> cmake .. -G Ninja -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=D:\devtools\flann.1.9.2
```