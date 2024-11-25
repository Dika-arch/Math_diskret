---
title: Deretan Dan Rekursi

---

# Deretan Dan Rekursi
## Deretan (sequence) 
* Deretan adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu

* Definisi: Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.

   **N** = {1, 2, 3, 4, … }
   S misalnya {2, 4, 6, 8, …},   {1/3, 1/5, 1/7, …},  dsb

* $$Notasi.deretan: \{a_n\}$$

* Deretan umumnya dinyatakan dalam suatu formula, misalnya:
	$$a_n = 2n$$
	$$a_n = 1/n$$
	$$a_n = 7 – 3n$$

Dalam konteks matematika, deretan sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu.
 Misalnya:
1. Deretan bilangan ganjil: 1,3,5,7,…
2. Deretan bilangan genap: 2,4,6,8,…
3. Deretan bilangan yang membentuk deret aritmetika: 3,6,9,12....

* **Contoh-contoh deretan dan formulanya:**

* **Deret Aritmetika**
 Deret dengan pola kenaikan atau penurunan tetap. 
. **Contoh**: 2,5,8,11,14,… 
. **Rumus suku ke-n**: $$𝑈_𝑛=𝑎+(𝑛−1)⋅𝑏$$

Di mana: 
. 𝑎 : suku pertama 
. 𝑏 : b eda (selisih antar suku 
. 𝑛 : nomor suku yang dicari

* **Deret Geometri**
Deret dengan pola kelipatan tetap.
. **Contoh**: 3,6,12,24,48,…
. **Rumus suku ke-n**:$$𝑈_𝑛=𝑎⋅𝑟 ^{(𝑛-1)}$$

Di mana:
. 𝑎 : suku pertama 
. 𝑟 : rasio (perbandingan antar suku),
. 𝑛 : nomor suku yang dicari

* **Deret Bilangan Kuadrat**
Deret dengan pola nilai berupa kuadrat bilangan bulat.
. **Contoh** : 1,4,9,16,25,…
. **Rumus suku ke-n**: $$ 𝑈_𝑛=𝑛^2 $$

* **Deret Bilangan Kubik**
Deret dengan pola nilai berupa kubik bilangan bulat 
. **Contoh**: 1,8,27,64,125,…
. **Rumus suku ke-n**: $$𝑈_𝑛=𝑛^3$$

* **Deret Fibonacci**
Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
. **Contoh**: 0,1,1,2,3,5,8,…
. **Rumus suku ke-n** (rekursif): $$𝐹_𝑛=𝐹_{𝑛−1}+𝐹_{𝑛−2},𝐹_0=0,𝐹_1=1$$


String adalah deretan berhingga karakter berbentuk
$$ a_1a_2a_3a_4...a_n $$

Panjang string S adalah jumlah karakter di dalam string tersebut.
     
Contoh:  informatika adalah string dengan panjang 11 karakter
10100101 adalah string biner dengan panjang 8 bit

$$ String. kosong. dilambangkan. dengan. \lambda,panjangnya = 0 $$

## Penjumlahan deretan 

Jumlah deretan  
aₘ, aₘ₊₁, aₘ₊₂, ..., aₙ  

adalah  
aₘ + aₘ₊₁ + aₘ₊₂ + ... + aₙ  

atau dalam notasi summasi:  
Σₖ₌ₘ aₖ  

k adalah indeks summasi,  
m adalah batas bawah indeks,  
n adalah batas atas indeks

Contoh 2:  
Berapa nilai $$∑_{𝑘=1}^{5}𝑘^2$$

Jawaban:  
$$
\Sigma_{k=1}^{5} k^2 = 1^2 + 2^2 + 3^2 + 4^2 + 5^2 = 1 + 4 + 9 + 16 + 25 = 55
$$

Contoh 3:  
Batas bawah sumasi kadangkala perlu digeser agar dapat dijumlahkan dengan sumasi lain yang memiliki batas bawah berbeda. Pada contoh 2 di atas batas bawah digeser dari 1 menjadi 0, akibatnya:  
$$
\Sigma_{k=1}^{5} k^2 = \Sigma_{k=0}^{4} (k + 1)^2
$$

Contoh 4:  
Sumasi dapat dipecah dengan membagi dua indeksnya, misalnya:  
$$
\Sigma_{k=1}^{100} k^2 = \Sigma_{k=1}^{49} k^2 + \Sigma_{k=50}^{100} k^2
$$

* Beberapa sumasi sudah ditemukan rumus penjumlahannya sebagai berikut:

.........

Contoh 5: Hitung Nilai $$∑_{(k=50)}^{100} k²$$

*Jawaban*:

$$
\Sigma_{k=50}^{100} k^2 = \Sigma_{k=1}^{49} k^2 + \Sigma_{k=1}^{100} k^2
$$

$$
\Sigma_{k=50}^{100} k^2 = \Sigma_{k=1}^{100} k^2 - \Sigma_{k=1}^{49} k^2
$$

Gunakan rumus:

$$
\Sigma_{k=1}^{n} k^2 = \frac{n(n+1)(2n+1)}{6}
$$

Perhitungan:

$$
\Sigma_{k=50}^{100} k^2 = \frac{100(101)(201)}{6} - \frac{49(50)(99)}{6}
= 338.350 - 40.425 = \mathbf{297.925}
$$

## Sumasi ganda

* Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.

Contoh: $$∑_{𝑖=1}^{4}∑_{𝑗=1}^{3}𝑖𝑗 $$

Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu  dilanjukan dengan sumasi terluar:
$$∑_{(𝑖=1)}^{4}∑_{𝑗=1}^{3}𝑖𝑗 = ∑_{𝑖=1}^{4}(𝑖+2𝑖+3𝑖)= ∑_{𝑖=1}^4 6𝑖 = 6 + 12 + 18 + 24 = 60$$

Contoh penggunaan: Berapa kali operasi + dilakukan di dalam algoritma di bawah ini? 

    x = 0
    for j = 1 to 10 do  
        for k = 1 to j do  
            x = x + 2  
        end for  
    end for



Penyelesaian:
Operasi + terdapat di dalam pernyataan x = x + 2
Operasi ini dilakukan satu kali pada setiap pengulangan
Jumlah seluruh operasi + adalah:

$$t = ∑_{(𝑗=1)}^{10}∑_{(𝑘=1)}^{𝑗}1 $$
  
$$  = ∑_{(𝑗=1)}^{10}(1+1+ …+1 .𝑠𝑒𝑏𝑎𝑛𝑦𝑎𝑘. 𝑗 .𝑘𝑎𝑙𝑖)〗$$

$$  = ∑_{(𝑗=1)}^{10}𝑗 $$

$$  = \frac{10(10+1)}{2}  = 55$$

## Rekursi
* Sebuah objek dikatakan rekursif  (recursive) jika ia didefinisikan dalam terminologi dirinya sendiri. 

* Proses mendefinisikan objek dalam terminologi dirinya sendiri disebut rekursi (recursion).

* Objek fraktal  adalah contoh bentuk rekursif.

### Fungsi Rekursif
* Fungsi rekursif didefinisikan oleh dua bagian:
 (i)  Basis 
* Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit. 
* Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).
 
 (ii)  Rekurens
* Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri. 
* Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil. 

Contoh 6
Misalkan $f$ didefinisikan secara rekursif sebagai:

$$
f(n) = \begin{cases}
3, & \text{, } n = 0 \\ b
2f(n-1) + 4, & \text{, } n > 0
\end{cases}
$$

Tentukan nilai $f(4)$!

Solusi:      f(4) = 2f(3) + 4 
			=  2(2f(2) + 4) + 4
			=  2(2(2f(1) + 4) + 4) + 4
			=  2(2(2(2f(0) + 4) + 4) + 4) + 4
			=  2(2(2(2.3 + 4) + 4) + 4) + 4	
			=  2(2(2(10) + 4) + 4) + 4
			=  2(2(24) + 4) + 4
			=  2(52) + 4
			=  108	
            
Cara lain menghitungnya:
		f(0) = 3
		f(1) = 2f(0) + 4 = 2 . 3 + 4 = 10
		f(2) = 2f(1) + 4 = 2 . 10 + 4 = 24
		f(3) = 2f(2) + 4 = 2 . 24 + 4 = 52
		f(4) = 2f(3) + 4 = 2 . 52 + 4 = 108
		
Jadi, f(4) = 108.

Contoh 7: Nyatakan n! dalam definisi rekursif

Solusi:

$$
n! =  \underbrace{ 1 \times 2 \times 3 \times \dots \times (n-1)}_{(n-1)!} \times n 
={(n-1)!} \times n
$$

Misalkan f(n) = n!, maka  

$$
n! = 
\begin{cases} 
1 & \text{, } n = 0 \\
n. (n-1)! & \text{, } n > 0
\end{cases}
$$


Menghitung 5! secara rekursif adalah:
		         5! = 5 . 4! = 5 . 4 . 3! = 5 . 4 . 3 . 2! 
			= 5 . 4 . 3 . 2 . 1! = 5 . 4 . 3 . 2 . 1 . 0!	=  5 . 4 . 3 . 2 . 1 . 1 = 120
            
Algoritma menghitung faktorial:

function Faktorial (input  n :integer) **integer**
{ mengembalikan nilai n!;
  basis   : jika n = 0, maka 0! = 1
  rekurens: jika n > 0, maka n! = n x (n-1)!
}
DEKLARASI ALGORITMA:


    if n = 0 then
       return 1		              { basis }
    else
       return  n * Faktorial(n – 1)	{ rekurens }
    end




