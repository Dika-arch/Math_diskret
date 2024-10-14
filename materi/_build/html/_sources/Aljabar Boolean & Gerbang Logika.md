---
title: '#Aljabar Boolean & Gerbang Logika'

---

# Aljabar Boolean & Gerbang Logika

## Operator Biner:
Aljabar Boolean memiliki dua operator biner:
Penjumlahan (+): Digunakan untuk operasi disjungsi (OR).
Perkalian (⋅): Digunakan untuk operasi konjungsi (AND).

## Operator Uner:
Komplemen: Digunakan untuk menghasilkan nilai yang berlawanan dari suatu elemen. Misalnya, jika a = 1, maka komplemen a = 0, dan sebaliknya.

### Aljabar Boolean 
sering digunakan dalam pemrograman untuk mengevaluasi ekspresi logika. sistem matematika untuk manipulasi variabel yang dapat memiliki salah satu dari dua nilai.  
Ekspresi Boolean dibuat dengan melakukan operasi pada variabel Boolean.  
Operator Boolean yang umum termasuk AND (AND), (OR), dan (NOT).

Aljabar Boolean adalah sistem matematika untuk manipulasi variabel yang dapat memiliki salah satu dari dua nilai.  
Dalam logika formal, nilai-nilai ini adalah "benar" dan "salah."  
Dalam sistem digital, nilai-nilai ini adalah "nyala" dan "mati," 1 dan 0, atau "tinggi" dan "rendah."  
Ekspresi Boolean dibuat dengan melakukan operasi pada variabel Boolean. 

* Sebuah operator Boolean dapat dijelaskan sepenuhnya menggunakan tabel kebenaran.  
* Tabel kebenaran untuk operator Boolean D (AND) dan (OR) ditunjukkan di sebelah kanan.  
* Operator AND  juga dikenal sebagai produk Boolean. Operator OR adalah jumlah Boolean
![image](https://hackmd.io/_uploads/By11g3wJke.png)

 

---


### Boolean Algebra
Tabel kebenaran untuk operator Boolean (NOT) ditunjukkan di sebelah kanan. Operasi NOT paling sering dilambangkan dengan garis atas. 
**Sebuah fungsi Boolean memiliki:**  
* Setidaknya satu variabel Boolean,  
* Setidaknya satu operator Boolean, dan  
* Setidaknya satu input dari himpunan {0,1}.  
Fungsi ini menghasilkan output yang juga merupakan anggota dari himpunan {0,1}.

![image](https://hackmd.io/_uploads/SyM2ynD1yl.png)



Tabel kebenaran untuk fungsi Boolean. : 
![image](https://hackmd.io/_uploads/HkdPk2D1yg.png)

Untuk mempermudah evaluasi fungsi Boolean, tabel kebenaran berisi kolom tambahan (diarsir) untuk menyimpan evaluasi dari bagian-bagian subfungsi

Sebagian besar identitas Boolean memiliki bentuk AND (perkallian) serta bentuk OR (jumlah). Kami menyajikan identitas kami menggunakan kedua bentuk tersebut.
![image](https://hackmd.io/_uploads/SkD3ZnPJke.png)

![image](https://hackmd.io/_uploads/BySyMnPJ1l.png)

![image](https://hackmd.io/_uploads/BkvqMnw1yg.png)

Terkadang, lebih ekonomis membangun sirkuit dengan menggunakan komplemen fungsi dan mengkomplementasi hasilnya dibandingkan mengimplementasikan fungsi secara langsung. Hukum DeMorgan memudahkan penemuan komplemen dari fungsi Boolean, yang menyatakan: 

![image](https://hackmd.io/_uploads/SJlH7hDJ1e.png)


---

### Logic Gates
* Fungsi Boolean diimplementasikan dalam sirkuit komputer digital yang disebut gerbang (gates).  
* Gerbang adalah perangkat elektronik yang menghasilkan hasil berdasarkan dua atau lebih nilai input.  
* Dalam kenyataannya, gerbang terdiri dari satu hingga enam transistor, tetapi desainer digital menganggapnya sebagai satu kesatuan.  
* Sirkuit terintegrasi mengandung kumpulan gerbang yang sesuai untuk tujuan tertentu.

**Tiga gerbang AND, OR, dan  NOT.**

![image](https://hackmd.io/_uploads/BJf8Env1kl.png)

Gerbang AND
1 AND 0=0

![image](https://hackmd.io/_uploads/H1CNHhw11g.png)

Gerbang OR
1 OR 0=1

![image](https://hackmd.io/_uploads/S1cdH3wJkg.png)

Gerbang yang sangat berguna lainnya adalah gerbang eksklusif OR (XOR). 
*Output dari operasi XOR adalah benar hanya ketika nilai-nilai input berbeda.*
![image](https://hackmd.io/_uploads/Hy2eIhvk1e.png)

Gerbang XOR
1 XOR 0=1

![image](https://hackmd.io/_uploads/Hyezv2DJke.png)

Gerbang XOR
1 XOR 1=0
![image](https://hackmd.io/_uploads/B1aEw3wy1x.png)


NAND dan NOR dua gerbang yang sangat penting. Simbol dan tabel kebenarannya ditunjukkan di sebelah kanan

![image](https://hackmd.io/_uploads/Bk79RpPkyx.png)


---

### Komponen Digital

* Hal utama yang perlu diingat adalah bahwa kombinasi gerbang menerapkan fungsi Boolean.
* Rangkaian di bawah ini mengimplementasikan fungsi Boolean 

![image](https://hackmd.io/_uploads/rJNNJ0P1ke.png)

Seperti kita lihat, jumlahnya dapat ditemukan menggunakan operasi XOR dan sisanya menggunakan operasi AND.

![image](https://hackmd.io/_uploads/rJ2kzRwkJx.png) ![image](https://hackmd.io/_uploads/HJGbM0wyyx.png)



