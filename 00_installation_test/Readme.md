# Installation 'OpenCV' 


## Installation
On ubuntu 
```sh
sudo apt-get install -y \
    cmake \
    build-essential

sudo apt-get install libopencv-dev
```

Verify the installation by checking the version of OpenCV:
```sh
pkg-config --modversion opencv4
```

# OpenCV C++ Installation

This guide explains how to compile a C++ project using OpenCV with CMake.

## 1. Find the OpenCV Config File

Run this command to locate `OpenCVConfig.cmake`:

```sh
sudo find / -name OpenCVConfig.cmake
/usr/lib/x86_64-linux-gnu/cmake/opencv4/OpenCVConfig.cmake

```

```sh
echo 'export OpenCV_DIR=/usr/lib/x86_64-linux-gnu/cmake/opencv4' >> ~/.bashrc
```

3. Generate Build Files
Run CMake to create the build system files:
```sh
cmake -B build -S .
```

4. Compile the Project
Compile the project in Release mode:
```sh
cmake --build build --config Release
```

5. Run the Executable
```sh
Execute the compiled binary:
```

## python
```sh
pip install opencv-contrib-python
```


