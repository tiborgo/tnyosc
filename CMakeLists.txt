cmake_minimum_required (VERSION 2.8.11)
project (tnyosc)

file(GLOB headers "include/*")

add_library (tnyosc STATIC src/tnyosc-dispatch.cc)

target_include_directories (tnyosc PUBLIC include/)

install (TARGETS tnyosc
         ARCHIVE DESTINATION lib)
         
install (FILES ${headers}
         DESTINATION include)