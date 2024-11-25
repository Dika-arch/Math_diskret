---
title: Deret dan rekursi

---

### Deret dan rekursi

---

Deretan adalah suatu urutan atau susunan elemen atau objek yang disusun secara teratur berdasarkan suatu aturan tertentu. Elemen dalam deretan biasanya berupa angka, huruf, simbol, atau objek lainnya, dan urutannya dapat didasarkan pada pola, nilai, atau hubungan tertentu
Definisi: Sebuah deretan adalah fungsi dari subset suatu himpunan bilangan bulat (biasanya N atau P) ke sebuah himpunan S.

```
   N = {1, 2, 3, 4, … }
   S misalnya {2, 4, 6, 8, …},   {1/3, 1/5, 1/7, …},  dsb
```
 Notasi deretan: {an}
 
 Deretan umumnya dinyatakan dalam suatu formula, misalnya:
 	an = 2n
	an = 1/n
 	an = 7 – 3n


 Dalam konteks matematika, deretan sering merujuk pada barisan bilangan, yaitu kumpulan bilangan yang disusun dalam suatu pola tertentu.
  Misalnya:
 Deretan bilangan ganjil: 1,3,5,7,…
 Deretan bilangan genap: 2,4,6,8,…
 Deretan bilangan yang membentuk deret aritmetika: 3,6,9,12.... 
## CONTOH DERETAN ARITMETIKA
# DERET ARITMETIKA
 Deret dengan pola kenaikan atau penurunan tetap.
