# project-baseConfig<br>
I will use this template.<br>
I am making this for cross-compiling and to be stopping relying Visual Studio.<br>

# Prerequisite environment<br>
* CMake<br>
* Ninja(Build system)<br>
* Clang(llvm)<br>

**Option**<br>
* Visual Studio Code<br>
    * CMake Tools<br><https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools>
    * CodeLLDB<br><https://marketplace.visualstudio.com/items?itemName=vadimcn.vscode-lldb>

# Use Command<br>
* Debug<br>
cmake -G "Ninja" -B build -DCMAKE_BUILD_TYPE=Debug<br>
cmake --build build<br>

* Release<br>
cmake -G "Ninja" -B build -DCMAKE_BUILD_TYPE=Release<br>
cmake --build build<br>