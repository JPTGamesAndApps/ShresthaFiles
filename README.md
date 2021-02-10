## Shrestha Files

If you like file managers such as Q-dir, Directory Opus, Total Commander, xplorer2, and XYplorer because they offer tabs and multiple panes but do not like the classic Windows 32 style interface or your Windows 10X device does not support them, then Shrestha Files might be what you are looking for. It offers the convenience of tabs and dual pane in a modern and minimalist interface to supercharge your productivity. [Download it from the Microsoft Store Now](https://www.microsoft.com/en-us/p/shrestha-files/9npnffsv2hqm).

### Screenshots

Light Mode | Dark Mode
---------- | ----------
![Single Pane Light](/images/SingleLight.png) | ![Single Pane Dark](/images/SingleDark.png)
![Dual Pane Light](/images/DualLight.png) | ![Dual Pane Light](/images/DualDark.png)

### Keyboard Shortcuts
* F1 - About dialog
* F2 - Rename file/folder
* F3 - Open file/folder
* F4 - Open with
* Ctrl+A - Select All
* Ctrl+B - Edit Navigation Bar Items
* Ctrl+C - Copy Files/Folders
* Ctrl+Shift+C - Copy Path
* Ctrl+D - Pin Current Folder in Navigation Bar
* Ctrl+N - Create New Folder
* Ctrl+Shift+N - Create New File
* Ctrl+R - Refresh
* Ctrl+S - (Manually) Save Settings (Settings are also saved automatically while closing the app)
* Ctrl+X - Cut
* Ctrl+V - Paste
* Delete - Delete
* Alt+Left - Go Back
* Alt+Right - Go Forward
* Alt+Up - Go Up

### Tips and Tricks
* You can double click on empty area in any tab to navigation to the parent directory (go up a level).
* You can right click any navigation bar item to open the path in a new tab or delete the item.
* Some settings are currently only accessible from config.json file in app directory.
* You can drag and drop files and folders from inside one tab to inside another tab or inside the folder listed in the tab.
* Detailed log are stored in the log.txt in LocalCache directory. If the app crashes, you can email the log and steps to reproduce the crash to the developer so that it can be fixed.


### Chanegelog
**Changelog for Version 0.34.x (February 12, 2021)**
* Updated sizes for this PC (Home Page) items. Thanks to Chomu_ for feedback!
* When dragging and dropping items in the same folder, it does not copy/move items anymore. Thanks to Chomu_ for feedback!
* Initial implementation of back and forward button in mouse to navigation back and forward. Let the developer know if it still does not work.
* Improved change tracker when items are deleted from outside the app.
* Added translations in Chinese (Simplified), Czech, French, German, Hindi, Hungarian, Italian, Japanese, Korean, Russian, Spaish, and Turkish. The translations are based on Google Translation, so some of the translations could be confusing and/or misleading.
* Bug Fixed: Updated method to set panel background transparency in dual pane mode to fix the crash caused by the Layout Cycle bug.
* Other bug fixes.

**Changelog for Version 0.33.x (February 8, 2021)**
* Added update checker. Updates are checked every time Shrestha Files loads.
* Added single click mode in config file.
* Thanks to Parasec Glenkwyst for German (de-DE) Translation.
* Added translator names in About page.
* Bug fixes
* Note: If recent updated added repeated items (such as This PC) in the side bar, please remove the repeated once by right clicking on the item, and keep the first ones.

**Changelog for Version 0.32.x (February 6, 2021)**
* Automatically checks for an udpated version of the app in the store and prompts to install if newer version is available.
* Fixed crash while upgrading from older version (before v0.30 to later version)
* Fixed other bugs.

**Changelog for Version 0.31.x (February 5, 2021)**
* Fixed serious bug introduced while adding the translations. The bug resulted in the failure of all file operations. The developer apologizes for the serious bug.




### Privacy Policy
The app requires access to user File System to execute the apps core functionalities (as a file manager). Users can enable the file access from: ```Windows 10(X) Settings -> Privacy -> File System -> Toggle On File Access for Shrestha Files.```

Microsoft telemetry and App Center APIs in the app may collect information about the app crashes and usage for diagnostics and analytical purposes. A log file is generated to store logs such as errors, warnings, and other information. However, the file is not tranmitted outside the users device. Users can send the log for diagnostic purposes.

### Frequently Asked Questions (FAQs)
#### Keyboard Accelerators (Shortcuts) does not appear to work. What can I do?
Sometimes the keyboard accelerators does not work as expected. This is currently a known bug that will be fixed in the future. If the accelerator is not working, click at the empty space in one of the two panes once and the shortcuts should work. If it still does not work, please let the developer know.

#### I ran the app, but the drives do not show up, and clicking libraries load empty folders only. What's wrong?
Make sure that the Windows 10 File Access permission is granted for Shrestha Files. You can either go to
```Windows 10(X) Settings -> Privacy -> File System -> Toggle On File Access for Shrestha Files.```
OR
```Shrestha Files Settings (Gear Icon) -> File Access Permission -> Toggle On File Access for Shrestha Files.```
Once toggled, Shrestha files will close automatically. Launch Shrestha Files again!

#### Where is the config file located?
By default, the config.json file should be located in the folder location similar to the one shown below. Replace <UserName> with the actual user name. 
  
```C:\Users\<UserName>\AppData\Local\Packages\43158JPTGamesandApps.ShresthaFiles-AModernDualPane_pnxmbr0ydfejr\LocalState ``` 
  
The AppData is a hidden folder and is not visible from Shrestha Files, but if you type the path, it should be able to show the contents inside. Alternately, you can click the 
  
```Open Application Folder ``` 
  icon on the top right side of the 
```Log Viewer``` 

to load the folder.

#### All my tabs and bookmarks are gone after updating the app. Can I recover them?
The tabs, bookmarks, and other settings are stored in config.json file. Sometimes newer version of config file is not compatible with older version of config. When newer versions are installed, the app attempts to update the config file. Sometimes this process might fail, and the config file may be reset. In such cases, you can try to recover tabs, bookmarks, and other settings from backed up config file(s). The LocalState folder will may have other versions of config file such as config.failed.json that was saved when the app failed to read the previous config.json the last time. Similary, config.prior.json should have the version from the last version of the app. config.successful.json stores the last config file that was read successfully. More back ups are stored in the temporary location ```C:\Users\<UserName>\AppData\Local\Packages\43158JPTGamesandApps.ShresthaFiles-AModernDualPane_pnxmbr0ydfejr\LocalCache\Backups``` folder. The contents in this temporary location is deleted by Windows 10 automatically.


#### App Crashed at Launch after Updating to a Newer Version, What can I do?
Sometimes the config file (that stores the settings for the app) changes in the newer version. While attempts are made to upgrade the config files automatically, sometimes such process fails and can crash the app. In such case, you might need to rename or move the config.json and its versions in the LocalState folder. Launch the app again and save settings (Ctrl+S) and a new config.json will be created. You can manually import desired previus settings from the existing config files that you just moved or renamed.

#### I edited the config.json, but nothing changed. Did I do something wrong?
Make sure the app was not running when you edited and saved config.json. The application saves the config.json when closing the app. If you edited the config.json when the application was running, it will be overridden by the values in the memory. Thus, make sure the app is closed while editing the config.json. Then save the config.json, and launch the app afterwards.


#### I edited the config.json. Now I lost all my tabs and bookmarks. What happened?
If the config.json is edited improperly, the app will fail to read the config.json. In such case, the app will try to read previous version of config.json. If that fails as well, it will rest the settings.

#### Shrestha Files does not show shortcuts, hidden files, and system files, why?
UWP APIs have platform limitations that do not allow accessing some files such as shortcut (.url, .lnk, etc.), hidden files, and system files. Microsoft needs to allow access to such files before Shrestha Files is able to show such files.

#### Shrestha Files failed to open some files, why?
Some files such as .exe, .bat are considered risky by Microsoft. As such, the UWP APIs cannot launch such files.

#### Shrestha Files takes takes a split second extra time to load the files and folders when compared to Windows File Explorers and other classic (win32) file managers, why?
The UWP API needs to access files and folders through a runtime broker provided by Microsoft instead of accessing the files and folders directly. This runtime broker is slower than more direct access (that is used by win32 apps). Microsoft is working to improve the file access speed in Project Reunion. Once Microsoft completes the project, the tab loading speed will improve.

#### What is the difference between the Pro and Free version?
The pro verion is updated more often than Free version. Some features are available only in Pro version. The free version also shows a prompt requesting to consider purchasing a pro version every time the Free version is launched. Users support is essential to continue improving the app further. This includes providing feedback, sending bug information, requesting new features, and purchasing pro version. While all features requests cannot be fulfilled, the developer will attempt to fulfill features that are requested by more users and that are easier to implement.


### Note
This repo does not contain source code for Shrestha Files!
