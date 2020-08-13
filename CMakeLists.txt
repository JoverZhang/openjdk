cmake_minimum_required(VERSION 3.7)
project(jdk14-6c954123ee8d)

include_directories(
    src/hotspot/cpu
    src/hotspot/os
    src/hotspot/os_cpu
    src/hotspot/share
    src/hotspot/share/precompiled
    src/hotspot/share/include
    src/java.base/unix/native/include
    src/java.base/share/native/include
    src/java.base/share/native/libjli
)

file(GLOB_RECURSE SOURCE_FILES "*.cpp" "*.hpp" "*.c" "*.h")
add_executable(hotspot ${SOURCE_FILES})
