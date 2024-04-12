---
layout: page

title: Change History
description: Change History.

language: en
language_reference: change-history

published: true
order: 6
---

# Change History

## Version 4.58 released on 2024-03-17

Enhancements and improvements:

* Only for the .Net 4.6.1 variants: New version 0.28.2 of the exiv2 library integrated: lens recognition extended and minor bugs fixed.

Note: Due to the hosting provider going out of business, the previous contact e-mail address will be deactivated at the beginning of May. Please use the following address from now on: [quickimagecomment@gmail.com](mailto:quickimagecomment@gmail.com). Links in the program and in the help have been adjusted accordingly.

## Version 4.57 released on 2023-12-29

Enhancements and improvements:

- For users who start the program with different configurations via the command line (or adapted shortcuts): With the switch "/TitleSuffix:" a text can be defined, which is additionally displayed in the mask title of the main mask.
- Export of selected properties: Line breaks and line feeds (CR/LF) in metadata are replaced by spaces to avoid problems when importing into Excel.
- Only for the .Net 4.6.1 variants: New version 0.28.1 of the exiv2 library integrated: minor bugs have been fixed.
- Only for the .Net 4.6.1 variants: New version 0.21.1 of the library LibRaw integrated: minor bug fixed when decoding images from some Panasonic cameras.
- Metadata of iPhone .heic files and JPEG-XL files (.jxl) are displayed.

The following errors have been fixed:

- Occasionally the program could block if files in the displayed folder were added, changed or deleted by other programs.
- If files were deleted, the file counter at the bottom left was not updated.
- If a folder containing images with IPTC keywords was opened the first time the program was used (i.e. no configuration file saved yet), the program crashed.
- Refresh folder tree under Windows 11 caused a crash. Under other Windows versions, the update was incomplete if there were several folders with the same name.

## Version 4.56 released on 2023-09-04

Enhancements and improvements:

- Sequence number of the image is displayed below the image to the left of the file name.
- New internal fields "Image.MetaDataWarningsExiv2" and "Image.MetaDataWarningsNotExiv2". The fields allow to search for images with corresponding messages - separated by whether the message comes from Exiv2 or not. Since the search does not read the meta-data completely, the warnings may be incomplete.
- In the text field for the query in the mask "Search via Properties - Edit query" manual changes can be undone with Ctrl-Z and restored with Ctrl-Y. In each case, all changes since the text field was filled (when the mask is opened or when "Previous" or "Next" is pressed) are undone.

The following errors have been fixed:

- With each restart, the mask became smaller if scaling for Toolbar was set to a different value than for general scaling.
- When changing the scaling in full screen mode, a part of the mask could be cut off on the right and bottom.
- Variant for Windows XP only: Crash when saving changes to JPEG files.

## Version 4.55 released on 2023-06-02

Enhancements and improvements:

- New in mask "Image in own window": scrolling of images with keyboard or mouse; display of meta data in title bar (configurable).
- Mask "Predefined IPTC Keywords": By indenting, a hierarchy of keywords can be defined. This allows parts to be expanded and collapsed in the tree of the "IPTC Keywords" area, making it easier to select keywords.
- Optionally, a hint can be displayed if a non-predefined keyword has been assigned to an image. Such images can also be searched for. This is to facilitate consistent keywording.
- Search via properties: If the option "Save data on exit" is activated, the update of the data now starts when the program is started, not when the search mask is opened for the first time. This makes the updated data available earlier.
- Search via properties: If IPTC keywords is defined as a search field, a tree with the predefined keywords is displayed on the right in the lower area of the mask. Keywords to be searched for can be checked here.
- Search via properties: Some fields can have multiple values, e.g. IPTC keywords. For the search, these values are combined into a string, whereby the order is not defined. Therefore, the comparison operators have been removed for these fields, where the order of the single values is important.
- Search via properties: also, the second operator can now be "<>", "contains", "does not contain", "does not start with" or "does not end with".
- Search via properties: In an additional mask the query can be edited in a SQL-like syntax. This allows for more complex queries. In addition, a previously executed query can be selected to customize and re-execute it.
- Only for .Net 4.6.1 variants: New version 0.28.0 of library exiv2 integrated: some new tags and lens data; for ExifEasy more Exif properties are considered, so now ExifEasy properties of some images are filled, which were empty in the previous version.  
    Since exiv2 0.28.0 is no longer executable under Windows XP, the variant for Windows XP continues to be shipped with exiv2 0.27.5.1.

