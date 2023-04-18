# Jeston-Tx2配置教程

![Cover](planner_learning/img/animation_medium.gif)

## 从零开始安裝

### Requirements

- `Ubuntu 18.04`
- `ROS Melodic`
- `gcc/g++ 7.5.0.`


### Others

```bash

```



### Compile `Open3d v0.9.0`

```bash
git clone --recursive https://github.com/isl-org/Open3d.git
cd Open3d
git checkout v0.9.0
git submodule update --init --recursive
bash ./util/scripts/install-deps-ubuntu.sh
mkdir build
cd build
cmake -DCMAKE_INSTALL_PREFIX=$HOME/open3d_install ..
make -j$(nproc)
make install
```

#### Possible error !

`SDL库`：

```bash
sudo apt-get install libsdl-image1.2-dev
```

***[What is sdl ?](https://en.wikipedia.org/wiki/Simple_DirectMedia_Layer)***

`libffi`：

***[What is libffi ?](https://sourceware.org/libffi/)***

