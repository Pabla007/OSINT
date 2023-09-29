
Will install a Exif tool that is not installed 
```
apt install libimage-exiftool-perl
```

![[Pasted image 20230925114922.png]]

Already installed in our i guess that .install tools i have run earlier might have installed it for us.

Image Location: https://cdn.fs.teachablecdn.com/G0XVtAlUTOaG2LIh7UVV
Will simply open it in browser and than safe it in Desktop 

![[Pasted image 20230925120327.png]]

```
─# exiftool dog.JPG 
ExifTool Version Number         : 12.65
File Name                       : dog.JPG
Directory                       : .
File Size                       : 3.9 MB
File Modification Date/Time     : 2023:09:25 06:26:09+00:00
File Access Date/Time           : 2023:09:25 06:26:09+00:00
File Inode Change Date/Time     : 2023:09:25 06:26:09+00:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
Exif Byte Order                 : Big-endian (Motorola, MM)
Make                            : Apple
Camera Model Name               : iPhone 4S
Orientation                     : Rotate 90 CW
X Resolution                    : 72
Y Resolution                    : 72
Resolution Unit                 : inches
Software                        : 5.0.1
Modify Date                     : 2012:03:11 12:01:53
Y Cb Cr Positioning             : Centered
Exposure Time                   : 1/1842
F Number                        : 2.4
Exposure Program                : Program AE
ISO                             : 64
Exif Version                    : 0221
Date/Time Original              : 2012:03:11 12:01:53
Create Date                     : 2012:03:11 12:01:53
Components Configuration        : Y, Cb, Cr, -
Shutter Speed Value             : 1/1842
Aperture Value                  : 2.4
Brightness Value                : 10.39054726
Metering Mode                   : Multi-segment
Flash                           : Off, Did not fire
Focal Length                    : 4.3 mm
Subject Area                    : 1631 1223 881 881
Flashpix Version                : 0100
Color Space                     : sRGB
Exif Image Width                : 3264
Exif Image Height               : 2448
Sensing Method                  : One-chip color area
Exposure Mode                   : Auto
White Balance                   : Auto
Focal Length In 35mm Format     : 35 mm
Scene Capture Type              : Standard
Sharpness                       : Normal
GPS Latitude Ref                : North
GPS Longitude Ref               : West
GPS Altitude Ref                : Above Sea Level
GPS Time Stamp                  : 17:30:26
GPS Img Direction Ref           : True North
GPS Img Direction               : 191.2603175
Compression                     : JPEG (old-style)
Thumbnail Offset                : 914
Thumbnail Length                : 9959
Image Width                     : 3264
Image Height                    : 2448
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Aperture                        : 2.4
Image Size                      : 3264x2448
Megapixels                      : 8.0
Scale Factor To 35 mm Equivalent: 8.2
Shutter Speed                   : 1/1842
Thumbnail Image                 : (Binary data 9959 bytes, use -b option to extract)
GPS Altitude                    : 182 m Above Sea Level
GPS Latitude                    : 41 deg 40' 43.20" N
GPS Longitude                   : 83 deg 39' 21.00" W
Circle Of Confusion             : 0.004 mm
Field Of View                   : 54.4 deg
Focal Length                    : 4.3 mm (35 mm equivalent: 35.0 mm)
GPS Position                    : 41 deg 40' 43.20" N, 83 deg 39' 21.00" W
Hyperfocal Distance             : 2.08 m
Light Value                     : 14.0
```

The methodology is same that we have seen earlier the only difference is that we have to use command line tools and not the web app tools.

