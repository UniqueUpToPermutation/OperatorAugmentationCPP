cmake_minimum_required(VERSION 3.7)
project(OperatorAugmentation)

find_package(Eigen3 3.3 REQUIRED NO_MODULE)

set(CMAKE_CXX_STANDARD 14)

add_executable(OperatorAugmentation main.cpp augmentation.cpp diagnostics.h dgnGridLaplacian1D.cpp dgnGridLaplacian2D.cpp diagnostics.cpp)
target_link_libraries(OperatorAugmentation Eigen3::Eigen)