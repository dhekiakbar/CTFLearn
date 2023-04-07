### Taking LS
Ini adalah Challenge keenam saya di [CTFLearn](ctflearn.com)

### Pertanyaan 
Just take the Ls. Check out this zip file and I be the flag will remain hidden. https://mega.nz/#!mCgBjZgB!_FtmAm8s_mpsHr7KWv8GYUzhbThNn0I8cHMBi4fJQp8

### Cara Mengerjakan 
Pertama-tama, download dahulu file yang ada di dalam mega.nz yang diberikan. Kemudian Ekstak filenya
Setelah Meng-Ekstrak, akan ada 2 folder yang kita dapat. Yaitu "The Flag" dan "_MACOSX" 

Karena kita tidak menggunakan MAC-OS, maka kita hanya akan membuka folder "The Flag"
Didalam folder tersebut awalnya hanya akan terlihat 1 file, yaitu "The Flag.pdf" yaitu file pdf yang terkunci
maka dari itu kita akan menggunakan perintah ```ls``` di dalam folder "The Flag". Caranya adalah dengan :
```
cd 'The Flag'
ls -a
```
maka akan terlihat folder ".ThePassword"
Lalu, kita pindah ke folder tersebut dengan mengetik :
```
cd .ThePassword
```
Setelah itu, kita akan menemukan "ThePassword.txt" yang berisi :
```
Nice Job!  The Password is "Im The Flag".
```
Kembali lagi ke "The Flag.pdf", dan gunakan "Im The Flag" Sebagai Password dalam membuka pdf tersebut
didalam "The Flag.pdf' berisi flag, yaitu :
```
Here is the flag: ABCTF{T3Rm1n4l_is_C00L}
```
