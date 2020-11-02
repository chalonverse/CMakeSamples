# This says we require C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# This says to create a library called Ex05Lib that compiles Hello.cpp
add_library(Ex05Lib Hello.cpp)