Contoh: 2,5,8,11,14,…
Rumus suku ke-n:
𝑈_𝑛=𝑎+(𝑛−1)⋅𝑏
Di mana:
𝑎: suku pertama 
𝑏: beda (selisih antar suku
𝑛: nomor suku yang dicari
# DERET GEOMETRI
Deret dengan pola kelipatan tetap.
Contoh: 3,6,12,24,48,…
 Rumus suku ke-n:𝑈_𝑛=𝑎⋅𝑟^((𝑛−1) )
 Di mana:
 𝑎: suku pertama 
𝑟: rasio (perbandingan antar suku,
 𝑛: nomor suku yang dicari
# DERET BILANGAN KUADRAT
 Deret Bilangan Kuadrat
Deret dengan pola nilai berupa kuadrat bilangan bulat.
Contoh: 1,4,9,16,25,…
Rumus suku ke-n:𝑈_𝑛=𝑛^2
# Deret Bilangan Kubik
Deret dengan pola nilai berupa kubik bilangan bulat.## - Contoh: 1,8,27,64,125,…
Rumus suku ke-n:𝑈_𝑛=𝑛^3
# DERET FIBONACCI
Deret dengan pola di mana setiap suku merupakan jumlah dua suku sebelumnya.
Contoh: 0,1,1,2,3,5,8,…
## - Rumus suku ke-n (rekursif):𝐹_𝑛=𝐹_(𝑛−1)+𝐹_(𝑛−2),𝐹_0=0,𝐹_1=1
String adalah deretan berhingga karakter berbentuk
		a1a2a3a4…an

##    Panjang string S adalah jumlah karakter di dalam string tersebut
##      
Contoh:  informatika adalah string dengan panjang 11 karakter
         10100101 adalah string biner dengan panjang 8 bit
 
String kosong dilambangkan dengan , panjangnya = 0

# PENJUMLAHAN DERETAN
Jumlah deretan ### 	am, am+1, am+2, …, an
  adalah
	 am + am+1 + am+2 + … + an
  atau dalam notasi sumasi:
 	∑_(𝑘=𝑚)^𝑛▒𝑎_𝑘   
    
    k adalah indeks summasi, 
    m adalah batas bawah indeks,
     n adalah batas atas indeks

Contoh 2: Berapa nilai ∑_(𝑘=1)^5▒𝑘^2 ?
 Jawaban: 
	∑_(𝑘=1)^5▒𝑘^2 = 12 + 22 + 32 + 42 + 52 = 1 + 4 + 9 + 16 + 25 = 55

 Contoh 3: Batas bawah sumasi kadangkala perlu digeser agar dapat dijumlahkan dengan sumasi lain yang memiliki batas bawah berbeda. Pada contoh 2 di atas batas bawah digeser dari 1 menjadi 0, akibatnya:
	 ∑_(𝑘=1)^5▒𝑘^2 = ∑_(𝑘=0)^4▒〖(𝑘+1)〗^2  
 
 Contoh 4: Sumasi dapat dipecah dengan membagi dua indeksnya, misalnya
 	  ∑_(𝑘=1)^100▒𝑘^2 =  ∑_(𝑘=1)^49▒𝑘^2  +  ∑_(𝑘=50)^100▒𝑘^2 
 Contoh 5: Hitung nilai    ∑_(𝑘=50)^100▒𝑘^2   
## Jawaban:
## 	   ∑_(𝑘=1)^100▒𝑘^2 =  ∑_(𝑘=1)^49▒𝑘^2  +  ∑_(𝑘=50)^100▒𝑘^2   
## 
## 	    ∑_(𝑘=50)^100▒𝑘^2  = ∑_(𝑘=1)^100▒𝑘^2 −  ∑_(𝑘=1)^49▒𝑘^2   
## 
##  Gunakan rumus                                                  :

## 	      ∑_(𝑘=50)^100▒𝑘^2  =((100)(101)(201))/6 − ((49)(50)(99))/6  = 338.350 – 40.425 = 297.925
# SUMASI GANDA
 Di dalam algoritma, kita perlu menghitung berapa kali suatu operasi tertentu dilakukan di dalam sebuah kalang bersarang (nested loop). Penjumlahan semua operasi di dalam kalang bersarang dinyatakan dalam bentuk sumasi ganda.
 
##     Contoh: ∑_(𝑖=1)^4▒∑_(𝑗=1)^3▒𝑖𝑗 

##     Untuk menghitung sumasi ganda, mula-mula ekspansi sumasi terdalam, lalu  dilanjukan dengan sumasi terluar:
## 	 	∑_(𝑖=1)^4▒∑_(𝑗=1)^3▒𝑖𝑗 = ∑_(𝑖=1)^4▒〖(𝑖+2𝑖+3𝑖)= ∑_(𝑖=1)^4▒6𝑖〗 = 6 + 12 + 18 + 24 = 60


![image](https://hackmd.io/_uploads/rkkCQ6l7ye.png)
![image](https://hackmd.io/_uploads/rkNZr6lQJl.png)

# FUNGSI REKURSIF
## Fungsi rekursif didefinisikan oleh dua bagian:
 (i)  Basis 
 Bagian yang berisi nilai fungsi yang terdefinisi secara eksplisit. 
 Bagian ini juga sekaligus menghentikan rekursif (dan memberikan sebuah nilai yang terdefinisi pada fungsi rekursif).
 
  (ii)  Rekurens
Bagian ini mendefinisikan fungsi dalam terminologi dirinya sendiri. 
 Berisi kaidah untuk menemukan nilai fungsi pada suatu input dari nilai-nilai lainnya pada input yang lebih kecil. 
![image](https://hackmd.io/_uploads/HyGErTl7Jx.png)
![image](https://hackmd.io/_uploads/SyaNHagmJg.png)

![image](https://hackmd.io/_uploads/rk7jH6xmkx.png)

## Algoritma menghitung faktorial:
## 
## function Faktorial (input  n :integer)integer
## { mengembalikan nilai n!;
##   basis   : jika n = 0, maka 0! = 1
##   rekurens: jika n > 0, maka n! = n  (n-1)!
## }
## DEKLARASI
##       -
## ALGORITMA:
##     if n = 0 then
##        return 1		              { basis }
##     else
##        return  n * Faktorial(n – 1)	{ rekurens }
##     end


![image](https://hackmd.io/_uploads/ByDXL6xXkx.png)
![image](https://hackmd.io/_uploads/BJF4ITxXJg.png)

## Latihan
## 	1. Definisikan an secara rekursif , yang dalam hal ini a adalah bilangan riil tidak-nol dan n adalah bilangan bulat tidak-negatif.
## 
## 	2. Nyatakan a  b secara rekursif, yang dalam hal ini a dan b adalah bilangan bulat positif.
## 
## (Solusinya ada setelah slide berikut!)
# ![image](https://hackmd.io/_uploads/S1kP9agmyg.png)
# STRUKTUR REKURSIF
 Struktur data yang penting dalam komputer adalah pohon biner (binary tree). 

![image](https://hackmd.io/_uploads/rJ9cqpxmye.png)
 Simpul (node) pada pohon biner mempunyai paling banyak dua buah anak.

 Jumlah anak pada setiap simpul bisa 1, 2, atau 0.

 Simpul yang mempunyai anak disebut simpul cabang (branch node) atau simpul dalam (internal node)

 Simpul yang tidak mempunyai anak disebut simpul daun (leave).
 
## Pohon biner adalah struktur yang rekursif, sebab setiap simpul mempunyai cabang yang juga berupa pohon. Setiap cabang disebut  upapohon (subtree).


![image](https://hackmd.io/_uploads/HyZT9TeX1e.png)

Oleh karena itu, pohon dapat didefinisikan secara rekursif sebagari berikut:

## 	(i) Basis: kosong adalah pohon biner
## 	(ii) Rekurens: Jika T1 dan T2 adalah pohon biner, maka                        
##           adalah pohon biner
## 								                    T1       T2 
## 
![image](https://hackmd.io/_uploads/HJrGiTgmyl.png)

