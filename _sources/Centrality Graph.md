---
title: Centrality Graph

---

# Centrality Graph
---
Dengan menggunakan teori graf. Implementasi Social Network Analysis dapat menjelaskan relasi atau hubungan antar aktor melalui visualisasi berbentuk graf

![image](https://hackmd.io/_uploads/rJGXBWdM1x.png)

terdapat node yang mewakili orang atau individu atau aktor. Relasi antar objek dapat dinyatakan dengan link, Social network terdiri dari banyak aktor yang mempunyai relasisatu sama lain hingga membentuk peta jaringan sosial yang dinyatakan dengan graph

![image](https://hackmd.io/_uploads/rJ7z8-dfye.png)

Tidak semua node dalam jaringan adalah penting  (aktor)
Mencari node yang paling penting dalam suatu jaringan
Centrality adalah penentuan aktor menggunakan ukuran pada Social Network 

Centrality dalam teori graf dan social network. Dibagi menjadi empat jenis, 
* degree centrality, 
* betweeness centrality, 
* closeness centrality 
* eigenvector centrality


---
 ## Degree centrality
Degree centrality adalah jumlah link yang terkoneksi pada suatu node yang mewakili interaksi.
Pentingnya node ditentukan oleh jumlah node yang berdekatan dengan node tersebut
Lebih besar derajatnya (degree), maka lebih penting node itu dalam suatu jaringan 
Hanya sebagian kecil node yang memiliki derajat tinggi dalam jaringan 

$$
C_D(v) = \frac{\text{deg}(v)}{n - 1}
$$

Di mana:

deg(v) : jumlah koneksi langsung dari node v
n : total jumlah node dalam jaringan.

![image](https://hackmd.io/_uploads/HkwqDWdfyg.png)

Untuk  node 1, degree centrality adalah 3


---
## Closenes centrality
Closenes centrality adalah nilai kedekatan antara satu node dengan node lain dalam jaringan dengan menghitung rata-rata dari jarak relasi node-node tersebut. Skor closeness centrality mewakili kecepatan dalam penyebaran informasi.

![image](https://hackmd.io/_uploads/B11oFbuzkl.png)

![image](https://hackmd.io/_uploads/BJYntbdzJg.png)

node 1 ke node 1 jaraknya 0, node 1 ke node 2,3,4 jaraknya 1, node 1 ke 5,6 jaraknya 2 node, node 1 ke node 7,8 jaraknya 3 node, node 1 ke node 9 jaraknya 4 node

![image](https://hackmd.io/_uploads/H1nTnW_GJl.png)



---
## Betweeness Centrality
Skor betweeness Centrality mewakili seberapa besar informasi yang tersebar dari suatu aktor. Semakin besar skor, artinya aktor tersebut semakin berperan dalam penyebaran informasi 

Semakin banyak lintasan yang harus melewati persimpangan itu (misal tidak ada jalan alternatif), maka semakin penting arti persimpangan tersebut. Hal ini menandakan seberapa besar suatu node diperlukan sebagai penghubung dalam penyebaran informasi di dalam jaringan

Ukuran ini juga dapat digunakan untuk mengidentifikasi orang atau node yang berperan sebagai penghubung (jembatan) antara dua komunitas

![image](https://hackmd.io/_uploads/SypS3b_zye.png)

![image](https://hackmd.io/_uploads/SkAqhZ_Mke.png)



