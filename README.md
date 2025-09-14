# Spinning 3D cube
This C++ app renders a spinning 3D cube in [VulkanSceneGraph](https://vsg-dev.github.io/vsg-dev.io/)

## Pre-Requisities to Running
Make sure you have the following installed:
* vcpkg

Make sure you have the following environment variables set:

| Env         | Description               |  
|-------------|---------------------------|
| VCPKG_ROOT  | Root of the vcpkg config  |   


## How to run the program
In the same directory as the `CMakeLists.txt`, run the following:
```bash
 /usr/bin/cmake -DCMAKE_TOOLCHAIN_FILE=$VCPKG_ROOT/scripts/buildsystems/vcpkg.cmake -S . -B ./build -G Ninja
```
Followed by,
```bash
/usr/bin/cmake --build ./build
```
Finally, run the program with,
```bash
./build/vsg_example
```