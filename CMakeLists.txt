cmake_minimum_required(VERSION 3.10)
project(tensor)

add_library(libtensor INTERFACE
    src/include/tensor/format.hpp
    src/include/tensor/index_generator.hpp
    src/include/tensor/layout.hpp
    src/include/tensor/slice.hpp
    src/include/tensor/storage.hpp
    src/include/tensor/stride_generator.hpp
    src/include/tensor/tensor_ops.hpp
    src/include/tensor/tensor_slice.hpp
    src/include/tensor/tensor.hpp
    src/include/tensor/types.hpp
)

target_include_directories(libtensor INTERFACE src/include)
