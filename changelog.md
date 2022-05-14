---
title: Change Log History
layout: default
filename: changelog
--- 

## Change Log History
The latest "Free" version is version 2.0. "Pro X" versions are updated to the latest version posted here.

Some versions are relased gradually, meaning not everyone will get the latest version as soon as it is released. This is to ensure that if any unexpected bugs are introduced in the app resulting in crashes, the developer will get a chance to fix it before releasing it to all users.





**Changelog for Version 2.0 (2022 May)**

* Shrestha Files Pro X (version 2.0) is officially launching with Microsoft Build 2022! This version offers a significant performance improvements, new features, and customization options.





**Changelog for Version 1.77 (May 13, 2022)**

* Updated Italian translation, thanks to Alessandro!
* Updated German translation, thanks to Parasec!
* Updated Serbian translations, thanks to Bzzrak!





**Changelog for Version 1.76 (May 12, 2022)**

* Welcome to a brand-new version of Shrestha Files! This is a major update of Shrestha Files, and it brings a significant performance improvement by utilizing the latest windows platform developed for modern desktop apps. Most of the limitations of the previous version (e.g. not being able to run .exe files, show hidden and system files, etc.) are addressed in this version.
* Check out the full changelog from About Section of the settings to see numerous improvements made since the last major version of Shrestha Files Pro was released.
* Feel free to share this update with others and/or write a blog about it.



**Changelog for Version 1.75 (May 8, 2022)**

* More changes to ensure the Theme Settings does not crash.
* Miscellaneous improvements.



**Changelog for Version 1.74 (May 7, 2022)**

* Updated logo.
* Attempted to fix theme setting crash issue again.
* Miscellaneous improvements.



**Changelog for Version 1.73 (May 6, 2022)**

* Theme settings should load faster now.
* Various colorful font icons are used to indicate the type of files (e.g. text, picture, audio, video, or others).
* Version numbers bumped to 1.x instead of 0.x to indicate that this is a newer version of the app than the original Shrestha Files Pro. All the changelog documentations is also updated to reflect this.
* Miscellaneous improvements.



**Changelog for Version 1.72 (May 5, 2022)**

* Changes in the libraries bookmark will be saved again.
* Refined sizes of colorful font icons.
* Updated Hungarian translation. Thanks to Kristóf Kékesi!
* Updated Spanish translation. Thanks to Damián Roig!
* Miscellaneous improvements.



**Changelog for Version 1.71 (May 02, 2022)**

* Simple icon selection for bookmarks in the bookmark editor works now (shows a selection of simple glyph icons).
* Updated Spanish translation. Thanks to Damián Roig!
* Miscellaneous improvements.



**Changelog for Version 1.70 (April 30, 2022)**

* Drag and drop works again to drop items to a folder in a tab.
* Drag and drop works for tab headers as well, but requires moving the cursor a bit (outside the folder name text area).
* Added email link in about page. It was previously removed because it did not work.
* Can retain the simple glyph from Pro version while using the same config file for Pro X version. Users can copy the config.json file from Pro and paste it in the Pro X folder.
* Attempted to fix the Theme Settings crash. Not sure if the fix will solve the issue.
* Updated Chinese Simplified translation. (Thanks to Fairycn).
* Miscellaneous improvements.



**Changelog for Version 1.69 (April 28, 2022)**

* Additional shortcut "Space" to open the selected item with an internal viewer (if supported, otherwise it opens with an external viewer)
* Additional shortcut "Ctrl + Space" for Open With menu.
* "Ctrl + Shift + C" copies item path if an item is selected. Otherwise, it copies the tab path as before.
* Added shortcuts in This PC page context menu.
* Improved reliability of shortcuts.
* Navigation items are now called Bookmarks everywhere.
* Fixed again: Bookmarks Editor did not have semitransparent surrounding.
* Miscellaneous improvements.




**Changelog for Version 1.68 (April 26, 2022)**

* Background of disabled buttons set to transparent.
* Feedback heroes are added and recognized in the About page.
* Startup improvements.
* Miscellaneous improvements.
* [Fixed] Pictures and devices icon disappearing from the sidebar once bookmark editor was opened (in Simple Icon Mode).

