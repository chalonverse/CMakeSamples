# This says we require C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# This says to create an executable target called Ex03 that compiles Main.cpp and Hello.cpp
add_executable(Ex03 Main.cpp Hello.cpp)