Contoh 8: Barisan Fibonacci  0, 1, 1, 2, 3, 5, 8, 11, 19, …. Dapat dinyatakan secara rekursif sebagai berikut:

$$
f_n = 
\begin{cases} 
0, & \text{ } n = 0 \\
1, & \text{ } n = 1 \\
f_{n-1} + f_{n-2}, & \text{ } n > 1
\end{cases}
$$



Contoh 9: Fungsi (polinom) Chebyshev dinyatakan sebagai

$$
T(n, x) = 
\begin{cases} 
1, & \text{ } n = 0 \\
x, & \text{ } n = 1 \\
2x \cdot T(n-1, x) - T(n-2, x), & \text{ } n > 1
\end{cases}
$$


Contoh 10: Sumasi    $$∑_{(𝑘=0)}^{𝑛}𝑎_𝑘 $$             didefinisikan secara rekursif sebagai  berikut:

$$∑_{𝑘=0}^𝑛 𝑎_𝑘 =𝑎_0+𝑎_1+𝑎_2+...+𝑎_{𝑛−1}+𝑎_𝑛 $$   
$$= (𝑎_0+𝑎_1+𝑎_2+...+𝑎_(𝑛−1))+𝑎_𝑛 $$         
$$= (∑_{𝑘=0}^{𝑛−1}𝑎_𝑘 )+𝑎_𝑛 $$

sehingga 
$$
\sum_{k=0}^{n} a_k = 
\begin{cases}
a_0   & \text{, } n = 0 \\
\left( \sum_{k=0}^{n-1} a_k \right) + a_n & \text{, } n > 0
\end{cases}
$$


## Struktur Rekursif

Struktur data yang penting dalam komputer adalah pohon biner (binary tree). 

.......

* Simpul (node) pada pohon biner mempunyai paling banyak dua buah anak.

* Jumlah anak pada setiap simpul bisa 1, 2, atau 0.

* Simpul yang mempunyai anak disebut simpul cabang (branch node) atau simpul dalam (internal node)

* Simpul yang tidak mempunyai anak disebut simpul daun (leave).


* Pohon biner adalah struktur yang rekursif, sebab setiap simpul mempunyai cabang yang juga berupa pohon. Setiap cabang disebut  upapohon (subtree).

.....

Oleh karena itu, pohon dapat didefinisikan secara rekursif sebagari berikut:

(i) Basis: kosong adalah pohon biner
(ii) Rekurens: Jika T1 dan T2 adalah pohon biner, maka 

....

 adalah pohon biner

Proses pembentukan pohon biner secara rekursif:

....

## Pembuktian Rumus-Rumus Summasi

## 1. Rumus Deret Geometri
$$
\sum_{k=0}^n ar^k \quad (r \neq 0) = \frac{ar^{n+1} - a}{r - 1}, \quad r \neq 1
$$

*Bukti:*
1. Mulai dari definisi deret geometri:
   $$
   S = a + ar + ar^2 + \dots + ar^n
   $$

2. Kalikan kedua sisi dengan \(r\):
   $$
   rS = ar + ar^2 + \dots + ar^{n+1}
   $$

3. Kurangkan \(S - rS\):
   $$
   S - rS = a - ar^{n+1}
   $$

4. Faktorkan \(S(1 - r)\):
   $$
   S(1 - r) = a(1 - r^{n+1})
   $$

5. Bagi dengan \(1 - r\) (dengan syarat \(r \neq 1\)):
   $$
   S = \frac{a(r^{n+1} - 1)}{r - 1} = \frac{ar^{n+1} - a}{r - 1}
   $$

---

## 2. Rumus Penjumlahan Bilangan Bulat
$$
\sum_{k=1}^n k = \frac{n(n+1)}{2}
$$

*Bukti dengan Induksi Matematika:*
1. *Basis:* Untuk \(n = 1\):
   $$
   \sum_{k=1}^1 k = 1 = \frac{1(1+1)}{2}
   $$
   Benar.

2. *Hipotesis Induksi:* Misalkan benar untuk \(n = m\):
   $$
   \sum_{k=1}^m k = \frac{m(m+1)}{2}
   $$

3. *Langkah Induksi:* Tunjukkan benar untuk \(n = m+1\):
   $$
   \sum_{k=1}^{m+1} k = \sum_{k=1}^m k + (m+1)
   $$
   Substitusi hipotesis induksi:
   $$
   \sum_{k=1}^{m+1} k = \frac{m(m+1)}{2} + (m+1)
   $$
   Faktorkan \(m+1\):
   $$
   \sum_{k=1}^{m+1} k = \frac{m(m+1) + 2(m+1)}{2} = \frac{(m+1)(m+2)}{2}
   $$
 

---