The following errors have been fixed:

- When changing "incl. cards for display only (\* ...)", the selection list was filled incorrectly, selection at the end of the list led to a program crash.

## Version 4.54 released on 2023-05-02

Enhancements and improvements:

- New mask "Scaling": magnification of all masks can be adjusted; separate scaling for toolbar and thumbnail/tiles. The zoom factor in mask "Customize mask" can still be used to scale individual masks. Mask-specific zoom factors can be disabled in "Customize mask" by setting the factor once to the general scaling factor.
- Some properties can also be changed in the "Overview", "Exif" and "IPTC" tabs. Modifiable values are displayed with a white background, non-modifiable with a light gray background. Details in the Help, Chapter 3.6, subsection "Input in the tabs for properties".
- Changed entries for artist, comment and IPTC keywords as well as in the configurable input area are marked by a light-yellow background. If the entry is reset, the background becomes white again. Instead of light-yellow, another color can be specified in the general configuration file.

The following errors have been fixed:

- When opening a sub-mask for the second time, the zoom factor from mask "Customize mask" mask was not taken into account.
- The program could crash at "Set file date to date image generated" if recording date was out of the allowed range for file date.

## Version 4.53 published on 2023-02-16

Enhancements and improvements:

- The selected files can be passed to other programs or to Windows batch scripts for further processing.
- The first reading and especially the updating of the read data for the search has been accelerated.
- Menu "File" has new entry to select a folder. A mask is opened where a folder can be selected in a folder tree or from a drop-down list with last selected folders. In this way the space for folder tree in main mask can be used for other information, e.g., a longer a list of files.
- New fields: "Image.DisplayImageErrorMessage" contains error message when displaying the image, "Image.MetaDataWarnings" contains warnings when reading metadata. Both information is already displayed in the Overview tab. The fields allow to search for images with corresponding messages. Since the meta data is not read completely during the search, the warnings may be incomplete

Following errors are corrected:

- The program could crash if unknown XMP tags were selected for modifying data.
- The program could crash if XMP-Struct fields (e.g. Xmp.iptcExt.LocationShown\[1\]/...) were configured for searching.

## Version 4.52 published on 2023-01-14

Enhancements and improvements:

- Variant for Net 4.6.1 and higher and if WebView2 Runtime is installed: When displaying the recording location on map, maps only for display (e.g. Google Maps and Bing Maps) can be hidden (which technically means disabling WebView2).  
    Background: Google Maps and Bing Maps require WebView2. However, WebView2 occasionally causes problems. Instead of disabling WebView2 via the general configuration file as before, you can now do this directly in the interface.
- Wildcard characters ("?" for any one character, "\*" for any number of characters) can now be used in the file filter.

Following errors are corrected:

- If the installed version of WebView2 did not match the components shipped with the program, the program could crash. In such cases, the "old" browser component is now used, but it does not support Google Maps and Bing Maps.
- Mask "Search via properties": With the button " Criteria of current file" the GPS data of the recording location were not taken over.
- Program could crash with "SplitterDistance must be between Panel1MinSize and Width - Panel2MinSize" when container with image details was made very small.

## Version 4.51 published on 2022-11-29

Enhancements and improvements:

- In the general configuration file map sources for Leaflet can be defined. With these maps - unlike the maps for "Map in Standard Browser" - the recording location can be changed.
- Images from JPEG-2000 (\*.jp2) and Photoshop (\*.psd) files can be displayed; previously only the metadata was displayed.

