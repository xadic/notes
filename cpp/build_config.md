## Build Config

### 人脸识别模型Ultra-Light-Fast-Generic-Face-Detector-1MB


安装依赖库:
```sh
sudo pacman -S opencv hdf5 glew vtk
```
或者直接安装opencv和opencv-samples
```sh
sudo pacman -S opencv opencv-samples
```

克隆到本地:
```sh
git clone --recursive --depth=1 https://github.com/Linzaer/Ultra-Light-Fast-Generic-Face-Detector-1MB
```

更新ncnn,否则可能报错
```sh
cd Ultra-Light-Fast-Generic-Face-Detector-1MB/ncnn
git pull
```

编译:
```sh
cd Ultra-Light-Fast-Generic-Face-Detector-1MB/ncnn
mkdir build && cd build && cmake ..
make -j$(nproc)
```

测试:
```sh
./main ../data/version-RFB/RFB-320.bin ../data/version-RFB/RFB-320.param ../data/test.jpg
```

####
[Ultra-Light-Fast-Generic-Face-Detector-1MB](https://github.com/Linzaer/Ultra-Light-Fast-Generic-Face-Detector-1MB)
[C++ implemententation of Ultra-Light-Fast-Generic-Face-Detector-1MB with NCNN](https://github.com/Linzaer/Ultra-Light-Fast-Generic-Face-Detector-1MB/tree/master/ncnn)
