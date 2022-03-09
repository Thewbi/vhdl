# Source of this project

https://github.com/gabriele-tomassetti/antlr-cpp
https://github.com/antlr/antlr4/tree/master/runtime/Cpp/cmake

## Building

Download antlr-4.9.3-complete.jar from here: https://www.antlr.org/download.html
Place antlr-4.9.3-complete.jar into the bin folder in this project.

Update the CMakeLists.txt file.
In there, replace

```
set(ANTLR_EXECUTABLE /home/user/antlr-4.9.3-complete.jar)
```

by

```
set(ANTLR_EXECUTABLE ${CMAKE_CURRENT_SOURCE_DIR}/bin/antlr-4.9.3-complete.jar)
```

Run cmake so it can generate the build infrastructure for your operating system
run make to finally build the executable

```
cd buildfolder
cmake ../
make
```

You can run the demo application by executing the binary:

```
cd buildfolder
./demo
```

## The demo application

You can run the demo application by executing the binary:

```
cd buildfolder
./demo
```
