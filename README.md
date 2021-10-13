# AutoRefreshRate

Changes the refresh rate depending on whether the computer is plugged in or not to save battery.

My laptop supports 60Hz and 240Hz, these values must be changed according to your screen.

# Scheduling

To automate the change, use the Task Scheduler.
Create a new task, trigger it on this event:   
- Log: System   
- Source: Kernel-Power   
  
For the action, simply run AutoRefreshRate.exe.

# Documentation

- [GetSystemPowerStatus function (winbase.h)](https://docs.microsoft.com/en-us/windows/win32/api/winbase/nf-winbase-getsystempowerstatus)   
- [SYSTEM_POWER_STATUS structure (winbase.h)](https://docs.microsoft.com/en-us/windows/win32/api/winbase/ns-winbase-system_power_status)   
- [EnumDisplaySettingsA function (winuser.h)](https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-enumdisplaysettingsa)   
- [ChangeDisplaySettingsExA function (winuser.h)](https://docs.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-changedisplaysettingsexa)   