## 3. Rumus Penjumlahan Kuadrat Bilangan Bulat
$$
\sum_{k=1}^n k^2 = \frac{n(n+1)(2n+1)}{6}
$$

*Bukti dengan Induksi Matematika:*
1. *Basis:* Untuk \(n = 1\):
   $$
   \sum_{k=1}^1 k^2 = 1^2 = 1 = \frac{1(1+1)(2\cdot1+1)}{6}
   $$
   Benar.

2. *Hipotesis Induksi:* Misalkan benar untuk \(n = m\):
   $$
   \sum_{k=1}^m k^2 = \frac{m(m+1)(2m+1)}{6}
   $$

3. *Langkah Induksi:* Tunjukkan benar untuk \(n = m+1\):
   $$
   \sum_{k=1}^{m+1} k^2 = \sum_{k=1}^m k^2 + (m+1)^2
   $$
   Substitusi hipotesis induksi:
   $$
   \sum_{k=1}^{m+1} k^2 = \frac{m(m+1)(2m+1)}{6} + (m+1)^2
   $$
   Faktorkan \((m+1)\):
   $$
   \sum_{k=1}^{m+1} k^2 = \frac{m(m+1)(2m+1) + 6(m+1)^2}{6}
   $$
   $$
   = \frac{(m+1)m(2m+1) + 6(m+1)]}{6}
   $$
   $$
   = \frac{(m+1)(2m^2 + 7m + 6)}{6}
   $$
   $$
   Faktorkan (2m^2 + 7m + 6):
   $$
   $$
   = \frac{(m+1)(m+2)(2m+1)}{6}
   $$
   

---

## Latihan

---

## 1. Tentukan nilai:
$$
\sum_{k=1}^8 2^k + \sum_{k=2}^8 (-3)^k
$$

*Penyelesaian:*
- Untuk $$\sum_{k=1}^8 2^k$$, gunakan rumus deret geometri:
  $$
  S = \sum_{k=1}^8 2^k = \frac{2(2^8 - 1)}{2 - 1} = 2^9 - 2 = 512 - 2 = 510
  $$

- Untuk $$\sum_{k=2}^8 (-3)^k $$, gunakan rumus deret geometri (dengan suku pertama $$(-3)^2 = 9)$$:
  $$
  S = \sum_{k=2}^8 (-3)^k = \frac{9((-3)^7 - 1)}{-3 - 1} = \frac{9(-2187 - 1)}{-4} = \frac{9(-2188)}{-4} = 4923
  $$

- Jadi, total:
  $$
  \sum_{k=1}^8 2^k + \sum_{k=2}^8 (-3)^k = 510 + 4923 = 5433
  $$

*Jawaban: 5433*

---

## 2. Tentukan nilai:
$$
\sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j)
$$

*Penyelesaian:*
1. Pisahkan penjumlahan:
   $$
   S = \sum_{i=0}^2 \sum_{j=0}^3 (2i + 3j)
   = \sum_{i=0}^2 \left( \sum_{j=0}^3 2i + \sum_{j=0}^3 3j \right)
   $$

2. Untuk $$\sum_{j=0}^3 2i:$$
   $$
   \sum_{j=0}^3 2i = 4i \quad \text{(karena ada 4 suku, semua dengan nilai \(2i\))}
   $$

3. Untuk $$\sum_{j=0}^3 3j$$:
   $$
   \sum_{j=0}^3 3j = 3(0 + 1 + 2 + 3) = 3 \cdot 6 = 18
   $$

4. Gabungkan:
   $$
   S = \sum_{i=0}^2 (4i + 18) = \sum_{i=0}^2 4i + \sum_{i=0}^2 18
   $$

5. Hitung:
   - $$\sum_{i=0}^2 4i = 4(0 + 1 + 2) = 4 \cdot 3 = 12$$
   - $$\sum_{i=0}^2 18 = 18 \cdot 3 = 54$$

6. Total:
   $$
   S = 12 + 54 = 66
   $$

*Jawaban: 66*

---

## 3. Tentukan nilai:
$$
\sum_{i=0}^3 \sum_{j=0}^2 i
$$

*Penyelesaian:*
1. Pisahkan penjumlahan:
   $$
   S = \sum_{i=0}^3 \sum_{j=0}^2 i
   $$

2. Karena \(i\) adalah konstanta untuk setiap \(j\), maka:
   $$
   \sum_{j=0}^2 i = 3i \quad \text{(ada 3 suku, semua bernilai \(i\))}.
   $$

3. Maka:
   $$
   S = \sum_{i=0}^3 3i = 3 \sum_{i=0}^3 i
   $$

4. Hitung $$(\sum_{i=0}^3 i:$$
   $$
   \sum_{i=0}^3 i = 0 + 1 + 2 + 3 = 6
   $$

5. Total:
   $$
   S = 3 \cdot 6 = 18
   $$

*Jawaban: 18*