Following error is corrected:

- Program crash with exception "ctor System.NullReferenceException: Der Objektverweis wurde nicht auf eine Objektinstanz festgelegt. ExtendedImage.cs:Zeile 287.". Reported via AppCenter.

Note: Version 4.51 is also available for Windows XP 32-bit and .Net 4.0 Framework.

## Version 4.50 published on 2022-10-30

Enhancements and improvements:

- When displaying images, orientation information of manufacturer specific tags is also considered (up to now only Exif.Image.Orientation was used).
- As some RAW decoders rotate images according Exif.Image.Orientation, with the new menu item "Zoom/Rotate - RAW: Rotate after decoding" it can be selected, if rotation is applied after decoding or not. If it is selected on one image, it applies to all images read with the same decoder.
- Field entries from the "Overview", "Exif", "IPTC", "XMP" and "Other" tabs can be transferred to the table in the "Multiple image edit" tab via the context menu.
- Additional groups of Exif tags are displayed in the mask "Field definitions". If they were included in images, the values were also displayed in the previous version.
- File filter is changed: files are filtered for containing the filter string, not for starting with the filter string as before.

Following errors are corrected:

- In very rare cases, the lens name was displayed incorrectly.
- The save button was not enabled when geo data were cleared.
- The settings for "Image details" were not loaded correctly, so that one area became smaller with each new start of the program.

Note: Version 4.50 is available to run with .Net 4.6.1 (or higher) only. Net 4.6.1 was published already in November 2015 and so support for the very old .Net 4.0 is cancelled.

## Version 4.49 published on 2022-05-29

Enhancements and improvements:

- RAW image display is supported for more camera models.  
    The variant for .Net 4.6.1 has LibRaw integrated for displaying RAW images. When using the variant for .Net 4.0 or if LibRaw does not support the RAW format, a codec from the camera manufacturer must be installed to display the image. As an alternative, the Microsoft Raw Image Extension can be installed, which supports various RAW formats.

Following errors are corrected:

- Recording location on map: some maps could not be displayed when WebView2 was installed.
- Recording location on map: The maps "HikeBike.HikeBike" and "OpenMapSurfer.Roads" are no longer freely available. They have therefore been removed from the selection list.
- Program crash "Not a valid Win32 FileTime" due to invalid modification date/time of a file. Reported via AppCenter.

## Version 4.48 published on 2022-03-29

Enhancements and improvements:

- Under Windows 10 with Microsoft Raw Image Extension: DNG images from some Samsung models can now be displayed.

Following errors are corrected:

- The properties File.ImageSize and Image.CodecInfo were empty after saving.
- Opening a file via menu "File - Open" and entering a URL did not work.
- Program crash when file or folder not present in the command line was specified.
- It was not possible to delete all IPTC keywords, but only all but one.
- Program crash with exception " GeneralUtilities.comboBox_Resize_Unselect (Object sender, EventArgs e) System.ArgumentOutOfRangeException: InvalidArgument=El valor de '-1544604736' no es válido para 'start'. Nombre del parámetro: start". Reported via AppCenter.

Hints:

- To display RAW images, a codec from the camera manufacturer may need to be installed. As an alternative, the Microsoft Raw Image Extension can be installed, which supports various RAW formats. However, with the camera manufacturer's codec, the display could be faster. One can install a specific codec and the Microsoft Extension. The specific codec is then used for the corresponding images, for all others the Microsoft Extension.
- To make it easier to get started with QuickImageComment, there are now tutorials on YouTube. To access them, there is a new entry in the Help menu. Currently five videos cover the basics, more are to follow.

## Version 4.47 published on 2022-01-09

Enhancements and improvements:

- In the variant for .Net 4.6.1 and higher and if WebView2 Runtime is installed: Google Maps or Bing Maps can now also be used for the map display. The links that were previously used for "Map in Standard Browser" are used for this. With these links only display is possible, the coordinates cannot be changed.
- New version 0.27.5 of exiv2 library integrated, with new tag Exif.Photo.Gamma.

Following errors are corrected:

- Program crash if during meta data removal the image was used by another process.
- Map view: Search did not work in the variant for .Net 4, error message: Could not create SSL/TLS secure channel.
- If the mask "Settings" was exited with "Cancel", no values were displayed in the configurable input area.
- Application could freeze in views tile or thumbnails, if several files were changed within short time period.

## Version 4.46 published on 2021-10-22

Enhancements and improvements:

- Buttons can be defined for frequently used menu items. Self-defined buttons are displayed in the command strip, to the right of the predefined ones. Menu entry: "Tools – User defined buttons".

Following errors are corrected:

- Use of placeholders failed input validation for fields with specific format (e.g., for date). Values with placeholders are no longer checked.
- Program crash when main mask is minimized while making changes in mask "Adjust view".
- Program crash with exception "System.ArgumentNullException: Key cannot be null. Parameter name: key

## Version 4.45 published on 2021-10-09

Enhancements and improvements:

- The files can be sorted in ascending or descending order by Name, Size, Modified or Created using the menu "View", the context menu in file list or by clicking on the headers in view "Details".

Following errors are corrected:

- Configurable input area: Date changes via calendar (button right next to input field) did not work.
- Multiple image editing: displayed file was not marked, no update if files were modified outside QuickImageComment.
- The settings for "IPTC Keywords" were not loaded correctly, so that the field for free entry of keywords could become invisible.
- After renaming, renamed files were shown twice in file list.

## Version 4.44 published on 2021-07-08

Enhancements and improvements:

- If the "Thumbnail" or "Tile" view was selected for the file list, all images to be displayed with their thumbnails were loaded before a user input was accepted. Especially with RAW images this could take a long time. Now the images are listed with their filenames first and user input is accepted faster. The thumbnails are loaded in the background.
- Display of RAW images from some Nikon models accelerated.
- New version 0.27.4 of exiv2 library integrated, supports DNG 1.6 and Exif 2.32 (about 150 new tags).
- Placeholder: for date/time properties the format can be selected. New date/time format: Exif.

Following error is corrected:

- Program crash with exception "System.NullReferenceException: Referencia a objeto no establecida como instancia de un objeto.". Reported via AppCenter.

Hint:

- For those who modified the general configuration file: the (undocumented) parameter DisplayFullSizeImageCacheContent has been removed.

## Version 4.43 published on 2021-06-01

Enhancements and improvements:

- The user defined settings saved by name in mask "Adjust View" screen can be selected directly from the menu "View".
- Recording location on map: the entries of the last used positions can be renamed. This allows saved locations that are initially listed only with coordinates to be given a descriptive name. Entries that are no longer needed can be deleted.

Following error is corrected:

- Program crash when the last file in a folder was deleted.

Hint:

- The general configuration file as well as other configuration files are no longer located in the program directory itself but in a subfolder "config". The name of the general configuration file for 32-bit and 64-bit is now identical. This hint is only important if you want to customize these files yourself.

## Version 4.42 published on 2021-05-11

Following error is corrected:

- Severe error in caching: Depending on settings and folder content, caching could end up in 100% CPU load.

## Version 4.41 published on 2021-05-08

Enhancements and improvements:

- Search via properties: data can be stored into XML-file and loaded at next start of program. This can save much time for preparing search.
- Instead of just one image/video, several images/videos can now be handed over at the same time via drag-and-drop.
- New menu entry "Help – GitHub": Direct access to the new created GitHub repository with source code, issues (errors, feature requests) and discussions.
- If a mask-related help is available, it can be opened with F1.
- F11 is assigned to the function "Save image and switch to previous image". If this assignment is deleted (see mask "Customize mask", keyboard shortcut), F11 now toggles the view mode between normal and maximized.
- No direct impact for users, but mentioned to ensure transparency: To facilitate the analysis of crashes reported via Appcenter.ms, the events "Initialization finished", "Start closing program = Save configuration" and "End closing program" are logged in Appcenter.ms.

