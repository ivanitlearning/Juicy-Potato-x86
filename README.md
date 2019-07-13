# Juicy-Potato-x86
Juicy Potato for x86 Windows

This is a version of [ohpe's Juicy Potato][1] privilege escalation exploit modified for x86 Windows. I preserved as much of the code as I could, while making small changes necessary to compile for x86 Windows. Tested successfully on Windows 7 SP1 x86 Build 7601.

Edit/compile it with Visual Studio 2017 (v141) toolset. Use at your own peril.
More [explanation here][2] on how to use it and how it works.

P.S. I'm new to Github so forgive me if it looks awkward.

### Example usage

```
"Juicy Potato x86.exe" -l 4444 -p c:\windows\system32\cmd.exe -t * -c {6d18ad12-bde3-4393-b311-099c346e6df9}
```
![How to use](https://github.com/ivanitlearning/Juicy-Potato-x86/blob/master/JuicyPotato.png)


### Stuff to figure out
I had to comment out this line in `JuicyPotato x86.cpp` for it to work. It works without it but I'm uncertain of its significance.
```
si.lpDesktop = L"winsta0\\default";
```

[1]: https://github.com/ohpe/juicy-potato
[2]: https://hunter2.gitbook.io/darthsidious/privilege-escalation/juicy-potato
