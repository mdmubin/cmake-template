# A Simple CMake Template Project

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

1. **Clone Repository**:
    ```
    git clone https://github.com/mdmubin/cmake-template.git
    ```

2. **Open clone directory, create build directory and change current directory to
build directory**:
    ```
    cd cmake-template
    mkdir build
    cd build
    ```

3. **Configure cmake**:
    ```
    cmake ..
    ```
4. **Build project**:
  - debug mode
    ```
    cmake --build . --config Debug
    ```
  - release mode
    ```
    cmake --build . --config Release
    ```

I am using `MSVC` compiler and for me the executable/library file built by cmake
is present in `../project-root/build/src/[Debug or Release]/`. If you are using
a different compiler, you might not find it in the same directory as I did.

---

* ## Directory Structure:
  This is just a directory structure that I personally think manages to arrange
  every file in a neat manner.
```
project_root/
  |---> build/
  |       |---> (cmake files are built in this directory)
  |
  |---> external/
  |       |---> include/ (external include headers)
  |       |---> libs/ (external library files, for example: .lib, .dll, etc)
  |
  |---> src/
  |       |---> include/ (public headers for your library goes here)
  |       |---> ... (any source files, for example: .cpp, .c, .h, .hpp, etc)
  |       |---> CMakeLists.txt
  |
  |---> test/
  |       |---> ... (test source files)
  |       |---> CMakeLists.txt
  |
  |---> .gitignore
  |---> CMakeLists.txt
  |---> LICENCE.txt
  |---> README.md
```

* ## List of useful CMake resources
  - [CMake Official Documentation](https://cmake.org/cmake/help/latest/)
  - [How to Make CMake Good - Video Series](https://youtube.com/playlist?list=PLK6MXr8gasrGmIiSuVQXpfFuE1uPT615s)
  - [Modern CMake](https://cliutils.gitlab.io/modern-cmake/)
  - [Modern CPP Starter](https://github.com/TheLartians/ModernCppStarter)


* **I plan to add a simple cmake test, as soon as I learn more about it**
