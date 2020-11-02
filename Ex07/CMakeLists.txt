# This says we require C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# This is required to issue any FetchContent commands
include(FetchContent)

# This declares "catch" as a git repository we depend on
FetchContent_Declare(
  catch
  GIT_REPOSITORY https://github.com/catchorg/Catch2.git
  GIT_TAG        v2.13.3
)

# This says we want the "catch" we declared available
FetchContent_MakeAvailable(catch)

# The ${catch_SOURCE_DIR} variable is set by MakeAvailable
# In this case we want catch.hpp to be in the include path
include_directories(${catch_SOURCE_DIR}/single_include/catch2)

# This says to create an executable target called Ex07 that compiles Main.cpp
add_executable(Ex07 Main.cpp)
