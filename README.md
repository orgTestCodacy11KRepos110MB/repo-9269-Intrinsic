# Intrinsic

# Getting started

## Prerequisites

* Visual Studio 2015
* CMake >= 3.5
* Qt 5.7
* PhysX 3.3
* FBX SDK 2015.1

## Windows

```
1. Download and install the latest Qt 5.x (open-source) distribution
2. Create a new environment variable "INTR_QTDIR" pointing to "[...]\Qt5.7\5.7\msvc2015_64"

3. Get access to the latest PhysX SDK from NVIDIA: https://developer.nvidia.com/physx-sdk
4. Follow the instructions from NVIDIA and compile the PhysX libraries for the configurations "Release", "Profile" and "Debug"
5. Download and install the latest Autodesk FBX SDK (2015.1): http://usa.autodesk.com/adsk/servlet/pc/item?siteID=123112&id=10775847
5. Create a new directory called "Intrinsic_Dependencies" on the same level as the Intrinsic repository folder
6. Inside, create a new folder "dependencies" containing two folders "physx" and "fbx"
7. Copy the static/dynamic libraries and header files of both SDKs to folders named "bin" (DLLs), "lib" (LIBs) and "include" respectively

8. Go to the "scripts_win32" folder in the Intrinsic repository dir
9. Execute "ConfigAndBuildDependencies.bat" to build some of the remaining dependencies automatically
10. Execute "CopyDllsToAppDir_Debug.bat" and "CopyDllsToAppDir_Release.bat"
11. Execute "Config.bat" to create a Visual Studio 2015 solution file and all project configurations

12. If everything went well, you'll find the solution in the newly created "build" folder. You can also use one of the many build scripts: "Build_Release.bat", ... to get started
13. Execute "Intrinsic.exe" or "IntrinsicEd.exe" in the "app" directory - yey!
```

## Linux

Coming soon...

## Android

IntrinsicEd is neither configured for nor tested with Android - but the support is planned for the future.

# License

 Intrinsic
 Copyright (c) 2016 Benjamin Glatzel

 This program is free software : you can redistribute it and / or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.

 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU General Public License for more details.

 You should have received a copy of the GNU General Public License
 along with this program. If not, see <http://www.gnu.org/licenses/>.

# Credits

Intrinsic uses the following open-source libraries:

* Vulkan SDK (see https://lunarg.com/vulkan-sdk/)
* microprofile (https://github.com/jonasmr/microprofile)
* enkiTS (see https://github.com/dougbinks/enkiTS)
* gli (see http://gli.g-truc.net/0.8.1/index.html)
* glm (see http://glm.g-truc.net/0.9.8/index.html)
* glslang (see https://github.com/KhronosGroup/glslang)
* LuaJIT (see http://luajit.org/)
* rapidjson (see https://github.com/miloyip/rapidjson)
* rlutil (see https://github.com/tapio/rlutil)
* SDL 2.0 (see https://www.libsdl.org/download-2.0.php)
* SOL v2.0 (see https://github.com/ThePhD/sol2)
* sparsepp (see https://github.com/greg7mdp/sparsepp)
* SPIRV-Cross (see https://github.com/KhronosGroup/SPIRV-Cross)
* tinydir (see https://github.com/cxong/tinydir)
* TLSF allocator (see https://github.com/mattconte/tlsf)

Intrinsic uses the following proprietary libraries:

* PhysX 3 (see https://developer.nvidia.com/physx-sdk)
* Qt (IntrinsicEd only, see https://www.qt.io/download)
* FBX SDK (IntrinsicEd only, see http://usa.autodesk.com/adsk/servlet/pc/item?siteID=123112&id=10775847)

Intrinsic also uses the following tools in binary format:

* NVTT (see https://developer.nvidia.com/gpu-accelerated-texture-compression)
* Cloc (see http://cloc.sourceforge.net)
* 7za (see http://www.7-zip.org/download.html)
