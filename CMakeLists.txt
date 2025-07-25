cmake_minimum_required(VERSION 3.10.0)

project(spidevpp)

# Libs
add_subdirectory(libs/)
option( COMPILE_EXAMPLE_APPS "Compile the example app" OFF )

# Apps
if ( COMPILE_EXAMPLE_APPS )
    add_subdirectory(apps/loopback_example_app)
endif ()
