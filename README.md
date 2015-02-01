# .Net4-to-4.5-64bit-batch
This script uninstalls .net4 and installs .net 4.5 in a Windows 64 bit enviroment with a three minute pause after the uninstall.

%windir%\Microsoft.NET\Framework64\v4.0.30319\SetupCache\Extended\setup.exe /uninstall /x86 /x64 /ia64 /parameterfolder Extended /passive /norestart

SLEEP 240

%windir%\Microsoft.NET\Framework64\v4.0.30319\SetupCache\setup.exe /repair /x86 /x64 /ia64 /q /norestart
