---
title: Change Log History
layout: default
filename: changelog
--- 

## Change Log History
The latest "Free" version is version 0.90.x. "Pro" versions are updated to the latest version posted here.

Some versions are relased gradually, meaning not everyone will get the latest version as soon as it is released. This is to ensure that if any unexpected bugs are introduced in the app resulting in crashes, the developer will get a chance to fix it before releasing to all users.



**Changelog for Version 1.0 (September 1, 2021)** 

* Thank you everyone for using Shrestha Files Pro throughout the journey! Today, we are releasing Shrestha Files Pro version 1.0. This is a huge milestone and by no means the end of the journey! If you have any feedback or bug reports, please reach out to the developer.




**Changelog for Version 0.64.x (August 16, 2021)** 

* Fixed: Navigation editor crashes when path is null.
* Minor improvement.




**Changelog for Version 0.63.x (August 16, 2021)**

* Miscellaneous improvements and bug fixes.
* Fixed: Scrolls to an item when typing something while content dialog is open.



**Changelog for Version 0.62.x (August 15, 2021)**

* Image viewer should load image at the center now.
	* Known Issues: Zooming is not proper after an image is rotated.
* Miscellaneous improvements and bug fixes.
* Accessibility improvements.



**Changelog for Version 0.61.x (August 12, 2021)**

* Updated language list in the settings.
* Added feature to remove a single recent file from This PC page.
* Added feature to set image as an app background from internal image viewer.
* Addressbar improvement: Clicking an addressbar now highlights the path text.
	* Known issue: Context menu does not work as expected in the addressbar path mode.
* Fixed: Search suggestion selection copies now copies file name instead of detail.
* Fixed: Context menu did not show up in detailed tab view mode inside an empty folder.
* Fixed: The internal PDF viewer did not launch when an item without extension exists in the current folder.
* Typing a key will set focus on relevant item as well, not just scroll to the item.
* MTP improvements
	* Fixed: Copy/paste and drag and drop should work again with some limitations.
	* Known Issues
		* New file cannot be created in MTP devices.
		* Dropping an item from MTP device to other location will not refresh the MTP folder (move operation).
* Progress bar in home page upgraded to MUXC version.
* Miscellaneous improvements and bug fixes.




**Changelog for Version 0.60.x (August 10, 2021)**

* Added new machine translated languages.
* Pressing Enter after entering keyword in the search/filter box now executes extended search.
* Added search icon to enable accessing search UI in the touch mode.
* Content dialogs (such as rename dialog) now has semi-transparent background.
* Added option to clear recent items in This PC Page.
* Tabs are not equal width instead of SizeToContent.
* Added option for parallel file operation.
	* Known Issue: Sometimes UI may freeze while performing a large file operation in parallel.
* Improved Internal Viewers:
	* Image Viewer: 
		* Added Shortcuts:
			* Ctrl + - -> Zoome out
			* Ctrl + + -> Zoome in		
			* Ctrl + R -> Rotate Clockwise
			* Ctrl + Shift + R -> Rotate Counter Clockwise
			* Ctrl + W -> Set as Desktop Wallpaper
		* Known Issue: The first loaded image does not align to center of the canvas.
	* Text Viewer:
		* Added shortcuts:
			* Ctrl + E -> Toggle read/edit mode
			* Ctrl + S -> Save Edits
			* Ctrl + W -> Toggle word wrap
			* Ctrl + M -> Turn on/off markdown preview
			* Ctrl + - -> Decrease font size
			* Ctrl + + -> Increase font size		
	* Audio and Video Viewers:
		* Playback pauses/stops when the window is closed.
* Improved properties viewer positioning in the detailed tab view  mode.
* Miscellaneous improvements and bug fixes.
* Thanks to Alur for a number of UI feedback.




**Changelog for Version 0.59.x (July 27, 2021)**

* Added option to select the Navigation Transition (animation).
* Added context menu in This PC page:
	* Open Library, Drive, or Recent Item.
	* Open Library or Drive in new tab.
	* Show basic properties of Library, Drive, or Recent item.
	* Refresh This PC page.
