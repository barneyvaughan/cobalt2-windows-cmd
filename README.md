# Cobalt2 for Windows Command Line

A registry file to use the Cobalt2 color scheme in the Windows Command Line. Also changes Bash for Ubuntu for Windows!

## Installation

Download `cobalt2.reg` to anywhere on your file system. Double click and a voila, pretty colors inside your Windows command line.

## Example 

![Command line showing Cobalt2 color scheme](https://i.imgur.com/xOkyQ5f.jpg)

## FAQ

**Q: Help! I ran the registry file, but whenever I hit `Windows` and type _cmd_ I still get the default colors! is it not working?**

A: Turns out the shortcut in Windows is caching the old variables. An easy fix is to delete the shortcut for _Command Prompt_ under `%APPDATA%\Microsoft\Windows\Start Menu\Programs\System Tools` and remake a similar one from _cmd.exe_ under `C:\WINDOWS\system32`.

After that you should no longer be getting the old color scheme in command prompt.

**Q: Help! I ran the registry file, but whenever I hit `Windows` and type _bash_ I still get the default colors! is it not working?**

A: Same as the answer above! Some of the options are a little different though.

Remove the file _Bash on Ubuntu on Windows_ from `%APPDATA%\Microsoft\Windows\Start Menu\Programs` and remake a similar one from _bash.exe_ under `C:\WINDOWS\system32`.

Then change the properties of the link to the following options:
- **Target**: `C:\WINDOWS\system32\bash.exe ~`
- **Start in**: <leave this one blank>
- **Comment**: `Shortcut to bash.exe`

If you want the icon back click _Change Icon..._ and set the target to `%USERPROFILE%\AppData\Local\lxss\bash.ico`.

That should do it, good as new!

**Q: I want the old colors back!**

A: Under the Attribution [P4](https://gist.github.com/P4) has made some other [Color schemes for Windows Command Prompt](https://gist.github.com/P4/4245793). It also has the defaults, run that and it should be fine.

## Attribution

Original theme [Cobalt2](https://github.com/wesbos/cobalt2) by [@wesbos](https://twitter.com/wesbos)  
Code based on [Color schemes for Windows Command Prompt](https://gist.github.com/P4/4245793) by [P4](https://gist.github.com/P4)