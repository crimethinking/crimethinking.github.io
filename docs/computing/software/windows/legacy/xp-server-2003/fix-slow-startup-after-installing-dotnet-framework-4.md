# Fix slow startup after installing .NET Framework 4
I noticed that my XP installation booted very slowly after installing .NET Framework 4.
After logging in, everything (including networking) hung for about 90-120 seconds before
startup entries and networking got started

[Thanks to shorterxp on MSFN for the original tip](https://msfn.org/board/topic/178206-slow-logon-bug-caused-by-net-framework-ngen-how-to-fix/)

* Install .NET Framework 4 and all updates including those for other .NET Framework versions
* Execute `C:\WINDOWS\Microsoft.NET\Framework(64)\<version>\ngen.exe executeQueuedItems`
to compile native images for .NET assemblies (4 on my installation, for .NET Framework 2 and 4
in `amd64` and `x86`)
* Stop and disable all `.NET Framework NGEN` services (4 on my installation)