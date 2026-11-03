# Operating system config

Display Settings 
Monitor Turn-Off Timeout (-monitor-timeout-ac) 30 Minutes 
Prevents the display from going dark too quickly during active administrative tasks while saving energy when idle.

Power Settings 
Active Power Scheme & Standby (-setactive) High Performance (Sleep disabled: 0)
Eliminates CPU throttling and prevents the remote server from entering sleep mode, ensuring 24/7 service availability.

Accessibility 
Sticky Keys Shortcut (StickyKeys\Flags) 
Prevents accidental activation of accessibility prompts during rapid keyboard typing in remote terminal sessions.

# make a account

The first thing I was to ssh to the server and use the command net to create a user.

# installing software =

First I try using winget but the command isn't working so instead i choose to install scoop. using the command

```powershell
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser

//this if you are on admin on powershell

irm get.scoop.sh | iex
//if you are not a admin on powershell
iex "& {$(irm get.scoop.sh)} -RunAsAdmin"
```

the first thing i did was install git using

scoop install git

than after git choose to make a bucket
scoop bucket add extras

than we install the software we want
scoop install vscode
scoop install firefox
scoop install 7zip
