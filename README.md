# Execute Program Libraries
A library for execute program.

## Usage

```cpp
#include "Shell.h"
using namespace Easy;

CString sProgram = _T("C:\\Windows\\system32\\cmd.exe");
CString sArgv = _T("/c date /t");

Shell shell;
shell.Execute(sProgram, sArgv, Shell::CONSOLE);
while(shell.IsRunning()) Sleep(100);
shell.GetOutput(); // 2020/06/23 Thu 

```
