---
title: Frequently Asked Questions
layout: default
filename: faq
--- 


## Frequently Asked Questions (FAQs)
### Why does the app crash for no reason?
If the app is crashing, please email the log.txt, config.json, device information (such as device model and screen resolution) to the developer (JPTGamesAndApps@Outlook.Com) with steps to reproduce the crash.

### I ran the app, but the drives do not show up, and clicking libraries load empty folders only. What's wrong?
Make sure that the Windows 10 File Access permission is granted for Shrestha Files. You can either go to
```Windows 10(X) Settings -> Privacy -> File System -> Toggle On File Access for Shrestha Files.```
OR
```Shrestha Files Settings (Gear Icon) -> File Access Permission -> Toggle On File Access for Shrestha Files.```
Once toggled, Shrestha files will close automatically. Launch Shrestha Files again!

### Where is the config file located?
By default, the config.json file should be located in the folder location similar to the one shown below. Replace <UserName> with the actual user name. 
  
```C:\Users\<UserName>\AppData\Local\Packages\43158JPTGamesandApps.ShresthaFiles-AModernDualPane_pnxmbr0ydfejr\LocalState ``` 
  
The AppData is a hidden folder and is not visible from Shrestha Files, but if you type the path, it should be able to show the contents inside. Alternately, you can click the 
  
```Open Application Folder ``` 
  icon on the top right side of the 
```Log Viewer``` 

to load the folder.


### Where is log file stored?
Log file (log.txt) is stored in 

```C:\Users\<UserName>\AppData\Local\Packages\43158JPTGamesandApps.ShresthaFiles-AModernDualPane_pnxmbr0ydfejr\TempState ``` 

Alternately, click on the ```Log Viewer``` -> ```Open Full Log``` to open log file in a text viewer (such as the Notepad).


### All my tabs and bookmarks are gone after updating the app. Can I recover them?
The tabs, bookmarks, and other settings are stored in config.json file. Sometimes newer version of config file is not compatible with older version of config. When newer versions are installed, the app attempts to update the config file. Sometimes this process might fail, and the config file may be reset. In such cases, you can try to recover tabs, bookmarks, and other settings from backed up config file(s). The LocalState folder will may have other versions of config file such as config.failed.json that was saved when the app failed to read the previous config.json the last time. Similary, config.prior.json should have the version from the last version of the app. config.successful.json stores the last config file that was read successfully. More back ups are stored in the temporary location ```C:\Users\<UserName>\AppData\Local\Packages\43158JPTGamesandApps.ShresthaFiles-AModernDualPane_pnxmbr0ydfejr\LocalCache\Backups``` folder. The contents in this temporary location is deleted by Windows 10 automatically.


### App Crashed at Launch after Updating to a Newer Version, What can I do?
Sometimes the config file (that stores the settings for the app) changes in the newer version. While attempts are made to upgrade the config files automatically, sometimes such process fails and can crash the app. In such case, you might need to rename or move the config.json and its versions in the LocalState folder. Launch the app again and save settings (Ctrl+S) and a new config.json will be created. You can manually import desired previus settings from the existing config files that you just moved or renamed.

### I edited the config.json, but nothing changed. Did I do something wrong?
Make sure the app was *not* running when you edited and saved the config.json file. The application saves the config.json when closing the app. If you edited the config.json when the application was running, it will be overridden by the values in the memory. Thus, make sure the app is closed while editing the config.json. Then save the config.json, and launch the app afterwards.


### I edited the config.json. Now I lost all my tabs and bookmarks. What happened?
If the config.json is edited improperly, the app will fail to read the config.json. In such case, the app will try to read previous version of config.json. If that fails as well, it will rest the settings. The app attempts to back up config files that it failed to read and it should be stored in the App folder.

  
### Shrestha Files does not show shortcuts, hidden files, and system files, why?
UWP APIs have platform limitations that do not allow accessing some files such as shortcut (.url, .lnk, etc.), hidden files, and system files. Microsoft needs to allow access to such files before Shrestha Files is able to show such files. From one side, this is a limitation for the app. From another side, this could be better option if users would like to make sure they are not manipulating hidden and/or system files.
  
  
### Shrestha Files failed to open some files, why?
Some files such as .exe and .bat are considered risky by Microsoft. As such, the UWP APIs cannot launch such files.

  
### I would like to access my network locations quicker. Is there any way to do so?
There are two potential methods to ease accessing network locations. 
1. Type the location (e.g. "\\share\foldername") in the path and navigate to the folder. Now bookmark the path (Ctrl + D) or right click and Pin to Navigation Bar. 
2. Map the location as a drive from Windows File Explorer. The path will now show up in the list of drives in Shrestha Files!

  
### Shrestha Files takes a split second extra time to load the files and folders when compared to Windows File Explorers and other classic (win32) file managers, why?
The UWP apps need to access files and folders through a runtime broker provided by Microsoft instead of accessing the files and folders directly. This runtime broker is slower than more direct access (that is used by win32 apps). Microsoft is working to improve the file access speed in the Project Reunion. Once Microsoft completes the project, the tab loading speed will improve further. Meanwhile the developer is working to improve the tab loading speed using the existing APIs as much as practical and possible.

  
### What is the difference between the Pro and Free version?
The pro version is updated more often than the Free version. Some features are available only in the Pro version. The free version also shows a prompt requesting to consider purchasing a pro version every time the Free version is launched. Users' support is essential to continue improving the app further. This includes sharing the apps to others, providing feedback, sending bug information, requesting new features, and purchasing the pro version. While all feature requests cannot be fulfilled, the developer will attempt to fulfill features that are requested by more users and that requires less effort to implement.

