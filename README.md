# Juicy-Potato-x86
Juicy Potato for x86 Windows

This is a version of [ohpe's Juicy Potato][1] privilege escalation exploit modified for x86 Windows. I preserved as much of the code as I could, while making changes necessary to compile for x86 Windows. Tested successfully on Windows 7 SP1 x86 Build 7601.

Edit/compile it with Visual Studio 2017 (v141) toolset.

### Example usage

```
"Juicy Potato x86.exe" -l 4444 -p c:\windows\system32\cmd.exe -t * -c {6d18ad12-bde3-4393-b311-099c346e6df9}
```
[1]: https://github.com/ohpe/juicy-potato 
