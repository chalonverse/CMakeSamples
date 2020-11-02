# This says we require C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# This says to find zlib and error out if not found
find_package(ZLIB REQUIRED)

# This says to create an executable target called Ex06 that compiles Main.cpp
add_executable(Ex06 Main.cpp)

# This says we need to link against ZLIB
target_link_libraries(Ex06 PRIVATE ZLIB::ZLIB)
