# CMake Samples #
This repo contains sample projects demonstrating basic CMake functionality.

## How to Build (in a UNIX shell)##
1. Make a build directory `mkdir build` (this isn’t technically required, but it’s good to separate the temp build data from the rest!)
2. Change to the build directory `cd build`
3. Tell cmake to generate data for platform-specific build system `cmake ..`
4. Tell cmake to execute platform-specific build commands `cmake --build .`
