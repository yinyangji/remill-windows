it built success on Windows system
need tob_libraries, expect for llvm in the directory
install llvm before build remill
need install z3 and pthread, you can install them with vcpkg

cmake -G "Visual Studio 15 2017" -T llvm -A x64 -DCMAKE_BUILD_TYPE=Release -DCXX_COMMON_REPOSITORY_ROOT=D:\tools\code\compile\tob_libraries  -DCMAKE_INSTALL_PREFIX=${INSTALL_PATH} ..\remill

cmake --build . --config release

Cmake --install . --config release