* Pro features and enabled/disabled based on the purchase status. 
* List of Pro Only Features:
	- Theme:
		- System (Default) Theme
		- Colorful App Theme
		- Custom Background
		- Colorful Command (Button and Dropdown) Icons
		- Colorful Bookmark Icons
		- Icon Theme for Recent Files
		- Icon Theme for Libraries, Devices, and Drives
		- Icon Theme for Files and Folders
	- Opacity Settings:
		- Overall Tint Opacity
		- Overall Opacity
		- Content Area Tint Opacity
		- Content Area Opacity
	- Item Templates:
		- Solid Background for Items
		- Simple List Thumb Size
		- Simple List Length
		- Detailed List Thumb Size
		- Tiles Thumb Size
		- Tiles Length
		- Small Grid Thumb Size
		- Medium Grid Thumb Size
		- Large Grid Thumb Size
	- Internal Viewers:
		- Internal Text Viewer
		- Internal Text Viewer Editing Options
		- Internal Image Viewer
		- Internal Image Viewer Toolbar
		- Internal PDF Viewer (Experimental)
	- Parallel File Operation
	



**Changelog for Version 1.67 (April 24, 2022)**

* Re-enabled a feature for automatic update checking at the startup. However, it is disabled by default (CheckForUpdateAtStartup) and need to be tested.
* Startup improvements/optimizations. Some changes might result in unintended issues. Please report if user finds any issues/bugs with the app.
* Icons for the file, folder, library, and drive update instantly while changing the settings (except if the previously or newly selected option is the actual thumbnail).
* Added new icons for drives and libraries in the default icon theme. The libraries icons look similar to the built in Windows 11 icons. The drive icons look different. Users might need to delete existing default icons (located in the CustomIcons folder) before the new icons show up.
* Miscellaneous improvements.
* Fixed: Some icons such as log viewer and progress viewer did not appear reliably.




**Changelog for Version 1.66 (April 21, 2022)**

* Libraries, Devices, and Drives now follow the same icon type as This PC libraries, devices, and drives.
* Miscellaneous improvements.



**Changelog for Version 1.65 (April 20, 2022)**

* Added option to select icon types for This PC page.
* Fixed: Actual thumbnails for items were not loading without setting a proper config that was not exposed in GUI anymore.
* Miscellaneous improvements.




**Changelog for Version 1.64 (April 18, 2022)**

* Added splash screen.
* Text find previous/next implemented in the Internal Text Viewer.
* Added feature to use various themes for files/folders.
* Added feature to use various theme for commands such as buttons and drop downs.
* Added feature to use simple/colorful icons for the bookmark items. Setting simple icons from the bookmark editor does not work well yet. It does for colorful icons.
* Cancelling renaming shows up as a mini notification instead of a prompt that shows an error.
* Hyperlink color is more readable now. But, the hover over color is still not always readable.
* Minor update on the initial app tour.
* Startup improvements.
* Fixed: "Libraries" and "Devices and Drives" expanded state on the side bar was not restoring (other bookmark folders does).
* Fixed: Files without extension did not show a generic icon.
* Miscellaneous improvements.



**Changelog for Version 1.63 (April 10, 2022)**

* Libraries will appear above the "Devices and Drives" in the side bar now. This aligns with the order in the "This PC" page.
* "Libraries"" and "Devices and Drives" items can now have Emoji icons (instead of simple Glyph icons), colorful icons, and actual thumbnails. Live toggling may not work as expected in all scenarios. The changes should be reflected after restarting Shrestha Files Pro X. The colorful icons will be updated in the future.
* This PC page can now show Emoji icons (instead of simple Glyph icons), colorful icons, and actual thumbnails. Live toggling may not work as expected in all scenarios. The changes should be reflected after refreshing the "This PC" page.
* Custom icons are now organized in folders to keep them organized better.
* When a new file, folder, or zip file are created in any tab page, the page scrolls to the new item if it is not visible (until scrolled). This should work most of the time, but may not work reliably all the time.
* Markdown text with hyperlinks shows up again. Use of a reserved resource key (HyperlinkForeground) was the issue.
	- About page is updated so that the links for the third party licenses works again.
	- Changelog prompt now has links to the Discord server, Twitter, Youtube, etc.
	- Color of the link may not be very readable.
