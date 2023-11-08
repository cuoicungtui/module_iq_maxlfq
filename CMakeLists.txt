cmake_minimum_required(VERSION 3.4...3.18)
project(iq_lfq_Pypi)

add_subdirectory(pybind11)
pybind11_add_module(iq_test src/iqWithPybind11.cpp)

# EXAMPLE_VERSION_INFO is defined by setup.py and passed into the C++ code as a
# define (VERSION_INFO) here.
target_compile_definitions(iq_test
                           PRIVATE VERSION_INFO=${EXAMPLE_VERSION_INFO})
