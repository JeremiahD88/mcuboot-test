# CMakeLists.txt

cmake_minimum_required(VERSION 3.13.1)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(mcuboot_test)

target_include_directories(app PRIVATE ${ZEPHYR_BASE}/include)
target_sources(app PRIVATE src/main.c)