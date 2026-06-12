⚡ ZigIDE Professional – A Professional IDE for Zig
ZigIDE Professional is a lightweight, open source, cross platform Integrated Development Environment (IDE) written in Python with Tkinter, specifically designed for programming in the Zig language. It provides code editing, execution, project management, theme switching, search & replace, and seamless integration with Zig tools – all in a simple, user friendly interface.
✨ Key Features
•	🖊 Multi line editor with basic syntax highlighting (extensible)
•	🎨 Dark / Light theme toggle with one click
•	🗂 File management: New, Open, Save, Save As (.zig files)
•	▶ Run Zig code directly using your installed Zig compiler
•	🔍 Find & Replace inside the editor (with highlight of search results)
•	🔎 Text zoom (Ctrl+Plus / Ctrl+Minus / Ctrl+0)
•	🧰 Quick toolbar and status bar (shows Zig path, cursor position, active theme)
•	📂 Output panel – show / hide as needed
•	⌨ Standard keyboard shortcuts (Ctrl+S, Ctrl+F, Ctrl+Z, etc.)
•	🔁 Unsaved changes warning before closing a file
•	⚙ Automatic settings persistence (last theme, zoom level, window geometry)
•	🔌 Change Zig path on the fly (no restart required)

📥 Installation & Setup
Prerequisites
•	Python 3.7 or higher (optional if you use a packaged executable)
•	Zig compiler
Download Zig and install it. Remember the folder containing zig (or zig.exe).
Note: On first launch, a dialog will ask you to select the folder where Zig is installed. This is a one time setup.
🚀 User Guide
1. Main Interface
•	Toolbar (top): New, Open, Save, Run, Theme buttons.
•	Editor panel (main area): write your Zig code.
•	Output panel (bottom): shows program output or compilation errors.
•	Status bar (bottom): Zig path, cursor position (line/column), active theme.
2. Menus & Keyboard Shortcuts
Menu	Item	Shortcut	Description
File	New	Ctrl+N	Create a new file
	Open	Ctrl+O	Open an existing .zig file
	Save	Ctrl+S	Save current file
	Save As	Ctrl+Shift+S	Save with a new name
	Exit	Ctrl+Q	Quit the application
Edit	Undo	Ctrl+Z	Undo last change
	Redo	Ctrl+Y	Redo undone change
	Cut / Copy / Paste	Ctrl+X/C/V	Clipboard operations
	Find	Ctrl+F	Search text in editor
	Replace	Ctrl+H	Replace text
View	Zoom In	Ctrl+Plus	Increase editor font size
	Zoom Out	Ctrl+Minus	Decrease editor font size
	Reset Zoom	Ctrl+0	Restore default font size
	Toggle Theme	(no shortcut)	Switch between dark and light themes
	Toggle Output Panel	(no shortcut)	Show / hide the output panel
Window	License → Select Zig	(no shortcut)	Change Zig installation path (useful after Zig update)
	License → View License		Display the MIT license
	Preferences	(no shortcut)	Settings (e.g., font size)
Help	Documentation		Open Zig documentation in your browser
	About		Version and credits
3. Running Zig Code
•	Write your Zig code in the editor.
•	Click the ▶ Run button on the toolbar.
•	The output (stdout / stderr) appears in the output panel.
4. Switching Themes (Dark/Light)
•	Click the 🌓 Theme button on the toolbar, or use View → Toggle Theme.
The current theme is shown in the status bar.
5. Find & Replace
•	Ctrl+F : opens a search dialog. Enter a string – all matches are highlighted in yellow.
•	Ctrl+H : opens replace dialog. Enter search string and replacement.
6. Zooming
•	Ctrl+Plus : zoom in
•	Ctrl+Minus : zoom out
•	Ctrl+0 : reset zoom
Zoom level is saved between sessions.
7. File Handling
•	Settings (window size, theme, zoom) are automatically stored in ~/.zig_ide_config.json.
•	When closing a file or the application, you will be prompted if there are unsaved changes.
Project Structure (for developers)
zigide-professional/
├── zigide.py           # Main application file
├── README.md           # This file
├── LICENSE             # Custom open source license (see text below)
└── .gitignore
The zigide.py file contains:
• The ZigIDE class (UI and logic)
• Helper functions: load_config, save_config, validate_zig_path, select_zig_folder
• Event handling, keyboard shortcuts, and Zig integration
🛠 Contributing
Contributions are very welcome! You can help by:
• Reporting bugs: Open an issue
• Suggesting features: Discuss your idea in the Issues section.
• Submitting pull requests:
1.	Fork the repository
2.	Create a feature branch (git checkout -b feature/amazing-feature)
3.	Commit your changes (git commit -m 'Add some amazing feature')
4.	Push to the branch (git push origin feature/amazing-feature)
5.	Open a Pull Request
Ideas for future improvements
• Full syntax highlighting (using pygments or tree sitter)
• Multi file project support (workspace)
• Integrated debugger (via lldb or gdb)
• Built in terminal
• Code autocompletion using ZLS (Zig Language Server)
• Polyglot support (run Python, C, C++ snippets alongside Zig)
📜 License
This project is open source and free for public use under the 
GNU General Public License version 3 (GPL v3).

Copyright © 2025 M. Azizian. All rights reserved.

You may:
- Use, copy, and distribute this software freely
- Modify the source code
- Use it for commercial purposes

You MUST:
- Keep the original copyright notice (M. Azizian)
- Release your modified versions under GPL v3 as well
- Make your modified source code available to users

You may NOT:
- Incorporate this code into proprietary (closed-source) software
- Change the license to a more restrictive one

The software is provided "AS IS", without any warranty. 
The author (M. Azizian) assumes no liability for any damages 
arising from its use.

See the LICENSE file for the full GPL v3 license text.
🌟 Acknowledgements
•	The Zig team for their fast and powerful compiler.
•	The Python and Tkinter communities for simple, cross platform GUI tools.

📞 Contact
•	Email: aziziyan1364@gmail.com
•	GitHub: @MA1364