Following errors are corrected:

- Program crash if a file was deleted between filling file list from search mask and double clicking on that item.
- Program crash when starting program in English with Command strip set to "Hide - symbols in menu".
- Program crash with exception "System.ArgumentOutOfRangeException: InvalidArgument=El valor de '-1' no es válido para 'startIndex'. Nombre del parámetro: startIndex". Reported via AppCenter; similar to an error fixed in 4.40; the real cause has hopefully been found this time.
- Images loaded with Nikon NEF Codec 1.31.1 were displayed with wrong colors.

## Version 4.40 published on 2021-02-25

Following errors are corrected:

- Program crash with exception "System.ArgumentOutOfRangeException: InvalidArgument=Value mit dem Wert -1 ist für startIndex ungültig. Parametername: startIndex" resp. "System.ArgumentOutOfRangeException: InvalidArgument=El valor de '-1' no es válido para 'startIndex'. Nombre del parámetro: startIndex". Reported via AppCenter; unclear which activities caused this.
- Program crash with exception "System.NotImplementedException: No se puede implementar el método o la operación.". Reported via AppCenter. Reason must have been a notification of change in file system which was not relevant for QuickImageComment and thus this type of notification will be ignored in the future.
- Program crash when program was minimized and then terminated.
- Program crash with exception "System.IO.FileNotFoundException: No se pudo encontrar el archivo '....tif'.". Reported via AppCenter. The cause is probably that a file was deleted between filling the file list in the main screen and selecting it.

## Version 4.39 published on 2021-02-13

Enhancements and improvements:

- Images/videos can be searched via position on map with radius.
- Map view: Position can be entered via coordinates (degrees in decimal or with degrees/minutes/seconds).
- New fields "Image.GPSsignedLatitude" (negative values for south) and "Image.GPSsignedLongitude" (negative values for west), primarily for search for images via position.
- If a file is selected that is write-protected or to which access is generally not permitted, the controls for changing data are locked. A note "write-protected" or "no access" appears in the footer.
- The maximum number of GPS positions that are stored for the search list of the map display now applies separately to unnamed entries that were created by marking them on the map and to named entries that are the result of a search (recognizable by a speaking name such as "Düsseldorf Hbf"). This is to prevent new unnamed entries from gradually displacing named entries from the list.

Following errors are corrected:

- Program crash during search if an image was deleted between reading data and starting the search.
- Program crash if an empty folder was selected, a position in the map was selected and then the folder was changed.
- Program crash without message when opening an image with tag of type XmpSeq of length zero.
- Program crash when trying to save a read-only file.
- Program crash when trying to open the calendar in configurable input area in case the corresponding input field was empty.
- Program crash when changing setting configuration in mask "Adjust View".
- If no access to a file was possible, the Exif/IPTC/XMP data of the previously read file was displayed

## Version 4.38 published on 2021-01-21

Enhancements and improvements:

- Program starts faster.
- Export files and user configuration are written with encoding UTF-8 (including Byte Order Mark). Old configuration files still can be read.
- New menu entry in main mask: Help - Webpage - Change history.
- Date in mask "Check for new version" is displayed in the format defined in the Windows system settings. In addition, the days since the last check are displayed.

Following errors are corrected:

- The error reports submitted using Microsoft AppCenter did not contain the complete call hierarchy (stack trace). Therefore, reported errors could not be eliminated.

## Version 4.37 published on 2020-11-30

Enhancements and improvements:

