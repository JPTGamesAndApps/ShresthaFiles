---
title: Change Log History
layout: default
filename: changelog
--- 

{% comment %}
{% endcomment %}

## Changel Log History



**Changelog for Version 0.35.x (February 12, 2021)**
* Single click mode added as a result of popular demand.
* Flyout showing icons in Navigation bar edit view will now dismiss after selecting an icon.
* About Page now shows more information in selected language.
* Added analytics to understand and improve user experience.
* Added analytics to get handled exceptions (errors).
* Updated German Translation. Thanks to Parasec Glenkwyst!



**Changelog for Version 0.34.x (Unreleased)**
* Updated sizes for this PC (Home Page) items. Thanks to Chomu_ for feedback!
* When dragging and dropping items in the same folder, it does not copy/move items anymore. Thanks to Chomu_ for feedback!
* Initial implementation of back and forward button in mouse to navigation back and forward. Let the developer know if it still does not work.
* Improved change tracker when items are deleted from outside the app.
* Added translations in Chinese (Simplified), Czech, French, Hindi, Hungarian, Italian, Japanese, Korean, Russian, Spaish, and Turkish. The translations are based on Google Translation, so some of the translations could be confusing and/or misleading.
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



**Changelog for Version 0.30.x (February 5, 2021)**
* Improved Navigation Bar Edit View:
	* Item borders are now hidden for cleaner interface.
	* Icon choices now displayed in a grid instead of a long list.
	* Note that once the icon is selected, user needs to click outside the pop up to dismiss the pop up.
* Shows notification that the source and destination file cannot be same when replace option is set.
* Resources for all the language should be included by default in the application now! This will enable switching languages without having to download additional project resources.
* Fixed: Crash sometimes while switching theme.



**Changelog for Version 0.29.x (February 1, 2021)**
* File access permission prompt should not show up if at least one drive was accessed successfully.
* Fixed: App crashes when changing the tab view type before item loading is complete.
* Fixed: App crashes when trying to open a file that may not exist anymore.
* Several other bug fixes.



**Changelog for Version 0.28.x (January 31, 2021)**
* First release of the free version with some limitations!
* Re-added browse location for permission in Settings for devices such as XBox and Windows 10X that may not have File Access Permission Settings.
* Bug fixes.



**Changelog for Version 0.27.x (January 30, 2021)**
* You app settings might be reset after the udpate. A back up config will be saved in the Application folder (LocalState) if users desire to copy some settings manually.
* Draggable area improvements - More areas to drag/move windows:
	* Draggable region on the top right side of the screen is now wider. Thanks to feedback from @Zen.
	* Small draggable region added on the left end of the title bar as well.
	* Can also drag from the top of the title bar (only a narrow portion).	
	* Search box is now hidden in home page (as it does not do anything in the home page).
	* Search box is now narrower while browsing folders. 
* Navigation bar (side bar) improvements:
	* Navigation bar can now be opened from context menu of navigation bar as well.
	* Added tooltips for the navigation bar items.
	* Drives in the navigation bar shows progress bar indicating the used space. Thanks to @FireCube for feedback!
	* More robust navigation bar.
* Added tooltip for items in the homepage.
* Theme engine improvements.
* Single click selection mode added in the home page. Thanks to feedback from @Zen.
* Enter key now opens file/folder.
* Prompt to choose dual pane or single pane mode at the first launch after file access permission is provided.
* App tour at the first launch after file access permission is provided.	
* App reset option added in the About Page.
* Improved local network browsing - the breadcrumbs works now.
* Dual pane separator is thinner by default now. Its thickness can be customized in the config file (for thicker or even thinner pane separator).
* Mini notification added at the launch to indicate that the tabs and settings are loading. If many tabs are open this will let users know that the tabs are being loaded.
* Navigating away from a tab that is still loading (i.e. still enumerating files and folders) should be quicker and more reliable now.
* Fixed: Sometimes Search/Filter clearing (x) does not update the result as expected in dual pane mode.
* Fixed: Overlapping breadcrumb and path after path is entered (Enter) to browse to the path.
* Miscellaneous improvements and bug fixes.