* More friendly drive names such as "Local Disk" instead of "Fixed" is shown.
* PDF file loading in the internal PDF viewer should be more reliable now. It comes with an overhead though.
* Updated Visual State break points to account for previously added item in the tool bar.
* Improvement: Tasks performed while upgrading the app to a newer version.
* Improvement: Improved text reading speed.
* Fixed: Navigating to "C:" from the address bar was loading "C:\Windows"
* Fixed: Remove recent file button (X) was overlapping with the file name when the file name is longer.
* Miscellaneous improvements.



**Changelog for Version 1.62 (April 1, 2022)**

This is the biggest update of Shrestha Files Pro X (Beta) since the first beta version was released.

1. Colorful icon themes

	- Three colorful icon themes are added. Switch between the icon themes from the Theme Settings. Refresh pages to see the change.
	- These icon themes provides generic icons for various types of files. 
	- Enabling these icons allows files/folders to load faster (because generating actual thumbnails takes a while).
	- Users can still choose to show actual thumbnails instead of generic thumbnails from the settings.
	- Users can also choose to use very basic generic thumbnails (based on Glyph icons) that should be even faster to load.
	- Users can choose to load actual thumbnails for specific file types even when generic thumbnails are used. This is useful for file types such as images for which actual thumbnails are significantly more useful.
	- Users can create their own icon themes: 
		* Create a folder inside CustomIcons folder in the LocalState folder. 
		* Paste SVG files for various file types, e.g. for file type ".txt", add a SVG file named txt.svg. 
		* Users can download the SVG files from places such as svgrepo or icons8. Thanks to both websites! Link is not added here because Community Toolkit's MarkDown editor is not working as expected when links are added. svg repo and icons8 links are provided in the About section of the app.
		* Make sure the SVG icons does not have width and height, if they do, just remove them, e.g., update this (svg viewBox="0 0 48 48" width="240px" height="240px") to this (svg viewBox="0 0 48 48"). 
		* Also add defaultfile.svg and defaultfolder.svg. defaultfile.svg is used for all file types for which type specific SVG file is not provided. 
		* defaultfolder.svg is used for all folders. 
		* Users can also add text.svg, image.svg, audio.svg, and video.svg that will be used for corresponding formats (e.g. text.svg will be used for .txt, .json, etc. if type specific icon is not provided).

2. Title bar should look nicer when Extend Contents to Title bar is enabled in Windows 10.

3. Thumbnails/icons are available now for system files, hidden files, and other shortcuts .appref-ms, .url, and .wsh files. These might look blurry in grid views.

4. Acrylic background image now stretches while maintaining proportion to avoid image distortion.

5. Fixed PDFViewer was not opening for pdf files. Known issue: the PDF viewer sometimes does not load all pages properly.

6. App rating feature reimplemented.

7. App purchase feature reimplemented.

8. App updater feature reimplemented.

9. Added sliders in the item template settings to change simple list and tiles length.

10. Share should work for files again! It may not support some file types such as .lnk, .url, etc.

11. Settings should be automatically saved while closing Shrestha Files Pro X now. The reliability of this implementation needs to be tracked over time.

12. PDF files should look sharper even when the window is slightly wider (1920).

13. Language switching should work even after restarting the app.

14. Miscellaneous improvements.





**Changelog for Version 1.61 (March 20, 2022)**

* Fixed: Image viewer title bar issue.




**Changelog for Version 1.60 (March 20, 2022)**

* Fixed: File name was showing as file extension.
* App preview in the taskbar should now show Shrestha Files Pro X logo.
* Fixed: Shortcuts (such as Delete button) were executing in the main window even when an internal viewer was focused.




**Changelog for Version 1.61 (March 20, 2022)**

* Fixed: Image viewer title bar issue.




**Changelog for Version 1.60 (March 20, 2022)**

* Fixed: File name was showing as file extension.
* App preview in the taskbar should now show Shrestha Files Pro X logo.
* Fixed: Shortcuts (such as Delete button) were executing in the main window even when an internal viewer was focused.



**Changelog for Version 1.59 (March 17, 2022)**

