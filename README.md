# Comet Executor
A professional-grade Roblox script executor featuring a modern WPF interface and syscall-based injection.

## Features
- **Modern UI**: Smooth WPF interface with Gaussian blur, starfield animations, and rhythmic comet effects.
- **Advanced Editor**: Integrated AvalonEdit with Lua/Luau syntax highlighting.
- **Syscall Injection**: High-performance execution core (`Gargamel.dll`) using direct syscalls for stability.
- **Script Hub**: Easily manage, save, and execute your favorite scripts from a dedicated tab.
- **Auto-Attach**: Automatically detects and links to active Roblox processes.
- **Real-time Monitoring**: Track client status, UserID, PlaceID, and job details directly in the UI.
- **Built-in Utilities**: Quick access to "Kill Roblox" and a toggleable debug console.
- **Auto-Updates**: Integrated version checking to ensure you're always on the latest build.

## Installation
1. Download the latest release from the [Releases](https://github.com/OkaySleepy/Comet-Executor/releases) page.
2. Extract the contents to a folder. Ensure `Gargamel.dll` and `Comet Executor.exe` are in the same directory.
3. Launch `Comet Executor.exe`.
4. (Optional) Place your `.lua` or `.txt` scripts in the `/Scripts` folder to see them in the Script Hub.

## Usage
### Buttons
- **Attach**: Injects the core into the Roblox process.
- **Execute**: Runs the script currently in the editor.
- **Clear**: Wipes the editor content.
- **Save**: Saves the current script to the `/Scripts` folder.
- **Open**: Opens the `/Scripts` folder in File Explorer.
- **Kill Roblox**: Immediately terminates all Roblox processes.

### Navigation
- **Editor**: Your primary workspace for writing and running scripts.
- **Script Hub**: A gallery of your saved scripts for quick execution.
- **Clients**: View details about the currently attached Roblox session.
- **Settings**: Adjust UI preferences and view version info.
- **Discord**: Join our community for support and updates.

## Building from Source
### Prerequisites
- **C++ Core**: [CMake 3.10+](https://cmake.org/), Visual Studio (MSVC), MASM (Macro Assembler).
- **C# UI**: [.NET SDK](https://dotnet.microsoft.com/), Visual Studio (WPF Desktop Development).
- **Java**: Not required for this project (unlike the Minecraft mod example).

### C++ Core (Gargamel.dll)
```powershell
mkdir build
cd build
cmake ..
cmake --build . --config Release
```
Output: `build/Release/Gargamel.dll`

### C# UI (Comet Executor.exe)
1. Open `RblxExecutorUI.csproj` in Visual Studio.
2. Restore NuGet packages (AvalonEdit).
3. Build the solution in `Release` mode.
4. Copy the compiled `Gargamel.dll` into the output folder.

## Compatibility
- **OS**: Windows 10/11 (x64)
- **Game**: Roblox (WinInet/WinHttp required)
- **Framework**: .NET Framework 4.7.2+ or .NET 6/7/8 WPF

## License
MIT License
