# Use Consolas as Windows console font
[Thanks to Scott Hanselman for the original tip](https://hanselman.com/blog/using-consolas-as-the-windows-console-font)

!!! note "ConEmu Unicode support"
    This is [prerequisite for showing Unicode characters with ConEmu](https://conemu.github.io/en/UnicodeSupport.html#Check_if_is_capable_to_accept_unicode)

* Install Consolas font; get it yourself somehow, somewhere
* Save the following code block as a `.reg` registry key and import it
``` registry
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Console\TrueTypeFont]
"00"="Consolas"
```
* Reboot