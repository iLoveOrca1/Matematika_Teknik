# Pengenalan Determinan Matriks

Determinan matriks adalah sebuah nilai skalar (angka tunggal) yang dihitung dari elemen-elemen matriks persegi, berfungsi sebagai parameter yang merangkum sifat matematis dari matriks tersebut.

Intinya, determinan adalah satu angka tunggal yang dihasilkan dari matriks persegi. Angka ini sangat fundamental karena dua hal:

- Membantu kita memahami sifat-sifat matriks persegi tersebut.
- Menjadi kunci untuk mempelajari bagaimana ia mengubah suatu ruang (*transformasi linear*).

Ada 2 jenis matriks berdasarkan determinannya:
1. Jika $|A| = 0$, maka matriks $A$ itu disebut __matriks singular.__
2. Jika $|A| \neq 0$, maka matriks $A$ itu disebut __matriks nonsingular.__

Ada pula sifat-sifat determinan seperti:
1. $|A^t| = |A|$ 
(Determinan yang ditranspose dan tidak di transpose bernilai sama)
2. $|A^{-1}| = \frac{1}{|A|}$ 
(Determinan $A$ inverse sama dengan satu per determinan $A$)
3. $|AB| = |A| . |B|$ 
(Determinan AB sama dengan determinan A dikali determinan B)
4. $|A^n| = |A|^n$
5. $|k.A| = k^n . |A|$
($n$ adalah ordo matriks. Disini $k$ adalah skalar atau konstanta (Nanti akan kita bahas))


# Pencarian determinan matriks

Misal diketahui determinan matriks $A$. Determinan ini bisa ditulis $det A$ ataupun $|A|$

> Determinan matriks hanya ada pada matriks persegi

## Pencarian determinan Ordo 2 * 2
Cara mencarinya cukup gampang, kita tinggal mengkali-silangkan elemen pada diagonal utama lalu mengurangkan keduanya.

$$
A = \begin{pmatrix} 
a & b \\ 
c & d 
\end{pmatrix}
$$

Melalui hasil tersebut dapat disimpulkan bahwa rumus pencahariannya adalah seperti berikut:

$$
|A| = ad - bc
$$

## Pencarian determinan Ordo 3 * 3
Kita akan menggunakan metode __SARRUS__. Nilai determinan dihitung dengan menjumlahkan hasil kali elemen pada tiga diagonal menurun, lalu menguranginya dengan total hasil kali elemen pada tiga diagonal menaik.

Sebagai contoh, kita diberikan sebuah matriks $B$ sebagai berikut.

$$
B = \begin{pmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{pmatrix}
$$

Pada awal, kita akan menambahkan kolom 1 dan 2 pada samping matriks. Secara visual, susunan Metode Sarrus akan terlihat seperti ini:

$$
|B| = \begin{vmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{vmatrix}
\begin{matrix}
a & b \\
d & e \\
g & h
\end{matrix}
$$

Berikut visualisasi perkalian silangnya:

![Determinan 3 * 3](image/Determinan3x3.png)

- __Garis kuning:__ Kalikan elemennya lalu jumlahkan.
- __Garis biru:__ Kalikan elemennya lalu jumlahkan. 

Hasil akhirnya adalah total garis kuning dikurangi total garis biru.

Dengan ini, maka rumus mencari determinannya adalah seperti ini:

$$
|B| = aei + bfg + cdh - ceg - afh - bdi 
$$

Bisa juga disederhanakan menjadi seperti ini:

$$
|B| = (aei + bfg + cdh) - (ceg + afh + bdi) 
$$