* Added option to delete files/folders permanently. Note that even if this is disabled, files may be deleted permanently (for example files from an external storage devices).
* Various internal viewers (text, image, audio, video, and pdf viewers) can be individually set as default to open relevant files.
* Image viewer improvements:
	* Can now zoom in/out with Ctrl + Mouse Wheel Scroll.
* Only one warning is retained when switching themes multiple times so that user needs to dismiss only the last one if user choose not to restart the app.
* App tour follows the app theme now.
* Purchase option in About Settings is now hidden from Settings if the app is already purchased.
* Selection box now has solid border instead of dashed stroke to follow File Explorer's style.
* Fixed: Double tap in empty area to navigate to the parent folder works again.
* Fixed: Default DragAndDrop checkbox was not getting selected automatically in the settings based on the user preference.
* Fixed: Selected language should be shown in the Miscellaneous settings now.
* Several improvements to address design feedback from Alur, CyberDroid1, and Parasec that includes:
	* Background color of disabled buttons are now set to the transparent color.
	* Hyperlink and markdown hyperlink foreground colors are updated to use regular text color to ensure readability.
	* Property values in the Properties viewer uses TextBlock now so that it does not appear as input field.
	* Drive space indicator (Progress bar) in This PC page now have round edges.
	* Fixed: Sliders were looking different in various settings pages.
	* Log viewer is now hidden by default. Log viewer will record and show logs only if log viewer button is enabled. 
	* Initial tab loading notification is now replaced by a less intrusive progress ring.
* Miscellaneous improvements and bug fixes.




**Changelog for Version 0.58.x (July 21, 2021)**

* Extended search is finalized and is available to all uses by default.
* Added Settings:
    * Added a setting to extend or not extend contents to the traditional title bar so that users can use full title bar for dragging the window if desired.
    * Added settings to show/hide 'Edit Navigation Items' and 'Save Settings' items in the Navigation bar. 
    * Added a setting to show Properties Viewer by default. The Properties Viewer will continue to show/hide based on the current state of the tab for an existing tab. For tabs created based on another existing tab, the state of the Properties Viewer visibility will be copied from the existing tab.
* Improved internal text viewer/editor:
    * Added ability to preview markdown document.
    * Added ability to edit and save plain text documents.
    * Added ability to turn on/off word wrap.
    * Added ability to change font size.
    * Note: the text editing options are intentionally hidden for now. Right click on the top left side of the address bar to see the options.
* Improved internal image viewer:
    * Added option to set image as desktop background.
    * Added option to zoom in/out.
    * Added option to rotate image.
    * Added option to drag image.
    * Known issue: These features are still experimental and need some improvements. While double tapping works for zooming in, double tapping while holding shift key does not work as reliably. Control + Mouse wheel may not be possible because of CoreWindow limitation.
* Property viewer now resides inside the Tab Page and Home Page.
* App tour has been updated to address the changes in the UI.
* Disabled parallel file processing for file paste operation to improve stability of the UI. DispatcherQueue appears to freeze when it is overwhelmed with the parallel UI update requests from the parallel file processing requests. File operations will be slower than previous versions but will be significantly more stable for file operations involving a large number of items.
* Search bar next to the address bar is now renamed to filter bar to better communicate the actual functionality of the control.
* Removed dual pane prompt for new installs. Users can continue to enable/disable the dual pane mode from the settings as before.
* Fixed: Selection box had some offset compared to the pointer location in the detailed view mode.
* Items will not be added to the search page when tracker tries to update something.
* Updated German Translation. Thanks to Parasec!
* Miscellaneous bug fixes and improvements.




**Changelog for Version 0.57.x (July 8, 2021)**

