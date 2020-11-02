# This says we require C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# This grabs all files in this directory that end with .cpp
# and saves it in a variable called ${source_files}
file(GLOB source_files CONFIGURE_DEPENDS "*.cpp")

# This says to create an executable target called Ex03 that compiles the ${source_files}
add_executable(Ex04 ${source_files})