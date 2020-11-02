# This says we require C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# This says that we want to be able to include headers from the Ex05Lib directory
include_directories(../Ex05Lib)

# This says to create an executable target called Ex05Exe that compiles Main.cpp
add_executable(Ex05Exe Main.cpp)

# This says to link Ex05Exe with the Ex05Lib library
target_link_libraries(Ex05Exe Ex05Lib)
