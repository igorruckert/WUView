# WUView

### Introduction

Windows Update Viewer (WUView) is an application that displays information about Windows Updates. WUView uses the Windows Update API and Windows event logs to display details of installed updates. Event log entries are associated with individual updates by using the "KB" number. If an update does not use a KB number, or it isn't presented in a consistent format, no event log entries will be displayed.

### Oddities

Several updates on my machines show the HResult code 0x80242014 even though the Windows Update History shows that the updates were successfully installed. 0x80242014 translates to WU_E_UH_POSTREBOOTSTILLPENDING "The post-reboot operation for the update is still in progress."  This persists over multiple reboots.