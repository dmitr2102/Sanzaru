**Download:**
```console
git clone --recursive https://github.com/dmitr2102/Sanzaru.git -b rilley78
```
>изменить после пулла
  
**Install GameNetworkingSockets:**

```console
cd GameNetworkingSockets

git clone https://github.com/microsoft/vcpkg && .\vcpkg\bootstrap-vcpkg.bat 

.\vcpkg\vcpkg install --triplet=x64-windows

cmake -G "Visual Studio 17 2022" -A x64 -B build
```
and if you want to build with examples:

```console
cmake -G "Visual Studio 17 2022" -A x64 -B build -DBUILD_EXAMPLES=ON -DBUILD_TESTS=ON -DUSE_STEAMWEBRTC=ON
```
Открыть build/GameNetworkingSockets.sln в Visual Studio, собрать

>Переделать сборку, слишком геморно