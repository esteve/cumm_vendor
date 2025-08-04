cmake_minimum_required(VERSION 3.10)
project(cumm_vendor CXX)

find_package(ament_cmake REQUIRED)
find_package(ament_cmake_vendor_package REQUIRED)

ament_vendor(cumm_vendor
  VCS_URL https://github.com/FindDefinition/cumm.git
  VCS_VERSION v0.5.3
  GLOBAL_HOOK
)

ament_package()
