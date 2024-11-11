PRODIGY_CS_04
Simple Keylogger in C++
Overview
This is a basic keylogger application written in C++ for educational purposes. It captures and logs keystrokes from the keyboard to a file (keylog.txt) while running in the background. The application logs both standard characters and special keys like Shift, Ctrl, Enter, etc.

Features
Logs standard keys (A-Z, 0-9, symbols).
Logs special keys like Shift, Ctrl, Enter, Tab, etc.
Saves the logged data into a file (keylog.txt).
Disclaimer
This keylogger is intended for educational purposes only. Logging keystrokes without explicit permission from the user is illegal and unethical. Ensure you have proper authorization before using this program.

How It Works
The program captures keyboard input using the Windows API (GetAsyncKeyState) to detect keypresses. Each keypress is logged to a file (keylog.txt) in the program's working directory.

Prerequisites
Windows operating system (since the program uses Windows-specific API functions).
C++ compiler (such as g++ or Visual Studio).
Compilation and Execution
Step 1: Compilation
To compile this C++ program, you can use any C++ compiler. Below are a couple of options:

Using g++:
Install MinGW (for Windows) or any other g++ compiler.

Compile the program using the following command in the terminal:

g++ keylogger.cpp -o keylogger.exe
Using Visual Studio:
Open the project in Visual Studio.
Build the project by pressing Ctrl + Shift + B or selecting Build from the menu.
Step 2: Run the Program
After compilation, you can run the program:

keylogger.exe
Once the program starts, it will capture all keystrokes and log them to keylog.txt in the same directory as the executable.

Key Mappings
The program logs standard characters directly and replaces special keys with meaningful labels like:

[SHIFT]
[CTRL]
[ENTER]
[TAB]
[ESCAPE]
[BACKSPACE]
Example
If the user types:

Hello World!
The log file (keylog.txt) would contain something like:

Hello[SPACE]World[SHIFT]![ENTER]
License
This project is released under the MIT License. Feel free to use, modify, and distribute the code, but make sure to respect local laws and ethical guidelines regarding keylogging.

How to Use
Ensure you have permission before running the program on any machine.
Modify the code or adjust settings as necessary for your specific use case.
Further Development
You can expand the keylogger's functionality by:

Hiding the console window to make it run silently in the background.
Adding features like date and time logging for each keystroke.
Extending it to log mouse events or system states.