**Changelog for Version 0.26.x (January 16, 2021)**
* Added context menu option to open selected folder in a new tab.
* Updated the Most Recent Items View in the Home Page to use the tile view with thumbnails.
* Supercharged About Dialogue with keyboard shortcuts, changelogs, and more.
* Improved Breadcrumbtrail with MDL2 ">" icon. 
* Added "This PC" icon at the beginning of breadcrumbtrail similar to the ones in the Windows File Explorer.
* Acrylic removed from the progress viewer and log viewer. Thanks too @FireCube for feedback!
* Icon for new file updated for improved consistency.
* Configuration file reading mechanism updated. It tries to read regular config file. If it fails, it reverts back to config file that was previously read successfully. If that fails, it reverts to default config.
* Updated mechanism to show/hide breadcrumb and path.
* Fixed: Paste does not work sometimes when copying files from external applications. sometimes external applications can set the paste option wiht link as one of the options.
* Fixed: Grid splitter shows bidirectional (instead of four directional) arrow pointer while hovering over grid splitter in dual pane mode. Thanks to Kristóf Kékesi for the bug report!
* Fixed: Grid splitter color now uses theme-relevant color while dragging and mouseover. Thanks to Kristóf Kékesi for the bug report!
* Fixed: File Access Permission prompt should show now show up when the app is launched for the first time and file access permission has not been enabled yet. Thanks too @FireCube for bug report/feedback!
* Fixed: Minimize, maximize, and close buttons on the title bar now have contrasting colors in various all themes. Thanks to matthewotten for the feedback.
* Fixed: Double tapping an item sometimes navigates to the parent folder instead of opening double tapped item.