- Images/videos can be searched via their properties.
- Mask "Image in own window" is opened for each selected image if several images are selected in main mask and contains a configurable table with properties.
- New fields "Image.ArtistCombinedFields" and "Image.CommentCombinedFields" contain the values of different fields for artist and comment respectively, which makes search for them easier.
- Only for Windows 10 with .Net 4.6.1: With the help of the Microsoft AppCenter, error reports of program crashes and elementary anonymous usage data can be transmitted to the developer. Crashes can thus be reported easily. The developer receives information that can help with further development.
- Separate zip files with program variants (32 and 64 bit) for older operating systems with .NET 4.0 available

Following errors are corrected:

- Level 2 context menu entries and tooltip texts were not translated.
- Tag names and descriptions were not translated if the program was started in German.
- Tab "Multiple image edit": If the main mask was small, the checkboxes for changeable properties were not visible.
- The memory still available for buffering images was determined incorrectly, so that fewer images were buffered than would have been possible - which may have made image switching slower.

## Version 4.36 published on 2020-08-26

Enhancements and improvements:

- This version now requires .NET framework 4.0 (or higher).
- Main Memory display changed to "Physical memory in use by active processes". This is the value, which is usually shown in task manager.
- Redesign of folder tree view: now includes also network devices (previously only network locations)
- Folder tree view and file view are updated, when folders or files are added, changed or deleted outside the program. No update if files are changed outside, which are selected and have unsaved changes inside the program.
- In properties tables, the change of width of column "value" is considered when displaying next image. Up to now width was determined always new, based on longest entry considering a fixed maximum length.
- New entry in menu "Tools" to show map with standard browser. This allows displaying Google maps, which is not supported by the built-in browser component. URLs for this display are stored in general configuration file. They can be changed there, new URLs can be added. Note: change of GPS-data is not possible here.
- Exif and IPTC data are stored in UTF8, which in general is better supported by other programs to display Meta data. Via mask "Settings", it can be switched off, which means data are stored in the same way as in previous versions.
- Exif.Photo.UserComment is written with charset=Unicode, which in general is better supported by other programs to display Meta data. Via mask "Settings", it can be switched to Ascii, which means data are stored in the same way as in previous versions.
- When reading Exif and IPTC data, it is detected, if they are coded in UTF8 and are converted if needed. This reduces the probability that data written by other programs are not shown correct, if they contain special characters like the German umlauts (ä, ö, ü).
- New version 0.27.3 of library exiv2 integrated, contains error fixes and some new tags.

Following errors are corrected:

- GPS changes done via map were not saved.
- Several other minor errors

Hint:

- This version now requires .NET framework 4.0 (or higher).

## Version 4.35 published on 2019-11-17

Enhancements and improvements:

- New version 0.27.2 of library exiv2 integrated with error fixes, additional lens data, Nikon/AutoFocus and sony/FocusPosition metadata.
- The tags Exif.Image.XPAuthor, Exif.Image.XPComment, Exif.Image.XPKeywords, Exif.Image.XPSubject and Exif.Image.XPTitle can be now edited as strings. As their type is Byte previously they could be edited only as byte array.
- Exif.Image.XPComment and Exif.Image.XPTitle can be chosen as tags to store input in text field for comment in the center of main mask, Exif.Image.XPAuthor as tag for input in combo box for the name of the artist (author).

Following errors are corrected:

- Sometimes files were displayed not sorted in the list.

## Version 4.34 published on 2018-12-28

Enhancements and improvements:

- Mask to insert and edit placeholders added.
- Network folders and standard folder "Pictures" are shown in folder tree.

Following errors are corrected:

- Program crashed during multi-edit, if comment was not filled and "append comment" was selected.
- Program crashed after multiple pressing Ctrl-A in file list.
- Export of properties with several values (e.g. of type LangAlt, XmpSeq) was incomplete.

## Version 4.33 published on 2018-12-02

Enhancements and improvements:

- Data templates can be defined to set several properties in one step.
- Marker for recording location (and with this the coordinates) can be removed with right mouse button.
- Buttons and menu items are enabled/disabled based on context.
- When not saved changes may be lost e.g. when selecting other images or stopping the program, user has three options: save before continuing, continue without saving and cancel the new activity. Previously there were two options depending on situation.
- Escape-key and Reset-button are usable also when multiple files are selected.

