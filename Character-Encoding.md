### Character Encoding
Ini adalah Challenge kelima saya di [CTFLearn](ctflearn.com)

### Pertanyaan
In the computing industry, standards are established to facilitate information interchanges among American coders. Unfortunately, I've made communication a little bit more difficult. Can you figure this one out? 41 42 43 54 46 7B 34 35 43 31 31 5F 31 35 5F 55 35 33 46 55 4C 7D

### Cara Mengerjakan
Sebelum memulai, saya mencari dulu jenis karakter pada urutan angka dan huruf dibawah ini
```
41 42 43 54 46 7B 34 35 43 31 31 5F 31 35 5F 55 35 33 46 55 4C 7D
```
Sayapun menemukan bahwa karakter diatas merupakan Hexadecimal. Maka dari itu, saya melakukan konversi dari Hex ke ASCII. Dalam kasus saat ini saya menggunakan konverter online yang tersedia di internet, dan menemukan hasil seperti berikut:
```
ABCTF{45C11_15_U53FUL}
```
Maka, dapat disimpulkan bahwa flag yang kita temukan adalah :
```
CTFLearn{45C11_15_U53FUL}
```
