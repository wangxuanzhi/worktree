cmake_minimum_required(VERSION 2.8)
project(pickup)
find_package(qibuild)

set(_srcs 
  pickup.h
  pickupWXZ.cpp
  main.cpp
  wxzSVM.cpp
  wxzSVM.h
)

qi_create_bin(pickup ${_srcs})

qi_use_lib(pickup ALCOMMON ALPROXIES ALVISION OPENCV2_WORLD )
