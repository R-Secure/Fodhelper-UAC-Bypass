# Fodhelper-UAC-Bypass
C# implementation of the Fodhelper UAC bypass. As mentioned in s3cur3th1ssh1t's blogpost (https://s3cur3th1ssh1t.github.io/Signature_vs_Behaviour/) Defender does not like any .exe in the HKCU:\Software\Classes\ms-settings\Shell\Open\command(Default) entry. 

We don't need to specify .exe to execute a binary, but running unsigned executables is not really good practice. We can copy rundll to a writable location and execute it from there.

### Usage:
```
Fodhelper-UAC-Bypass.exe "C:\Windows\Temp\payload.dll,DllMain"
```
