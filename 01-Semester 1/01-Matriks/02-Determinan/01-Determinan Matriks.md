# Determinan Matriks

Misal diketahui determinan matriks *A*. Bisa ditulis __det A__ ataupun *|A|*

> Determinan matriks hanya ada pada matriks persegi ya

# Ordo 2 * 2
Cara mencarinya cukup gampang, kita tinggal mengkali-silangkan elemen pada diagonal utama lalu mengurangkan keduanya.

Contoh

$$
A =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

Maka 
-> __det A__ = ad - bc

# Ordo 3 * 3
Kita akan menggunakan metode Sarrus
Misal diketahui matriks B

$$
B =
\begin{pmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{pmatrix}
$$
Kita akan mengali silangkan matriks tersebut 
$$
|B| = 
\begin{vmatrix}
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