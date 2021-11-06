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

* ## List of useful CMake resources to help you if you are stuck
