# Keylogger Application

## Problem Statement

Design a keylogger.

## Overview

Keylogger app is a C++ application that has basic functionalities of key logging software. Three primary goals of this app are:

1. Execute in hidden mode in background.
2. Detect and capture Keystrokes.
3. Save keystrokes log in a text file.

## Description

This keylogger supports the following characters and symbols:

```
`1234567890-=
~!@#$%^&*()_+
qwertyuiop[]\asdfghjkl;'zxcvbnm,./
QWERTYUIOP{}|ASDFGHJKL:"ZXCVBNM<>?
[TAB][C0][C1][SHIFT][LCTRL][LWIN][LALT][SPACE][RALT][RWIN][MENU][RCTRL][ENTER][BACK]
[DEL][INS][END][HOME][PGDN][PGUP][ARROWD][ARROWU][ARROWL][ARROWR]
```

## Technology used

- C++

## Resources Used

- [GetAsyncKeyState function](https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-getasynckeystate)
- [Virtual-Key Codes](https://docs.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes)

## How to Run Keylogger [Using an IDE]

1. Clone this repository from GitHub: $ https://github.com/PERCY99/KeyLogger

2. Open _keylogger.cpp_ and change the maximum number of key strokes you wish to record (_max_ constant)
3. Compile with MinGW: g++ keylogger.cpp -o keylogger.exe
4. Run _keylogger.exe_
5. The program will terminate after a certain number(_max_ constant) of key strokes.
6. Inspect _Record.txt_


## Output

_Record.txt_ output:

![log-output output](output.png)