**Changelog for Version 0.25.x (January 1, 2021)** 
* Added proper tool tip descriptions for all buttons and context menus.
* When any picture is opened from the app, users will be able to browse to other photos in the Folder (in Windows Photos app).
* Added notification when saved settings cannot be read.
* Improved breadcrumb generation by relying on path solely instead of StorageFolder.
* Keyboard Accelerators (shortcuts) should finally work reliably.
* Added the app icon on the empty draggable area (top right corner of the app) for trial users.
* Changelog window can be dismissed by tapping outside (so that users don't have to scroll to the end to click Ok).
* Reduced memory usage by caching instead of using memory.
* Fixed: Bug extra libraries and disks are added while refreshing home page.



**Changelog for Version 0.24.x (December 28, 2020)** 
This is one of the major updates with a significant number of improvements and bug fixes.

* General Interface *
* After the app is updated, the most recent changelog is displayed directly in the app.
* Updated and improved Welcome and About Windows.
* Purchase option added in the trial expired message.

* Navigation Bar *
* Libraries now have Desktop, Documents, Downloads, Pictures, Music, and Videos. The Desktop link does not work in Windows 10X (not Windows 10).
* The library items now use path instead of StorageFolder. This will increase their reliability and enable the use of change trackers for the library folders.
* Improved code base to load drives in the navigation bar and home page.
* Does not navigate to "This PC" anymore when clicking to parent navigation items (such as Libraries) that has child items.
* While adding bookmarks in the navigation item bar (Ctrl+D), a unique name is generated to avoid any issue later.

* File Operations *
* Improved progress count behavior when "If File Exist in Destination -> Skip" option is selected.
* Added Progress Indicator for Compression and Decompression operations.
* Improved sanity check for file operations. Now also checks if an item is being replaced by itself (when "If File Exist in Destination" -> "Replace" is checked).
* Does not create empty folders in Recycle bin anymore while moving items.
* More streamlined notifications of file operations. Start and completion of file operations are logged now. File operation errors are also logged now.

* Miscellaneous *
* Background tracker for tabs in the second pane is removed when switching from dual pane to single pane mode.
* Cleaned up start up tasks for improved performance.
* Updated the minimum OS version to Windows 10 Version 2004 (20H1).

* Other Fixes *
* Fixed: Keyboard Accelerators not executing at all or not executing in the correct tab when the tab is empty.
* Fixed: Crash while dragging a file to navigation bar.
* Fixed: Sometimes tab header does not change from "This PC" to correct title.
* Fixed: Crash loop at the launch of the app in certain scenarios.
* Fixed: Decompression not working.
* Fixed: Error caused in some instances where UI updates are marshaled from a different thread.
* Fixed: Crash when clipboard cannot be accessed to enable/disable paste option.

* Other bug fixes and improvements.



**Version 0.23.x (December 14, 2020)**
* Updated Navigation bar item edit UI (wider UI to ease path entry and viewing)
* Improved file/folder drag and drop. Can drop items inside a folder now, not just inside a tab page.
* Can drag folders to navigation bar to pin it there.
* Updated About dialogue UI and content.
* Fixed crash that occurs when loading invalid path from saved tabs at the start of the app.
* Updated Microsoft UI XAML Control (MUXC) Dependency to 2.5



**Version 0.22.x (November 30, 2020)**
* This version focuses primarily on performance improvements and bug fixes.
* Added clickable breadcrumb trails inside the tabs in the dual pane mode.
* Hides purchase option if already purchased.
* Adjusted tile sizes to display file/folder name in up to two lines.
* Does not rely solely on tracker change for changes made from inside the app. Much reliable internal file change is developed for file operations from within the app itself.
* Updated navigation logic to improve reliability.
* Improved multi-threading to keep the UI more responsive while loading items, during file operations, and while updating the tabs with external changes in the file system. The experience should be notably smoother now.
* Further simplified tab header setting process to improve its reliability.
* Many other changes to improve performances and bug fixes.
 
 

**Version 0.21.x (November 15, 2020) **
* Back and forward navigation icons will be enabled/disabled as relevant.
* Reverted the fast loading option to an experimental status as it appear to cause some issues sometimes.
* Will open file/folders faster on double click double click.
* Various view types for libraries are assigned (e.g. if you open pictures library from the navigation bar, it will open with large grids irrespective of default tab view setting). If this is not a fresh install, you will need to reset (delete) your configuration file or edit the config file for it to work.
* Removed file access permission request messages other than for the first launch.
* Context menu improvements.
* File operation progress viewer will not close automatically anymore to let users' close it at their convenience.
* Improved error logging in file operation progress viewer.
* Can now show/hide progress logging for each operation.
* File permission keyboard accelerator (shortcut) (Ctrl+P) removed.
* Added tool tip for file/folders to easily view file name and other details in any tab view type. This may not be accurate in the fast loading mode.
* Improved background tracker's reliability. When automatic change trigger/update fails, the alternative tab refresh should work better than before after file operations. It still needs some improvements.
* Code cleanup to improve reliability for further development.
* Other bug fixes and improvements.



**Version 0.20.x (November 1, 2020)**
* Updated file operation (such as copy/paste/cut) speed with updated codebase.
* More detailed file operation progress reporting is available in the progress viewer.
* Re-enabled manual change trigger after file operations such as new file and new folder creation to improve auto refreshing of the tab contents.
* Added configuration option for acrylic tint opacity (not exposed via GUI yet).
* Teaching tips added to launch file access permission settings at the beginning if such access is not enabled.
* Fixed: Typing path in address bar was not loading the path in the tab in certain scenarios.
* Other miscellaneous improvements and bug fixes.



**Version 0.19.x (October 29, 2020)**
* This is the most significant update of the app to date. A significant portion of codebase is rewritten/updated to improve item loading speed, more future proof configuration files, and improved auto change tracker to reflect item changes.
* For faster loading, let Windows index the directories you frequently visit. Folders added in any Windows Libraries (such as Documents) are automatically indexed by default.
* Settings from previous version will be backed up in the application folder but cannot be imported automatically because of the significant changes in the codebase.
* Windows limits the number of background tracker that needs to keep the folder view updated (to about 20 trackers at a time for an app). If too many tabs are open (say more than 20), the background tracker will not work for new tabs unless older tabs are closed. File/folders views will not be updated automatically in such cases.

**Detailed changelog for this version.**
* Significant improvement in loading speed for indexed folders.
* Notable improvement in loading non-indexed folders as well.
* More professional file and folder icons.
* When switching the view types, thumbnails are automatically reloaded to provide optimum thumbnail quality without having to refresh the tab.
* Increased item viewing area in non-detailed-list view mode (the area for headers for detailed view will collapse in other views).
* Tab header icon removed to optimize the use of screen real estate.
* Added option to view full log file.
* Log file location moved to temporary folder so that older logs will be deleted automatically.
* Added option to view configuration file directly from the log viewer.
* Added option to view application data folder from the log viewer.
* Added option to enable/disable various types of logs in the log viewer. Log file will include all types of logs irrespective of this setting.
* Major changes to improve the tab information model storing, loading, and processing mechanism.
* Major changes to improve storage item display and update.
* Significant improvements on change tracking to reflect the changes in the file/folders instantly (without refresh).
* Improved navigation bar item codes/logics.
* Removed folder loading/navigation animations to improve loading speed.
* Added shortcut Ctrl + T for new tab in the current view.
* Status bar shows the number of items more reliably while loading new folder.
* Address under the tab is visible only in dual pane mode.
* Items are presorted from query directly whenever possible to speed up tab loading.
* The navigation pane open/close state is saved in configuration.
* Fixed: Most recently used list loading failing when an item cannot be accessed.
* Many other improvements and bug fixes.



**Version 0.18.x (October 11, 2020)**
* This is one of the major updates to this app since the first release!
* If icons do not appear as expected in the navigation bar, please restart the app.
* Added Home Page (This PC) with Libraries, Drives, and Recent Files list.
* Title bar removed to optimize the use of screen real estate.
* Added zip file extraction feature.
* One click editing of path in the address bar.
* Improved method to add drives to the navigation bar.
* If no tab is loaded, clicking the navigation bar item will open a new tab.
* Ignores content change tracking by default to improve performance.
* Updated mechanism to display icons which will enable the use of more icons than before.
* Added option to update default page for new tabs (not exposed in GUI yet).
* Fixed: Libraries not showing up when app is launched for the first time.
* Fixed: Bread crumb trail sometimes not created until user clicks on one of the panes even after navigating to a different location.
* Fixed: Creates unique folder name if file with the same name exist. UWP has a limitation of not being able to create folder with the same name as an existing file name.
* Miscellaneous improvements



**Version 0.17.x (October 6, 2020)**
* Added feature to change theme manually.
* Changed the selection mode option to checkbox to simplify the option.
* Updated the view modes sizes.
* Improved consistency of address bar and search bar while hovering.
* Settings pane reorganization/improvement.
* Added icon to indicate that the items in the navigation bar can be moved.
* Backs up previous settings when updated version of the app is launched. This will help manually restore some of the settings automatic restore fails.
* Documentations are copied to the app folder.
* Offers to open change log when the version is updated.
* Offers to open read me document when installed for the first time.
* Separated progress viewer and log viewer. Improved progress and log viewer show/hide logic.
* Improved logging.



**Version 0.16.x (September 28, 2020)**
* Can reorder navigation bar items from the edit navigation items view.
* Six view types are available now: Simple Lists, Detailed Lists, Small Grids, Medium Grids, Large Grids, and Tiles.
* Removed preset resize pane icon.
* Browse Folder Option for Permission removed.
* Added acrylic background in more areas of the application.
* Improved reliability of change tracker.
* Path and Search Box borders removed for minimalistic view.
* Folder size not displayed as "0 KB" anymore.



**Version 0.15.x (September 6, 2020)**
* Ratings option added
* Purchase option added
* Single Pane Mode Added



**Version 0.14.x (September 5, 2020)**
* Added context menu to open pinned navbar item in a new tab.
* Added context menu to unpin navbar item.
* Improve tracker reliability to keep the tabs updated.
* Updated the "CDRom" to "DVD Drive" for all spinning drives in the navigation bar.
* Shows build number in the About Window
* Added View Type option in the context menu
* Added Sort by option in the context menu
* Added checkbox mode for item selection (useful for touch screens)
* Added Date for Folders
* Compress context menu is visible only if items are selected
* Fixed: Libraries goes missing from the navigation bar.
* Fixed: Navigation item does not work when first item does not have subitems and the following one does.



**Version 0.13.x (August 30, 2020)**
* Implemented progressive loading by loading 100 items at a time to improve loading folders with a large number of items (>500). Sorting will not work perfectly as the folder loads, but the items will be resorted once everything loads. Thus, users will be able to see some files/folders as loading continues even if not sorted as desired.
* Improved reliability of quick loading. The previous quick loading option is now used in all cases.
* Added a loading time logger to measure loading performance.
* File/folder change notification removed. The log viewer shows a log instead.
* Fixed bug that showed an error message while loading a library.
* Fixed bug that showed an error message while loading an empty folder.
* Minor bug fixes and code cleanup.



**Version 0.12.x (August 23, 2020)**
* Sorting maintained when tab is updated with file content change
* Tab refresh will work even if an item(s) is selected
* Zip compression feature added
* Tracker improvements after file operations
* Bug fix: Rename did not remove existing item from the list.
* Bug fix: App crash while trying to refresh after file operations such as rename.



**Version 0.11.x (August 19, 2020)**
* Mini notifications added for file operations
* Added Open with Option
* Updated shortcuts: F3 will open a file/folder; F4 will show "Open With" dialogue box for files and launch Windows File Explorer for folders
* Launch the app from command line by typing "file"
* Bug fix: keyboard shortcuts/accelerators were not working sometimes



**Version 0.10.x (August 13, 2020)**
* Added Info Panel (Log Viewer and Progress viewer). Click on the "*" button on the status bar.
* Log viewer and progress viewer can be collapsed or made visible as desired by clicking on the headers.
* Progress bar can now be manually closed. More improvements on the progress bar.
* Progress bar cancel button disappears automatically after the operation is complete.
* Improved log reporting in the log viewer. Added button to clear log.
* Informational dialogue boxes are replaced with teaching tips versions for more stability.
* More intuitive experience of right clicking as in Windows File Explorer, i.e. right clicking will update the selected items (if the item is already selected, nothing happens, if the item is not already selected, the item will be selected and other items will be unselected).
* Various context menu items are visible depending on whether any item is selected.
* More intuitive left click behavior, i.e. left clicking on empty area will unselect existing selections.
* Displays licensing status on the title bar. Added notifications for expired trials.
* Initialization code improvements.
* (Experimental) Implemented automatic folder tracking to keep folder contents of tabs up to date even when files are changed from outside the app. 
* Implemented forced auto refresh to ensure folder contents of tabs are up to date after file operations even if automatic folder tracking fails.



**Version 0.9.x (August 2, 2020)**
* Navigation items can now have category items and subitems
* Drives automatically added to the navigation items
* Toolbar items moved to title bar for cleaner look and optimum utilization of screen space
* Items sorting added. Persistent sorting saved for each tab
* Added context menu (new folder, new file, copy, cut, paste, rename, delete, copy path, etc.)
* Cleaner settings pane
* View type uses cleaner dropdown instead of toggle bar
* Added tab loading progress indicator (and option to show/hide the indicator)
* Generic/Actual File and Folder thumbnail loading option added
* Can click anywhere in the empty space in the address bar for editing mode.
* Text in input dialogue selected by default to ease inputs.
* Experimental quick loading added (dates and sizes may not load. sorting may not work well.)
* Bug fixes



**Version 0.8.x (July 26, 2020)**
* Tab size fits header text instead of being equal sized.
* Application wide Compact mode (e.g. more rows of data fits on the screen).
* Bread crumb trail address bar (i.e., address bar is clickable).
* Drag and drop mode changed to move/cut instead of copy.
* Refreshes both source and destination folder after moving files/folders. Refresh also works while dropping files in a folder in the same tab view.
* Added feature to cancel file operation.
* Fixed: Tab view was reset after file operation.



**Version 0.8.x (July 19, 2020)**
* Customizable navigation bar item list.
* Added acrylic background for navigation view.
* Resizable panels. The panel sizes are saved and restored with other settings.
* Resizable columns in list view mode. Column sizes are saved and restored with other settings.
* Drag and drop improvements.



**Version 0.7.x**
* Saves and restores session (tabs and settings)
* Added Navigation Bar with Standard Libraries (document, music, video, pictures)
* Added Drag and Drop Support
* Clipboard support for file operation (copy/cut/delete/paste)
* Sanity check before copying/moving files
* File operations progress indicator improvements
* Much improved navigation
* Added alert for empty folders
* Improved search box
* Three panel size options
* Added button for file access privacy setting
* Lots of bug fixes

