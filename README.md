# project-baseConfig<br>

# Prerequisite environment<br>
*CMake<br>
*Ninja(Build system)<br>
*Clang(llvm)<br>

# Use Command<br>
* Debug<br>
cmake -G "Ninja" -B build -DCMAKE_BUILD_TYPE=Debug<br>
cmake --build build<br>

* Release<br>
cmake -G "Ninja" -B build -DCMAKE_BUILD_TYPE=Release<br>
cmake --build build<br>