Following errors are corrected:

- Instead of mask related help always information about licenses was shown.
- Memory issues when exporting selected properties of images in folder.

## Version 4.32 published on 2018-09-21

Enhancements and improvements:

- Via configuration file showing of hidden files and folders can be activated.
- Minor improvements in error handling.
- Upgrade von Leaflet (component for showing maps) auf 1.3.4
- Map display can be selected from several sources, including topographic, satellite and hybrid.

Following errors are corrected:

- Search for location in map view did not work (request was not accepted by OpenStreetMap).

## Version 4.31 published on 2018-03-01

Enhancements and improvements:

- In tabs for Exif, IPTC, XMP and other properties, fields can be marked and per context menu (right mouse button) added into the area of changeable properties or in tab Overview.
- In tab Overview, fields can be marked and per context menu (right mouse button) added into the area of changeable properties.
- In XMP property tab, language is added in column type for entries of type LangAlt as this type allows different values for different languages.
- Improved check of placeholders.

Following errors are corrected:

- Misleading message "For … saved value … differs from target value ...", when comment should be stored in Xmp.dc.description or Xmp.dc.title.
- During multi image edit with placeholders for all images the replacement of first image was selected. Now replacement is done for each image individually.

## Version 4.30 published on 2017-11-05

Enhancements and improvements:

- Via Drag-and-Drop and the menu entry "File - Open" images can be also opened via URLs. For this purpose they are downloaded into the folder "Downloads".
- Several files can be deleted (up to now only single files could be deleted).
- The file properties "Created at" and "Modified at" can be set to the date/time when image was generated (Exif.Photo.DateTimeOriginal).
- New version 0.26 of library exiv2 integrated with about 250 new tags, especially XMP and reading of an initialization file with assignments of lens names to lens Ids (for display of ExifEasy.LensName).

Following errors are corrected:

- With some XMP-entries (seen with photos taken with iPhone) the program crashed.
- During Multi-Saving the program could sometimes "freeze".

## Version 4.29 published on 2017-02-25

Enhancements and improvements:

- Display of image details possible in separate mask (especially useful if two monitors are available). Several windows can be opened to compare details of several images.
- The visible area of image in "image details" can be shifted by moving the mouse with left button pressed.
- Recording location of an image can be shown on a map and associated data can be changed. This can be done either in one of the areas of the main mask or in a separate mask.

## Version 4.28 published on 2016-12-22

Following errors are corrected:

- Program crashed when saving in view modus "tiles" or "thumbnails".

## Version 4.27 published on 2016-12-18

Enhancements and improvements:

- Performance improvement during starting the program.

Error corrections:

- After deleting an image a wrong thumbnail was displayed. This error is corrected.

## Version 4.26 published on 2016-11-17

Error corrections:

- An error in display is corrected.

## Version 4.25 published on 2016-11-13

Enhancements and improvements:

- Accept a folder or file name as command line argument, which allows using the program via "Send to" in Windows explorer context menu.
- Files can be opened via drag-and-drop.
- New menu entry "File - Open" to open folders or files via entering the full name (i.e. including complete path).
- Mask "Field definitions": allows defining a list of valid values, which are used in main mask to check input in configurable input area.
- Main mask: if Exif.Image.Orientation is added to configurable input area, a drop down list shows the valid (numeric) values together with an explanation (e.g. "bottom, left (180° + horiz.flip)"). After saving changes of Exif.Image.Orientation, image will be rotated accordingly.
- Performance improvement when opening a folder.
- During scrolling via scrollbar in file list with view tiles or thumbnails, no new thumbnails are created. Only already existing thumbnails are displayed. In this way scrolling can be much faster. During fast rotation of mouse wheel, update of thumbnails is avoided as well.
- Main mask: Size and spaces in tile and large icon view is configurable via general configuration file.
- Main mask: new buttons to go to first and last image in folder.

