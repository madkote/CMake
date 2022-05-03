# Steps

## First build
```sh
mkdir build && cd build
cmake ../
cmake --build .
./Tutorial 9
```

## Version build
```sh
rm -rf build && mkdir build && cd build
cmake ../
cmake --build .
./Tutorial 9
./Tutorial
```

`cmake ../Step2 -DUSE_MYMATH=OFF`