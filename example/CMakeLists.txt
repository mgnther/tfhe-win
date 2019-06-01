cmake_minimum_required(VERSION 3.14)
project(TFHE_Win_Test)

set(CMAKE_CXX_STANDARD 14)
include_directories("C:\\Program Files (x86)\\tfhe\\include")
find_library(TFHE libtfhe-fftw HINTS "C:/Program Files (x86)/tfhe/bin")
add_executable(TFHE_Win_Test main.cpp)
target_link_libraries(TFHE_Win_Test "${TFHE}")