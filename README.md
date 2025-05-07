# Unreal_Engine_Prerequisites
An Instruction to download Unreal Engine and related tools for C++ based development


### Visual Studio 2022
Below are required tools for Visual Studio 2022 to properly support Unreal Engine C++ development
#### .NET desktop development
#### Game development with C++
All default selected with the following:
- [x] Windows 11 SDK and/or any required Windows compatitable SDK depending on your machine and targeting platform
- [x] Visual Studio Tools for Unreal Engine
- [x] Unreal Engine Installer
- [x] Unreal Engine Test Adapter
#### Individual components
- [x] .NET 9.0 Runtime
- [x] .NET 9.0 WebAssembly Build Tools

Check this [link](https://learn.microsoft.com/en-us/visualstudio/gamedev/unreal/get-started/vs-tools-unreal-install)

#### VS Code
- [x] Update Code Editor in Unreal Engine/ Edit Preference to visualstudioCode
- [x] Perform Unreal Engine / Tools / Generate Visual Studio Code Project
- [x] Install VS Build Tools (should be included in Visual Studio 2022)
- [x] Instal VSCode Extensions:
  - [x] C/C++
  - [x] C/C++ Extension Pack
  - [x] C# Dev Kit

- [x] Add the below section into `c_cpp_properties.json`
```
"includePath": [ 
     "${workspaceFolder}\\Intermediate\\**", 
     "${workspaceFolder}\\Plugins\\**", 
     "${workspaceFolder}\\Source\\**" 
 ],
```

**Notes**:
- Compiler with VSCode seems to be really slow comparing to Visual Studio