* Internal text, image, and pdf viewers are back in their own Windows.
* Internal viewer settings are moved back to their own settings.
* Added Ukrainian translation (machine translated).




**Changelog for Version 1.59 (March 17, 2022)**

* Internal text, image, and pdf viewers are back in their own Windows.
* Internal viewer settings are moved back to their own settings.
* Added Ukrainian translation (machine translated).




**Changelog for Version 1.58 (March 17, 2022)**

* Fixed crash while toggling between "extend contents into the title bar" on/off in Windows 10.
* Fixed issue with language switching.
* *.tmp files created by MS Office should not show up anymore.
* Reimplemented the internal pdf viewer. But it only shows one page at a time.




**Changelog for Version 1.57 (March 16, 2022)**

* Updated logo for the Pro X version.
* The generic folder icon color changed to the familiar yellow color.
* Tab pages now have rounded corners to make the app designing  more consistent.
* Added additional settings for opacity.
* Colors for the title bar and some buttons should be fixed now (when changing the theme).
* Internal viewers settings are moved to the experimental settings page since the internal viewers cannot be opened in a separate window as of now (because of the platform limitation).
* Additional attempt to enable extend the contents to the title bar option work as before on Windows 10 (e.g. make caption button visible).
* Miscellaneous improvements.




**Changelog for Version 1.55/1.56 (March 13, 2022)**

* Improved phasing of items to improve item loading and reduce memory usage.
* Reimplemented the Ctrl + Mouse Wheel shortcut to change the tab view type.
* Reimplemented the "press key to navigate" feature to scroll to an item starting with a specific letter or number. However, this will not work until a file or folder is selected in a tab. Also, the first press highlights the first item (although the correct item is actually selected).
* Reimplemented the back and forward commands (of mouse).
* Reimplemented the cloud drive availability feature.
* File size is more friendly (i.e. GB MB, KB, Byte as relevant instead of just KB).
* Improved loading of thumbnails, cloud availability status, and more descriptive file type.
* Miscellaneous improvements.



**Changelog for Version 1.54 (March 8, 2022)**

* Added config option to make copied items available in the clipboard even after Shrestha Files is closed. If this option is enabled, it may take longer to copy files to the clipboard, which would be noticeable when copying a large number of files/folders.
* Fixed: Dark and Light color themes were mixing up and some texts were unreadable. (It does not fix everything yet; some issues still exist.)
* Miscellaneous improvements.




**Changelog for Version 1.53 (March 6, 2022)**

* Internal text editor reimplemented with mini window. Full screen windows as in the Pro version is not possible in Pro X version yet because of the platform limitations.
* Internal image viewer reimplemented now with mini window. Full screen windows as in the Pro version is not possible in Pro X version yet because of the platform limitations.
* Additional settings saved for internal text editors.
* Miscellaneous improvements.




**Changelog for Version 1.52 (March 3, 2022)**

* Fixed: Sometimes empty folders were left while moving the folders.
* Number of concurrent file operations (for paste operations) can be set in the config file now (set value for ConcurrentFileOperationCount). Value of -1 indicates an unlimited number of parallel file operation (although the actual operation would probably be limited by the performance of the machine).
* Can now be launched as "sfiles" or "sfiles.exe" (e.g. from command prompt or run dialog).




**Changelog for Version 1.51 (February 28, 2022)**

* Fixed crash in Windows 10 resulting from the title bar customization.




**Changelog for Version 1.50 (February 27, 2022)**

* Extends content to title bar option now works well in Pro X version. 
* A small invisible strip (15px) is also added at the top of the window for dragging the window when the title bar is hidden. 
* The config file now has two variables to store the actual and virtual extends content to title bar option. The UI only updates the virtual extends content (as intended).
* Small strip is also added left of the caption buttons for drag region when the title bar is hidden.




**Changelog for Version 1.48 (December 20, 2021)**

* Fixed: In very specific scenarios, the app incorrectly determines that the destination folder is inside the source folder, and hence does not execute copy/paste.




** Note that Version 1.48 and newer indicate the development of Shrestha Files Pro X.**



**Check [Shrestha Files Universal Changelog](https://jptgamesandapps.github.io/ShresthaFiles/changeloguniversal) for older change logs**
