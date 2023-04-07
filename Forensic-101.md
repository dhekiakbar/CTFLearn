### Forensic-101

Challenge ini adalah challenge Ketiga saya saat mencoba belajar di [CTFLearn](ctflearn.com)

### Pertanyaan
Think the flag is somewhere in there. Would you help me find it? https://mega.nz/#!OHohCbTa!wbg60PARf4u6E6juuvK9-aDRe_bgEL937VO01EImM7c

### Cara Mengerjakan
Pertama-tama, saya mendownload gambar minion yang ada di dalam mega.nz. Kemudian saya membuka terminal dan mengetik command

```
exiftool 95f6edfb66ef42d774a5a34581f19052.jpg
```

Ternyata tidak ada petunjuk dalam exifnya, kemudian saya mencoba
```
file 95f6edfb66ef42d774a5a34581f19052.jpg
```

Dan ternyata hanya mendapatkan hasil

```
95f6edfb66ef42d774a5a34581f19052.jpg: JPEG image data, JFIF standard 1.01, aspect ratio, density 1x1, segment length 16, progressive, precision 8, 236x218, components 3
```

Maka, setelah kegagalan tadi, sayapun mencoba command

```
strings 95f6edfb66ef42d774a5a34581f19052.jpg
```

Dan untungnya, command tersebut menunjukan hasil yang baik, yaitu:

```
JFIF
 , #&')*)
-0-(0%()(
((((((((((((((((((((((((((((((((((((((((((((((((((
L?~f
:UwR
y>2|
*'?-
yhH_&
Lmz'
 +f[
!"1$246B`35A
au>
~b*D
F_X:D
[ElC
him8
lr|.
L{2^
]]te
tBfE
j_s7Os/[i
W="'
"fkO
G&,ke:
eM_F
8O:J
9)/m>&
[P{!
}EI5#
a~Wt,1
]<e<
g:rc
"1Pa
ujM^P
P#3a
vFGO
ZniFi
%a      ?}
2AQaq 0B#@r
\xr>
\37g
4=i#N
F:Jx
.`Ot
v[xU
|='u
{~T{@
LX.9
?mBx
L1QG
lIYB+
|] %
QTj?:
$*,-
pk4D
4R gX
$mmk
_QSK
b)^L
a[T=
mpj<N;
!1AQaq
x'<L
we|C{
iiR8
"'A*
aZ(4
cj}+
NL7'4
u-kF3n
x       cd
s}F3_Y
$+Ym
zrsq
f}]@
L&/F
&F'$,
| *
ktWxn
 yLX*s]
pT)J
eR-3
SG=3\Y
JK%0
h"(p
!01Q
%^cJ
H|cO
!10AQ
'([P
!1AQaq
s`%"
X`3d'
'P]!
;#_l
ABx=~
"r&"
0YAP
ch-h
XoXrl
l0Je
V^_W
xp7p
v{*{8
=k"$TW3G
1)j!
7y}U
<~0GD
n%CeoQ=m8
`"n<P
 i}\D
X`(
8kF=
~9%]Tn
flag{wow!_data_is_cool}
$lqU
AG{u
Xm*CnC
@'hnQ
ax+p
bdQG
D_ O

```

Di dalam hasil diatas, sangat jelas ada flag yang tersimpan. Yaitu :

```
flag{wow!_data_is_cool}
```