* Added ability to launch various file types such as .exe and .bat using an add-in that can be [downloaded from the Store:](https://www.microsoft.com/store/apps/9N9RH89JLDL1).
* More efficient mechanism to update UI to show item changes (such as added new items or deleted existing items) from all tabs.
* Fixed: Internal viewer was not opening files when at least one of the files did not have a file extension.
* Migrated from core window dispatcher to dispatcher queue - should also reduce UI freeze when large number of files are being copied/pasted in any tab.
* Miscellaneous improvements and bug fixes. Thanks to Alur, CyberDroid1, Parasec, and Fairycn for continuous design feedback, bug reporting, feature request, and translation updates.



**Changelog for Version 0.56.x (July 2, 2021)**

* Added tabs on top mode. Users can switch to that mode from the general settings.
	* Known issue: Window must be dragged from a narrow strip on the top right corner of the window left of the caption (close, restore, minimize buttons) in the tabs on top mode. The tab strip footer is set as a draggable region but is not working as expected as of now.
* Can now drop items to tab headers. 
	* Known issue: It might take some time before it allows to drop items. (Users can hover over to a tab header only after sometimes before the drop acceptance indicator is shown).	
* When any alphanumeric key (such as "a" or "3") is pressed in a tab page, it will scroll automatically to an item whose name starts with the pressed alphanumeric character. Non alphanumeric characters are not supported at this time. Thanks to Yair for the feature request!
* Updated Glyph icon for the address bars. The icon is now visible only in the path edit mode. Thanks to CyberDroid1 for feedback!
* Improved context menu item visibility toggling.
* Fixed: Free space in drives were not showing correctly in the navigation bar and/or This PC page. Thanks to CyberDroid1 for the bug report!
* Fixed: Some minor changes to resolve app crash when navigation pane width slider is changed from the General Settings. Let the developer know if it still crashes.
* Fixed: Address bar and status bar was not updated as expected in some scenarios. This was intentionally unlinked in earlier versions to investigate the layout cycle error that was crashing the app in some cases.
* Miscellaneous improvements and bug fixes.



**Changelog for Version 0.55.x (June 28, 2021)**

* Updated various UI components to fit an updated WinUI version. Some UI elements will continue to be updated in the future versions.
* Added item templates setting to change default sizes of icons for various tab view types. Thanks to FireCube for feedback on the preview!
* Added option to view previous and next item (such as images) in the internal viewers.
* Internal audio player now shows music cover art as the background image.
* More robust method to show File Access Permission dialogue when relevant.
* Enabled saving settings even if file access permission is not granted.
* Added three levels of performance modes in config file.
* Fixed: Drives were not loading when "Reload Drives when refreshing This PC" is disabled.
* Fixed: Theme setting crashes in high contrast mode.
* Fixed: Layout cycle error is hopefully be fixed.
* Miscellaneous improvements and bug fixes.



**Changelog for Version 0.54.x (June 18, 2021)**

* Improved item layouts. Layouts are more condensed now.
* Generic icon (Glyph icon) now uses folder with solid color to easily distinguish with the generic icons for folders. The solid color should also blend well with the theme colors.
* Minor localization improvements.
* Minor changes in analytics to identify the source of the layout cycle bug.
* Fixed: Recently used item icons not visible when generic thumbnail was used.
* Miscellaneous bug fixes.



**Changelog for Version 0.53.x (June 17, 2021)**

* Added option for solid background (boxy looks) for items (files, folders, drives, libraries, and recent items).
* Added functionality to move previous and next images in the internal image viewer.
* Uses glyph icons for folders and files instead of image icon for reduced memory consumption when actual thumbnail is not used.
* Improved drag and drop items to navbar:
	* Can now drop folder(s) inside an existing navigation bar item to create children items (sub-items).
* Added opacity settings for content area (Tab Page and This PC Page) background.
* Restructured settings.
* Improved tab view layout. 
* Improved tab view cycle order (Ctrl + Mouse Scroll).
* Item selection method updated with more efficient method. Thanks to Yair for feedback!
* Unified and more robust method to obtain storagefile for copy/cut/delete/compress.
* Improved reliability and performance of updating UI with changes in the file system.
* Added low memory option in config that can significantly reduce memory usage. However, the low memory usage may not perform as well (e.g. thumbnails may not get updated quickly or at all sometimes for some items. Also, operations such as drag and drop will take longer to start.)
* Fixed: File Access permission was not showing in new installation.


**Changelog for Version 0.52.x (June 11, 2021)**

* Added minimalist internal viewer (F6) for various file types [Pro Users Only]:
	* Audio and video - supports formats such as mp3, mp4, and wmv.
	* Image - supports formats such as png, jpg, and gif.
	* Plain text - supports formats such as txt, json, and xml.
	* Pdf - supports pdf.
* Some notes on the internal viewer:
	* Users can add other file formats in the config file to see if that is supported. For example, text files that has other file extension can be viewed using the internal viewer.
	* Audio or video must be paused before closing the window. Otherwise, it will continue to play even after closing the window.
* Added drag selection. Thanks to Kweku for the feature request.
	* Now need to triple click instead of double click to navigate to the parent folder.
* Added option to show thumbnails for libraries, drives, and devices in "This PC" page. Some external devices may not show icons in the thumbnail mode.
* Added option on the navigation bar to pin the app to the taskbar.
* Added experimental setting to use a custom background instead of desktop (host) background in for the acrylic effect.
* Added machine translated Polish translation.
* Miscellaneous bug fixes and improvements.



**Changelog for Version 0.51.x (June 5, 2021)**

* If Navigation bar shows multiple copies of "This PC", "Libraries", or "Devices and Drives", please right click and remove both copies of those items and restart the app.
* Added compact mode under the experimental settings. Currently, it affects a few UI elements such as navigation bar item, addressbar, etc.
* Improved devices and drives loading. If some external devices did not show up in "This PC" page before, it may show up now.
* Improved drive loading. 
* Improved tooltips for drives.
* Improved localization. Thanks to Fairycn for feedback!
	* Toggle switch "On" and "Off" can also be translated now.
	* While switching language, different messages will show up depending on whether the translation is completely online or someone helped with the translation.
* Miscellaneous improvements and bug fixes.



**Changelog for Version 0.50.x (May 22, 2021)**

* Minor improvement in drag and drop.
* Minor improvements in analytics for better debugging.



**Changelog for Version 0.49.x (May 20, 2021)**

 * Another attempt to solve app crash resulting from Layout Cycle bug. If the app is crashing, please email the the developer with some information on when and how the app crashes.
 * Better analytics to improve bugs identification and fixing.
 * Updated Chinese Simplified Translation. Thanks to Fairycn!



 **Changelog for Version 0.48.x (May 17, 2021)**

* Improved extended search UI to match with the tab page.
* Fixed Ctrl + H not working fully as expected.
* Other miscellaneous bug fixes and improvements.



**Changelog for Version 0.47.x (May 15, 2021)**

* Tabs can now be dropped to a different pane. However, the destination pane must have at least one tab. Otherwise, a tab cannot be dropped there.
* Added option to show/hide progress viewer automatically. The progress viewer show/hide button will animate/rotate once (per application launch, not per operation) to indicate the location of the log viewer if user is interested in seeing the file operation progress.
* Share context menu is visible only when at least one item is selected.
* Fixed: Bug that loaded replica of tabs in the second pane when opening settings.
* Other miscellaneous bug fixes and improvements.



**Changelog for Version 0.46.x (May 12, 2021)**

* Can click and hold control key while dropping items to copy instead of move when default drag and drop option is move. External application such as Windows File Explorer may ask for copy or move option while dropping. Thanks to Parasec Glenkwyst for the feature request!
* Settings pages also uses compact mode now. This mostly affects the navigation bar items in the settings.
* Cleaned up the extra About Page (F1). Making it more minimalist.
* Fixed: Crash resulting from Layout Cycle error.
* Fixed: Error while trying to puchase the app in some cases.


**Changelog for Version 0.45.x (May 10, 2021)**

* Improved standard and hero themes.
* A sample theme is now included in the custom theme folder.
* Can now change the tab view type by using Control + Mouse Wheel Scroll. Thanks to Kweku for the feature request.
* Added option to sort items by clicking on the headers in the detailed list tab view mode.	
* Checkboxes can be turned on/off directly from selection split button inside a tab.
* Added "Share" option in the context menu for files and folders.
* Removed edit/pencil icon from the address bar. Thanks to Alur for the feedback!
* Settings page now shows category titles to better communiate the category information without having to hover over the icons or navigate to the category page.
* Breadcrumb in the addressbar can be scrolled if the content does not fit the available addressbar width.
* Improved UI to better fit different window sizes.
* Added experimental settings to show the number of number of files and folders and a sample list of files and folders in the preview pane. Thanks to Alur for feature request!
* Miscellaneous bug fixes and improvements.


**Changelog for Version 0.44.x (April 25, 2021)**

* Custom theme can be added by users now. Visit our discord server for additional themes.
* Bug fixed for back/forward button resulting in click effect when no back or forward stack is left.
* Miscellaneous bug fixes and improvements.




**Changelog for Version 0.43.x (April 17, 2021)**

* Back and forward mouse button "should" finally be working.
* Added shortcuts to navigate back
	* Windows + Backspace
	* Gamepad B button
* Added GUI to select all, invert selection, and clear selection.
* Miscellaneous improvements and bug fixes.




**Changelog for Version 0.42.x (April 14, 2021)**

* Translations restored.
* Tab view type and tab sort by icons should update more reliably.
* Fixed sticky search/filter text issue after filtering/searching.
* Miscellaneous improvements and bug fixes.



**Changelog for Version 0.41.x (April 13, 2021)**

* Several icons added in context menu. Now all context menu items and sub items have icons.
	* Copy Path Context Menu
	* Properties
	* Compress
	* Decompress
	* Sort By: Name/Type/Date/Size
	* View Types: Simple List/Detailed List/Small Grid/Medium Grid/Large Grid/Tiles
	* Ascending/Descending.
* Added settings to select default sorting field and sorting order for new tabs. This will be ignored when previous tab is used to create a new tab.
* Updated titles of settings categories (e.g. "This PC" instead of "ThisPC").
* Removed "None" option from tab view types. Consequently, any saved tab view types for bookmarked items will be reset to simple list.
* Rate menu will disappear from navigation bar after any future rating provided by the users. If you have already provided ratings, you can manully set RatingsProvided to true in the config file to hide the item.
* The library items in "This PC" page and the navigation bar items (in the sidebar) will always use the view type saved in the corresponding item (in the navigation edit view).
* As search can take quite long depending on the number of files and folders inside, the loading bar is now always visible in search page while loading items irrespective of the settings to show/hide loading bar.
* Search page should return pages quicker now (one at a time instead of waiting for more results).
* Added support for Windows 10 Version 1809 and newer. If you use older versions of Windows (prior than 2004) and encounter any bugs, please let us know.
* Fixed: Crash while opening settings in some cases.
* Fixed: Item being pasted while trying to paste path in default path settings.
* Miscellaneous improvements and bug fixes.




**Changelog for Version 0.40.x (April 5, 2021)**

* Show device information in properties in Home Page.
* Added opacity settings in the Theme Settings Page.
* Added setting to change open navigation pane length.
* Readded option to show/hide file operation icons in the title bar.
* Fixed bug that crashed the app while opening navigation bar.
* Improved reliability of opening the config file from the log viewer.
* Other bug fixes and improvements.




**Changelog for Version 0.39.x (March 24, 2021)**

* Settings fully migrated to the new experience. 
* Added basic property viewer (right click -> Properties). It currently shows some basic properties of a single selected file/folder or current tab folder.
* Added experimental extended search mode. Enable it from the settings.
* Added experimental limited support for MTP devices. Supported operations include creating folder and copying/pasting/deleting files/folders. 

	- Several features are currently unsupported which includes navigating to the parent folder, breadcrumbtrail, and moving (cutting) files/folders out of the MTP storage.

* Saving settings file and log file should be faster now.	
* Free and total spaces in hard drives should be shown more accurately and naturally (i.e. GB, MB, etc. as relevant) now.
* When switching from the dual pane to single pane mode, the first pane is now selected by default. Thanks to Parasec Glenkwyst for the bug report!
* Several new settings added in GUI:

	- Show/hide libraries, devices and drives, and recent files.
	- Reload drives every time This PC page is loaded.
	- Enable/disable delete confirmation dialogue before deleting items.
	- Default file operation for drag and drop.
	- Default page for new tabs.
	- Default view type for new tab (only applicable when specified path is set as the new tab option).
	- Show/hide cloud status. 
		
* Missing tile mode added in the navigation edit page.
* Other miscellaneous improvements and bug fixes.
	


**Changelog for Version 0.38.x (March 3, 2021)**

* Remembers the last state (expanded or collapsed) of navigation bar items/subitems. However, all the expanded items will be collapsed if the navigation bar itself is collapsed.
* Updated Settings Editor! Added shortcut Ctrl + P for the new settings editor (preview). For now, the settings icon still launches the context menu version of the settings.
* Color Themes added in the new settings editor. These color themes are experimental and will be updated in the future. Some color theme might look better in the dark base theme while others might look better in light base theme.
* Added option to check and install updates in the About Page.
* Added option to set default view types for bookmarked items in the bookmark editor.
* Improved the reliability of keyboard accelerators (shortcuts).
* Added keyboard accelerator Ctrl + H to switch between the single pane mode and dual pane mode. Thanks to Parasec Glenkwyst for the feature request!
* Clicking in empty space will now unselect selected items in single mode as well.
* Most recently used (MRU) items that are not available or accessible anymore are removed to avoid continues errors in the future.
* Updated Glyph (icon) for Pictures library. This will not show up for existing users unless the libraries are removed manually first.
* Bug fixes.




**Changelog for Version 0.37.x (February 23, 2021)**

* Updated logo.
* Added [Discord Link](https://discord.gg/nXmdRPJAdc) in About Page 
* Updated Hungarian translation. Thanks to Kristóf Kékesi!
* Loads thumbnail images after text to improve item loading speed.
* Change log in about page are now displayed with markdowntextblock instead of regular textblock.
* Improved method to track and update changes in the file system - especially delete and content change.
* Bug fixes.



**Changelog for Version 0.36.x (Skipped for special edition)**



**Changelog for Version 0.35.x (February 12, 2021)**

* Single click mode added as a result of popular demand.
* Flyout showing icons in Navigation bar edit view will now dismiss after selecting an icon.
* About Page now shows more information in selected language.
* Added analytics to understand and improve user experience.
* Added analytics to get handled exceptions (errors).
* Updated German Translation. Thanks to Parasec Glenkwyst!
* Date column is listed before Type column in detailed view mode to match Windows File Explorer's default behavior. Thanks to mgkai for feedback!
* Fixe bug that crashed the app when dragging multiple folders to the navigation bar.
* Link to the [Home Page](https://JPTGamesAndApps.Github.io/ShresthaFiles/) for Shrestha Files Added 



**Changelog for Version 0.34.x (Unreleased)**

* Updated sizes for this PC (Home Page) items. Thanks to Chomu_ for feedback!
* When dragging and dropping items in the same folder, it does not copy/move items anymore. Thanks to Chomu_ for feedback!
* Initial implementation of back and forward button in mouse to navigation back and forward. Let the developer know if it still does not work.
* Improved change tracker when items are deleted from outside the app.
* Added translations in Chinese (Simplified), Chinese (Traditional), Czech, French, German, Hindi, Hungarian, Italian, Japanese, Korean, Russian, Spaish, and Turkish. The translations are based on Google Translation, so some of the translations could be confusing and/or misleading.
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
 
 

**Version 0.21.x (November 15, 2020)**

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
