cmake_minimum_required (VERSION 2.8.11)
project (tnyosc)

add_library (tnyosc STATIC src/tnyosc-dispatch.cc)

target_include_directories (tnyosc PUBLIC include/)