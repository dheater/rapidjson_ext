# rapidjson_ext
Wrappers and extensions to [RapidJSON](http://rapidjson.org/)

# Installation
## Dependencies
CMake
[rapidjson](https://github.com/miloyip/rapidjson)

## Building and Installing
1. Create a directory called `build` within this directory.
2. Change to `build` directory and run `cmake ..` command to configure your build.
3. Run `make` to build the library.
4. Run `make install` (requires root privledges)

The library is installed into ${CMAKE_INSTAL_PREFEX}/lib, typically, /usr/local/lib

The header files are intalled into ${CMAKE_INSTAL_PREFEX}/include/rapidjson
