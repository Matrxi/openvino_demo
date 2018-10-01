

## Prerequisities

## Usage

* Go to https://software.intel.com/openvino-toolkit to download and install a toolkit.

* Open a terminal in Linux or Development Command Prompt in Windows and setup
environment variables to locate libraries:

  * Linux
  ```
  source /opt/intel/computer_vision_sdk_2018.3.343/bin/setupvars.sh
  ```
  * Windows
  ```
  C:\Intel\computer_vision_sdk_2018.3.343\bin\setupvars.bat
  ```

* Clone this repository using git or download [an archive](https://github.com/dkurt/openvino_demo/archive/master.zip):
```
git clone https://github.com/dkurt/openvino_demo.git
```

* Build

  * Linux
  ```
  cd openvino_demo && mkdir build && cd build
  cmake .. -DCMAKE_BUILD_TYPE=Release && make -j8
  ```

  * Windows (assuming that `openvino_demo\build` is a current working directory)
  ```
  "C:\Program Files\CMake\bin\cmake.exe" -DCMAKE_BUILD_TYPE=Release -G "Visual Studio 14 Win64" ..
  "C:\Program Files\CMake\bin\cmake.exe" --build . --config Release
  ```