### My Blog
Challenge ini adalah challenge Kedua saya saat mencoba belajar di [CTFLearn](ctflearn.com)

### Pertanyaan



Hi, I'm Noxtal! I have hidden a flag somewhere in my Cyberworld (AKA blog)... you may find a good application for your memory. ;)

Note: This is my real website (thus no deadly bug to exploit here). You might want to read some of my content (writeups, tutorials, and cheatsheets). I would be glad to receive any kind of feedback.

[Click here](https://noxtal.com/) to access it, have fun checking my blog out! Cheers!

Hint: replace the flag{} part with CTFlearn{}.

### Cara mengerjakan

Pada awal membuka kita akan disuguhkan tampilan web blog pada umumnya. Lalu saya kemudian mencoba membuka beberapa bagian webnya, dan tidak menemukan apa apa

Kemudian saya inspect webnya, dan saya tidak menemukan apa apa...

Sayapun membuka kolom komentar dan menemukan petunjuk bahwa flagnya berada di bagian local-storage yang dapat diakses dengan :
```
Klik Blog

klik kanan > Inspect > Storage > Local Storage > blog.noxtal.com
```
Kemudian cari Noxtal.com, maka akan terlihat flagnya

```
flag:"flag{n7f_l0c4l_570r463_15n7_53cur3_570r463}"

```
