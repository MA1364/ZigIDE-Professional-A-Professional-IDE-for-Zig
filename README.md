
⬡ ZigMA IDE v1.0.0
Professional Zig Development Environment for Windows

🚀 Quick Installation
Prerequisites
Python 3.8+ (with tcl/tk enabled - default on Windows)

Internet connection (for Zig SDK download)

Installation Methods
Method 1 - Direct execution:

text
python zigforge.py
Method 2 - Windows full install:

powershell
powershell -ExecutionPolicy Bypass -File install_windows.ps1
Method 3 - Batch launcher:

text
launch_zigforge.bat
✨ Features
🔥 Code Editor
Full Syntax Highlighting for Zig

Line numbers and minimap

Smart Auto-indent (block detection)

Tab completion with 4 spaces

Unlimited Undo/Redo

Toggle Comment (Ctrl+/)

Cascadia Code font (monospace)

Multiple tabs with change indicators

📦 SDK & Package Manager
Download all Zig versions from ziglang.org

Automatic installation and extraction

Manage multiple Zig versions simultaneously

Switch active version

List of popular packages with direct links

Add packages to build.zig.zon

🗂️ Project Management
File Tree Explorer with icons

Create new project (zig init)

Support for exe / lib / shared-lib

Outline view (functions and variables)

Search across all project files

⚡ Integrated Terminal
Built-in terminal with command history

Colorized output (error/warning/success)

cd and directory navigation support

Kill process when needed

🔥 Zig Commands
Key	Action
F5	zig build
F6	zig run <file> or zig build run
F7	zig test
Ctrl+S	Save
Ctrl+N	New file
Ctrl+O	Open file
Ctrl+F	Search
Ctrl+H	Replace
Ctrl+/	Comment/Uncomment
🎨 Appearance
ZigDark theme (dark - default)

ZigLight theme (light)

Font resizing (Ctrl++ / Ctrl+-)

Accent color from official Zig logo (golden ⬡)

🔧 Integration with Other Languages
ZigForge supports integration of Zig with other languages:

C/C++
zig
const c = @cImport({
    @cInclude("stdio.h");
});
pub fn main() void {
    c.printf("Hello from C!\n");
}
In the terminal:

text
zig build-exe main.zig -lc
Python (via ctypes)
python
import ctypes
lib = ctypes.CDLL("./mylib.dll")  # Library built with zig
lib.my_function.restype = ctypes.c_int
Creating DLL with Zig
zig
export fn add(a: i32, b: i32) i32 {
    return a + b;
}
text
zig build-lib mylib.zig -dynamic
📁 Suggested Project Structure
text
my-project/
├── build.zig          # Build script
├── build.zig.zon      # Package manifest
├── src/
│   ├── main.zig       # Entry point
│   ├── lib.zig        # Library code
│   └── ...
├── tests/
│   └── test_main.zig
└── README.md
⚙️ Configuration
Settings are saved in ~/.zigforge/settings.json:

json
{
  "theme": "ZigDark",
  "font_size": 12,
  "zig_path": "C:/Users/you/zig/zig-0.13.0/zig.exe"
}
🐛 Troubleshooting
tkinter not found error:

Reinstall Python and enable the "tcl/tk and IDLE" option

zig not found error:

Use the SDK Manager menu or manually set the path to zig.exe

PowerShell installation error:

powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
🗺️ Future Roadmap
Language Server Protocol (ZLS)

Integrated Debugger (DAP)

Git Integration

Code Snippets

Advanced Autocomplete

Extension API

More Project Templates
