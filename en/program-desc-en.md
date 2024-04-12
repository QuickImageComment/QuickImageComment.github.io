QuickImageComment displays EXIF, IPTC, and XMP properties of digital images (e.g., JPEG and TIFF as well as some RAW formats) and allows to edit them. Especially editing of user comment and artist (author) is supported by using the last entered or predefined values. Metadata (XMP) in video files are displayed.

### Overview of features:
- Display of all EXIF, IPTC and XMP properties of images, as well as some other file properties such as modification date.
- Display of meta data (XMP) of video files as well as (depending on the Windows version and, if necessary, installed components) display a frame of the video.
- Images or videos can be searched via their properties and recording location on map.
- In addition to the full lists of EXIF, IPTC and XMP properties a list of properties is displayed, which is configurable.
- In addition to user comment and artist further EXIF, IPTC and XMP properties can be changed. The list of modifiable properties can be configured. 
- Data templates can be defined to set several properties in one step.
- Via placeholder it is possible to copy values of properties in others.
- Changes can be carried out simultaneously for two or more files.
- EXIF, IPTC and XMP properties can be deleted, thereby exceptions can be defined. Single properties can be deleted selectively.
- Files can be renamed using Exif, IPTC and XMP properties.
- The EXIF, IPTC and XMP properties contained in the files can be compared.
- A special mask is used to synchronize the recording time of a set of images taken with different cameras. Images are grouped by properties (mostly camera model). For each group, a shift of the recording time can be entered. Then the images are immediately sorted in order to check whether the images are then in the correct timely order.
- Selected image properties of all images/videos in a folder (including any subfolders) can be exported to a text file.
- All image properties of selected images/videos can be exported to text files (one file per image).
- Display of image details with graphical and numerical representation of brightness and RGB values.
- Display recording location in a map using the GPS coordinates; change of coordinates by selecting a position on the map.

Further processing of the images (e.g., adjusting the contrast and brightness) is not the purpose of this program.

For reading and changing the EXIF, IPTC, and XMP properties the library exiv2 is used. On [www.exiv2.org](www.exiv2.org) a description of this library can be found as well as extensive information and links to Exif, IPTC and XMP. The formats supported by exiv2 are documented here:
- Images: [http://dev.exiv2.org/projects/exiv2/wiki/Supported_image_formats](http://dev.exiv2.org/projects/exiv2/wiki/Supported_image_formats)
- Videos: [http://dev.exiv2.org/projects/exiv2/wiki/Supported_video_formats](http://dev.exiv2.org/projects/exiv2/wiki/Supported_video_formats)

For displaying RAW images, the LibRaw library is integrated. If the camera manufacturer's codec or the Microsoft Raw Image Extension (which supports various RAW formats) are installed, they are used and then display is usually faster. One can install both a specific codec and the Microsoft Extension. The specific codec is then used for the corresponding images. For all others first the Microsoft Extension is tried and as last option the integrated LibRaw library. For the display of the metadata no codec is needed.

The program runs under Microsoft Windows 7, 8, 10 and 11 and is available as 32-bit and 64-bit variant. German or English can be selected as the language. There is also a variant with slightly reduced functionality available, which runs on Windows XP with .Net 4.0 framework.

QuickImageComment is free software; you can use it under the terms of the GNU General Public License as published by the Free Software Foundation.
