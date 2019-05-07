# STK500V2 bootloader

To build:<BR>
```make squeeky && make working```

## BUGFIXES
* Reformatted strange tabbing to actual terminal standards, tab == 8 spaces. Yes, I consider poor formatting a bug.
* Broken monitor mode on MCU with >64KB flash.
* APP arena end was incorrectly set. 
* On MCU with >64KB flash, you couldn't erase the last 8KB of app arena. 
* On MCU with <=64KB flash, you couldn't erase the last 2KB of app arena. 

## New feature
Ability for sketch to write to app arena. Library to be uploaded soon.
