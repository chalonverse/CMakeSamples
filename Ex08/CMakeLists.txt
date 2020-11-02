# This says we require C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Are we on Windows?
if (WIN32)
	# Use existing compiler flags plus /WX
	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} /WX")
# Are we on Mac?
elseif (APPLE)
	# Use existing compiler flags plus -Werror
	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Werror")
# If neither of these, assume another Unix platform
else()
	# Use existing compiler flags plus -Werror
	set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Werror")
endif()

# This is a normal executable target
add_executable(Ex08 Main.cpp)