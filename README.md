# Use Fun Console in Your Project

[![Build Status](https://travis-ci.com/joshpeterson/fun-console-cmake.svg?branch=master)](https://travis-ci.com/joshpeterson/fun-console-cmake)

Want to integrate [Fun Console](https://github.com/joshpeterson/fun-console) in your C++ project? Using CMake to build your project? You can use use this repository as an example!

1. Add the fun-console project as a submodule: `git submodule add git@github.com:joshpeterson/fun-console.git external/fun-console`
2. Update the submodule: `git submodule update --init --recursive`
3. Add this line to your CMakeLists.txt: `add_subdirectory(external/fun-console)`
4. Add `fun-console_lib` as a library: `target_link_libraries(${PROJECT_NAME} PRIVATE fun-console_lib)`

That's it!