Error corrections:

- An error in rotating images based on orientation given in Exif-properties is corrected.

## Version 4.24 published on 2016-09-27

Enhancements and improvements:

- In mask "Field definitions" for date values five more formats can selected. These formats can be adjusted individually via the general configuration file.

Error corrections:

- In case an error occurred during reading meta data, no changes of Meta data was possible, even not for those, which were displayed correct. This error is corrected.
- Translation to English was not complete on computers not using code page 1252. This also resulted in an error when starting the program. This error is corrected.

## Version 4.23 published on 2016-09-22

Enhancements and improvements:

- Storage location for user settings can be selected:
  - %Appdata%:  
        If several users are created on the computer, each user has his own settings.  
        Settings are kept during upgrade on newer program version.  
        Program folder can be write-protected.
  - Program folder:  
        Recommended for portable usage on USB-stick: the settings are on USB-stick too, no settings will be stored on other computer.  
        When upgrading to a newer program version, settings need to be copied manually or program files in currently used folder have to be overwritten.
- In mask "Field definitions" for date values following formats can be selected:  
    Local date/time format (according system settings)  
    ISO date/time format (e.g. 2016-09-20T18:25:00)
- In case an error occurred during reading Meta data, no Meta data were displayed. As these errors were related to single properties only (which usually are of no interest for the user), now Meta data are displayed.
- As (according to experience) errors in Meta data usually did not affect properties of interest for the user, one setting was changed: In this case no message box is displayed any longer. If desired, this can be changed via mask "Settings".

Error corrections:

- If no internet connection was available, the program terminated when checking for a new version. This error is corrected.

## Version 4.22 published on 2016-05-20

Enhancements and improvements:

- Mask "Adjust view": View can be adjusted so that more sections can be displayed side by side instead of one above the other. Several user defined views can be saved with names.
- Main mask - configurable input area: For entering a date, a calendar can be opened (new button on the right hand side of the input field).
- Main mask: Via context menu the mask "Field definitions" can be opened directly in order to change the fields displayed in the configurable input area, in tab "Overview", in file display with view "Tiles" and in the table for "Multi image edit".
- Mask "Remove meta data": Via command buttons the mask "Field definitions" can be opened directly to select meta data to remove resp. the exceptions.
- Mask "Rename files": The drop downs for "Field" and "sort by" have a new entry "new field", via which directly the mask "Field definitions" can be opened in order to customize the drop down list.
- Mask "Change recording date and time": Drop down for grouping (top left) has a new entry "all" as well as "other grouping", via which directly the mask "Field definitions" can be opened in order to customize the groups.
- Mask "Compare files": Via command button "Configure hidden columns" the mask "Field definitions" can be opened directly in order to configure the columns not to compare.
- Export: Selected properties of images in folder: Before starting the export, a query appears to open the mask "Field definitions" in order to select the properties to be exported.

Error corrections:

- Video data were not displayed correct.
- Check for new version compared with previous version (and thus by mistake announced, that a new version is available).
- Several other minor errors.

## Version 4.21 published on 2015-10-15

Enhancements and improvements:

- New version 0.25 of library exiv2 integrated with about 350 new tags, especially XMP, Panasonic and Casio.

Error corrections:

- Mask "Field definitions": After pressing the button "Meta Date 1" the program crashed. This is corrected now.

## Version 4.20 published on 2015-03-29

Enhancements and improvements:

- Adjustments for screens using DPI values higher than 96  
    This version is now also usable when DPI is set to a value higher than 96, using Windows configuration "Make text and other items larger or smaller" or "Set custom text size (DPI)".

Error corrections:

- The last two versions were not running on Windows XP. This is corrected now.

## Version 4.19 published on 2015-02-08

Enhancements and improvements:

- First version available in English  
    New languages can simply be made available by adding language files (if there is someone who provides the necessary translations).