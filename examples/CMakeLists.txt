file(GLOB SRC_FILES *.cpp)
add_executable(examples ${SRC_FILES})

target_link_libraries(examples cspeak_framework)