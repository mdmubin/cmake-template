# A Very Simple CMake Template Project

This is a very simple, bare-bones cmake project template.

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
---
* ## Build Instructions

