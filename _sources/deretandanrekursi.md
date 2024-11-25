---
title: DERETAN DAN REKURSI

---

# DERETAN DAN REKURSI
**Deretan(Sequence)**
* Deretan adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu.
* Definisi: Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.
*    N = {1, 2, 3, 4, … }
   S misalnya {2, 4, 6, 8, …},   {1/3, 1/5, 1/7, …},  dsb
* Notasi deretan: $\{a_n\}$
* Deretan umumnya dinyatakan dalam suatu formula, misalnya:
$\{a_n\}$ :2*n* 
$\{a_n\}$ :1/*n*
$\{a_n\}$ :7-3*n*
Dalam konteks matematika, deretan sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu.
Misalnya:
1. Deretan bilangan ganjil: 1,3,5,7,…
2. Deretan bilangan genap: 2,4,6,8,…
3. Deretan bilangan yang membentuk deret aritmetika: 3,6,9,12....

# Contoh-contoh deretan dan formulanya:
**1.Deret Aritmatika**
* Deret dengan pola kenaikan atau penurunan tetap.
**Contoh**: 2,5,8,11,14,…
**Rumus suku ke-n:** $U_n = a + (n - 1) \cdot b$
**Penjelasan:**
Di mana:
-𝑎: suku pertama
-𝑏: beda (selisih antar suku)
-𝑛: nomor suku yang dicari

**2.Deret Geometri:** Deret dengan pola kelipatan tetap
**-Contoh**: 3,6,12,24,48,…
**Rumus suku ke-n:** $U_n = a \cdot r^{(n-1)}$
**Di mana**:
-𝑎: suku pertama 
-𝑟: rasio (perbandingan antar suku,
-𝑛: nomor suku yang dicari

**3.Deret Bilangan Kuadrat**: Deret dengan pola nilai berupa kuadrat bilangan bulat
**-Contoh**: 1,4,9,16,25,…
**-Rumus suku ke-n:** $U_n = n^2$

**4.Deret Bilangan Kubik:** Deret dengan pola nilai berupa kubik bilangan bulat.
**-Contoh**: 1,8,27,64,125,…
**-Rumus suku ke-n:** : $U_n = n^3$

**5.Deret Fibonacci**: Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
**-Contoh**: 0,1,1,2,3,5,8,…
**-Rumus suku ke-n**(Rekursif): $F_n = F_{n-1} + F_{n-2}, \quad F_0 = 0, \quad F_1 = 1$

**String adalah deretan berhingga karakter berbentuk:**$a_1 a_2 a_3 a_4 \dots a_n$. Panjang string S adalah jumlah karakter di dalam string tersebut.
**Contoh:**: *informatika* adalah string dengan panjang 11 karakter 10100101 adalah string biner dengan panjang 8 bit.
* String kosong dilambangkan dengan $\lambda$, panjangnya = 0

# PENJUMLAHAN DERETAN
**Jumlah deretan**: $a_m, a_{m+1}, a_{m+2}, \dots, a_n$
adalah: $a_m + a_{m+1} + a_{m+2} + \dots + a_n$
* Notasi sumasi :$\sum_{k=m}^{n} a_k$
Dimana:
-k adalah indeks summasi, 
-m adalah batas bawah indeks,
-n adalah batas atas indeks.
**Contoh 2**:
Berapa Nilai:$\sum_{k=1}^{5} k^2$
**Jawaban**:$\sum_{k=1}^{5} k^2 = 1^2 + 2^2 + 3^2 + 4^2 + 5^2 = 1 + 4 + 9 + 16 + 25 = 55$
**Contoh 3**:
Batas bawah sumasi kadangkala perlu digeser agar dapat dijumlahkan dengan sumasi lain yang memiliki batas bawah berbeda. Pada contoh 2 di atas batas bawah digeser dari 1 menjadi 0, akibatnya:
$\sum_{k=1}^{5} k^2 = \sum_{k=0}^{4} (k+1)^2$
**Contoh 4:**
Sumasi dapat dipecah dengan membagi dua indeksnya, misalnya:$\sum_{k=1}^{100} k^2 = \sum_{k=1}^{49} k^2 + \sum_{k=50}^{100} k^2$

## Tugas
PEMBUKTIAN Dari 3 rumus dibawah.Beberapa sumasi sudah ditemukan rumus penjumlahannya sebagai berikut<br>
![Pictur1](https://hackmd.io/_uploads/B1DW02TfJe.png) (deret geometri) dan (deret aritmatika)

**Contoh 5:**
Hitung nilai:$\sum_{k=50}^{100} k^2$
**Jawaban:**
-$\sum_{k=1}^{100} k^2 = \sum_{k=1}^{49} k^2 + \sum_{k=50}^{100} k^2$
-$\sum_{k=50}^{100} k^2 = \sum_{k=1}^{100} k^2 - \sum_{k=1}^{49} k^2$
**Gunakan Rumus:**![p](https://hackmd.io/_uploads/rkqdDmRM1x.png)![n](https://hackmd.io/_uploads/B15Fv70Mye.png)
$\sum_{k=50}^{100} k^2 = \frac{(100)(101)(201)}{6} - \frac{(49)(50)(99)}{6} = 338,350 - 40,425 = 297,925$

# Sumasi Ganda:
* Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.
Contoh:$\sum_{i=1}^4 \sum_{j=1}^3 ij$ 
Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu  dilanjukan dengan sumasi terluar
$\sum_{i=1}^4 \sum_{j=1}^3 ij = \sum_{i=1}^4 (i + 2i + 3i) = \sum_{i=1}^4 6i = 6 + 12 + 18 + 24 = 60$
**Contoh penggunaan:** Berapa kali operasi + dilakukan di dalam algoritma di bawah ini? 
![Cuplikan layar 2024-11-22 225458](https://hackmd.io/_uploads/r13FYm0M1e.png)
**Penyelesaian:** Operasi + terdapat di dalam pernyataan x = x + 2 Operasi ini dilakukan satu kali pada setiap pengulangan Jumlah seluruh operasi + adalah:
![Cuplikan layar 2024-11-22 230120](https://hackmd.io/_uploads/HJ0NsXCGyg.png)

# REKURSI
* Sebuah objek dikatakan rekursif  (recursive) jika ia didefinisikan dalam terminologi dirinya sendiri.
* Proses mendefinisikan objek dalam terminologi dirinya sendiri disebut rekursi (recursion).
* Perhatikan tiga buah gambar pada tiga slide berikut ini.
* Objek fraktal  adalah contoh bentuk rekursif.
![p](https://hackmd.io/_uploads/r1MajQAfyg.gif)![n](https://hackmd.io/_uploads/rkyAjmCGyx.jpg)
**FUNGSI REKURSIF**
* Fungsi rekursif didefinisikan oleh dua bagian:
1.Basis 
-Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit
-Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).
2.Rekurens
-Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri. 
-Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil. 
**Contoh 6:** Misalkan f didefinsikan secara rekusif sbb
![Cuplikan layar 2024-11-22 231003](https://hackmd.io/_uploads/rkbbpmRzJg.png)
**Jawab:**
![Cuplikan layar 2024-11-22 231058](https://hackmd.io/_uploads/HyvHaXAf1g.png)
**Cara lain menghitungnya:**
f(0) = 3
		f(1) = 2f(0) + 4 = 2.3 + 4 = 10
		f(2) = 2f(1) + 4 = 2.10 + 4 = 24
		f(3) = 2f(2) + 4 = 2.24 + 4 = 52
		f(4) = 2f(3) + 4 = 2.52 + 4 = 108
		jadi,f(4)=108
**Contoh 7:** Nyatakan n! dalam definisi rekursif
Solusi: ![k](https://hackmd.io/_uploads/HkTMCQRMke.png)
Misalkan f(n) = n!, maka
![9](https://hackmd.io/_uploads/B10SCQCfyx.png)
Menghitung 5! secara rekursif adalah:
5! = 5 . 4! = 5 . 4 . 3! = 5 . 4 . 3 . 2! 
= 5 . 4 . 3 . 2 . 1! = 5 . 4 . 3 . 2 . 1 . 0!	=  5 . 4 . 3 . 2 . 1 . 1 = 120
**Algoritma menghitung fatorial**<br>
![Cuplikan layar 2024-11-22 231919](https://hackmd.io/_uploads/BkIB1ERM1e.png)
**Contoh 8:** Barisan Fibonacci  0, 1, 1, 2, 3, 5, 8, 11, 19, …. Dapat dinyatakan secara rekursif sebagai berikut:
![Picture8](https://hackmd.io/_uploads/SJRzkBRGyl.png)
**Contoh 9:** Fungsi (polinom) Chebyshev dinyatakan sebagai
![Picture9](https://hackmd.io/_uploads/rJtKkHCzJe.png)


# Struktur Rekursif
* Simpul (node) pada pohon biner mempunyai paling banyak dua buah anak.
* Jumlah anak pada setiap simpul bisa 1, 2, atau 0.
* Simpul yang mempunyai anak disebut simpul cabang (branch node) atau simpul dalam (internal node)
* Simpul yang tidak mempunyai anak disebut simpul daun (leave).
* Pohon biner adalah struktur yang rekursif, sebab setiap simpul mempunyai cabang yang juga berupa pohon. Setiap cabang disebut  upapohon (subtree).
![l](https://hackmd.io/_uploads/rkjlgS0zJl.jpg)
* Oleh karena itu, pohon dapat didefinisikan secara rekursif sebagari berikut:
(i) Basis: kosong adalah pohon biner
(ii) Rekurens: Jika T1 dan T2 adalah pohon biner, maka      adalah pohon biner
**Proses pembentukan pohon biner secara rekursif:**
1.$\phi$
2.![m](https://hackmd.io/_uploads/SJ2cxHCfkg.gif)

								









































