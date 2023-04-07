### Exif
Ini adalah Write-Up ketujuh saya dalam berlatih di [CTFLearn](ctflearn.com)

### Challenge
If only the password were in the image?

https://mega.nz/#!SDpF0aYC!fkkhBJuBBtBKGsLTDiF2NuLihP2WRd97Iynd3PhWqRw You could really ‘own’ it with exif.

### Cara Mengerjakan
Pertama-tama, kita download file foto dalam mega.nz yang diberikan. Kemudian langsung saya kita ketik perintah```exiftool (namafile)``` di Terminal kita, seperti :
```
exiftool 'Computer-Password-Security-Hacker - Copy.jpg'
```
Perintah terebut menghasilkan :
```
ExifTool Version Number         : 12.57
File Name                       : Computer-Password-Security-Hacker - Copy.jpg
Directory                       : .
File Size                       : 55 kB
File Modification Date/Time     : 2023:04:07 10:23:33-04:00
File Access Date/Time           : 2023:04:07 10:24:08-04:00
File Inode Change Date/Time     : 2023:04:07 10:23:34-04:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.02
X Resolution                    : 100
Y Resolution                    : 100
Exif Byte Order                 : Big-endian (Motorola, MM)
Resolution Unit                 : None
Y Cb Cr Positioning             : Centered
Exif Version                    : 0231
Components Configuration        : Y, Cb, Cr, -
Flashpix Version                : 0100
Owner Name                      : flag{3l1t3_3x1f_4uth0r1ty_dud3br0}
GPS Latitude Ref                : South
GPS Longitude Ref               : East
Quality                         : 60%
DCT Encode Version              : 100
APP14 Flags 0                   : [14], Encoded with Blend=1 downsampling
APP14 Flags 1                   : (none)
Color Transform                 : YCbCr
Image Width                     : 660
Image Height                    : 371
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:4:4 (1 1)
Image Size                      : 660x371
Megapixels                      : 0.245
GPS Latitude                    : 77 deg 17' 2.62" S
GPS Longitude                   : 44 deg 4' 7.30" E
GPS Position                    : 77 deg 17' 2.62" S, 44 deg 4' 7.30" E

```
Pada bagian ```owner name``` menampilkan ```flag{3l1t3_3x1f_4uth0r1ty_dud3br0}```
maka dapat disimpulkan kalau flag dalam challenge ini adalah :
```
CTFLearn{3l1t3_3x1f_4uth0r1ty_dud3br0}
```
