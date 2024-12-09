---
title: Probabilitas Bayesian

---

# Probabilitas Diskrit Probabilitas Bayesian
---
Bagaimana kemungkinan/probabilitas usia paruh baya tekanan darah sangat tinggi  kemungkinan penyakit Hipertensi (H) atau Tidak (T)

![image](https://hackmd.io/_uploads/rkWSSAq71l.png)



---

1. Prior Probability (Probabilitas Awal)
Merupakayan keyakinan awal atau distribusi probabilitas sebelum diperolehnya data tambahan. Prior ini merefleksikan pengetahuan atau keyakinan awal kita tentang parameter yang sedang dipelajari.

2. Likelihood (Peluang)
Ini merupakan distribusi probabilitas dari data yang diberikan parameter. Memberikan informasi tentang sejauh mana parameter dapat menjelaskan data yang diamati.

3. Posterior Probability (Probabilitas Posterior)
Merupakan distribusi probabilitas yang diperbarui setelah menggabungkan informasi dari prior dan likelihood. Posterior probability menggambarkan keyakinan kita tentang parameter setelah memperhitungkan data yang diamati.


---

konsep dalam probabilitas yang digunakan untuk menghitung kemungkinan kejadian dari variabel acak yang hanya memiliki nilai-nilai tertentu (terhingga atau dapat dihitung).

Dalam statistik dan teori probabilitas, teorema Bayes (juga dikenal sebagai aturan Bayes) adalah rumus matematika yang digunakan untuk menentukan probabilitas bersyarat dari suatu peristiwa. Pada dasarnya, teorema Bayes menggambarkan probabilitas suatu peristiwa berdasarkan pengetahuan sebelumnya


---

## Contoh soal

1. Diketahui:
Dokter mengetahui bahwa meningitis menyebabkan stiff neck adalah 50% -> P(S|M)
Prior probability of any patient having meningitis is 1/50.000 -> P(M)
Prior probability of any patient having stiff neck is 1/20 -> P(S)
Ditanyakan:
Apabila pasien menderita stiff neck, berapa probabilitas terkena meningitis? P(M|S)?
Jawab:
P(M|S) = P(S|M) P(M) : P(S)
P(M|S) = 0,5 x 1/50.000 : 1/20
P(M|S) = 0,0002

2. Diketahui:
Tiga anggota sebuah organisasi telah dicalonkan sebagai ketua. Peluang Ardy terpilih adalah 0,3; peluang Charles terpilih adalah 0,5; dan peluang Kinanti terpilih adalah 0,2. Seandainya Ardy terpilih, peluang terjadinya kenaikan iuran anggota adalah 0,8. Seandainya Charles dan Kinanti terpilih, peluang kenaikan iuran anggota masing-masing adalah 0,1 dan 0,4. Berapa peluang terjadi kenaikan iuran anggota?
Jawaban:
A = Kenaikan iuran anggota
B1 = Ardi yang terpilih
B2 = Charles yang terpilih
B3 = Kinanti yang terpilih
Peluang Ardy terpilih P(B1).P(A|B1) = (0,3)(0,8) = 0,24
Peluang Charles terpilih P(B2).P(A|B2) = (0,5)(0,1) = 0,05
Peluang Kinanti terpilih P(B3).P(A|B3) = (0,2)(0,4) = 0,08

3. Contoh Kasus
Misalkan, ada sebuah tes medis untuk mendeteksi penyakit tertentu. Probabilitas dasar adalah:
P( P )=0.01: Probabilitas seseorang memiliki penyakit adalah 1%.
P(T∣P)=0.9: Probabilitas tes memberikan hasil positif jika seseorang memiliki penyakit adalah 90%.
P(T∣¬P)=0.05: Probabilitas tes memberikan hasil positif jika seseorang tidak memiliki penyakit adalah 5%.
Pertanyaan: Jika seseorang mendapat hasil tes positif, berapa probabilitas orang tersebut benar-benar memiliki penyakit P(P∣T)?
Penyelesaian
Gunakan Teorema Bayes:
𝑃(𝑃∣𝑇)=𝑃(𝑇∣𝑃)⋅𝑃( 𝑃 ) / 𝑃(𝑇)
Langkah1: Cari 𝑃(𝑇)
𝑃(𝑇)=𝑃(𝑇∣𝑃)⋅𝑃( 𝑃 )+𝑃(𝑇∣¬𝑃)⋅𝑃(¬𝑃)
P(T)=(0.9⋅0.01)+(0.05⋅0.99)=0.009+0.0495=0.0585
Langkah 2: Hitung 𝑃(𝑃∣𝑇)
𝑃(𝑃∣𝑇)=0.9⋅0.01 / 0.0585=0.154
Jadi, probabilitas seseorang benar-benar memiliki penyakit jika hasil tes positif adalah 15.4%.



## Refrensi

1. https://info.populix.co/articles/statistik-bayesian/#
2. https://kumparan.com/berita-terkini/2-contoh-soal-teorema-bayes-dalam-pelajaran-matematika-beserta-jawabannya-20UEmgQrt1l/1
3. https://corporatefinanceinstitute.com/resources/data-science/bayes-theorem/
