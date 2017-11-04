cmake_minimum_required(VERSION 3.1)

project(nano)

set(nano_headers
  nano_function.hpp
  nano_observer.hpp
  nano_signal_slot.hpp
  )

add_library(nano INTERFACE)
target_sources(nano INTERFACE
  ${nano_headers}
  )

install(FILES ${nano_headers} DESTINATION "include/nano")
