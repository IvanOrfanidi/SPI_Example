# Version CMake
cmake_minimum_required(VERSION 3.10)

# Project name
project(spi_examples)

set(SPIDEV_TEST "spidev_test")
file(GLOB_RECURSE SPIDEV_TEST_SOURCES
    src/spidev_test.c
)

set(SPIDEV_FDX "spidev_fdx")
file(GLOB_RECURSE SPIDEV_FDX_SOURCES
    src/spidev_fdx.c
)

add_executable(${SPIDEV_TEST} ${SPIDEV_TEST_SOURCES})
add_executable(${SPIDEV_FDX} ${SPIDEV_FDX_SOURCES})