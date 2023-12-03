## Prerequisites

* A compiler with C++11 support
* Pip 10+ or CMake >= 3.4 (or 3.14+ on Windows, which was the first version to support VS 2019)
* Ninja or Pip 10+

## SETUP CMAKE
* download cmake x64 https://cmake.org/download/
* install cmake x64
* add cmake to PATH (C:\Program Files\CMake\bin) into system environment variable
* Check cmake version in cmd
```bash
cmake --version

#cmake version 3.26.5
#CMake suite maintained and supported by Kitware (kitware.com/cmake).
```
=> success

## SETUP Visual Studio >=2017

* download Visual Studio https://visualstudio.microsoft.com/downloads/
* Install Visual Studio
* visual studio installer -> modify
* select Desktop development with C++
* Done
  

## Installation

Just clone this repository and pip install. Note the `--recursive` option which is
needed for the pybind11 submodule:

```bash
git clone --recursive https://github.com/cuoicungtui/module_iq_maxlfq.git
pip install ./module_iq_maxlfq.git
```

With the `setup.py` file included in this example, the `pip install` command will
invoke CMake and build the pybind11 module as specified in `CMakeLists.txt`.
