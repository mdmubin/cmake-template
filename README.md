# A Very Simple CMake Template Project

This is a very simple, bare-bones cmake project template.

---

This project was originally created by me to learn about the cmake build system.
A lot of cmake resources that I've looked into just seem very tedious and
boring. My original sentiment was something along the lines of, "I just want to
start coding, I don't care about any of this..."

So this template is just here to serve as a bare bones starting point, to get
you up and running with a very simple project structure with some template cmake
and cpp files included as examples.

---

* ## Build Instructions

1. Clone Repository:
    ```
    git clone https://github.com/mdmubin/cmake-template.git
    ```

2. Open repository clone directory, create build directory and move to build directory:
    ```
    cd cmake-template
    mkdir build
    cd build
    ```

3. Configure cmake:
    ```
    cmake ..
    ```
4. Build project:
  - debug mode
    ```
    cmake --build . --config Debug
    ```
  - release mode
    ```
    cmake --build . --config Release
    ```

The executable/library file built by cmake should now be present in `build/src/[Debug or Release]`

---

* ## Directory Structure:
```
project_root/
  |---> build/
  |       |---> (cmake files are built in this directory)
  |
  |---> external/
  |       |---> include/ (external include headers)
  |       |---> libs/ (external library files, for example: .lib, .dll,.a, .so, etc)
  |
  |---> src/
  |       |---> include/ (public headers for your library goes here)
  |       |---> ... (any source files, for example: .cpp, .c, .h, .hpp, etc)
  |       |---> CMakeLists.txt
  |
  |---> test/
  |       |---> ... (test source files, )
  |       |---> CMakeLists.txt
  |
  |---> .gitignore
  |---> CMakeLists.txt
  |---> LICENCE.txt
  |---> README.md
```

* ## List of useful CMake resources
  - [CMake Official Documentation](https://cmake.org/cmake/help/latest/)
  - [Modern CMake](https://cliutils.gitlab.io/modern-cmake/)
  - [How to Make CMake Good - Video Series](https://youtube.com/playlist?list=PLK6MXr8gasrGmIiSuVQXpfFuE1uPT615s)
  - [Modern CPP Starter](https://github.com/TheLartians/ModernCppStarter)