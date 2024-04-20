## Diagnosa Penyakit Menggunakan Teorema Bayes

### Pendahuluan

Seorang dokter di klinik medis ingin menggunakan Teorema Bayes untuk mendiagnosis penyakit tertentu. Dokter tersebut memiliki informasi dasar sebagai berikut:

1. Tingkat keparahan penyakit pada populasi umum adalah **1%**.
2. Tes laboratorium memiliki tingkat kesalahan positif palsu **5%** dan kesalahan negatif palsu **2%**.
3. Pasien datang dengan gejala yang terjadi pada orang sehat juga.
4. Dokter ingin menghitung probabilitas bahwa pasien yang mendapat tes positif juga memiliki penyakit tersebut.

### Langkah-langkah

1. **Menentukan Probabilitas Prior:** Probabilitas prior adalah probabilitas awal bahwa pasien memiliki penyakit sebelum hasil tes dilakukan. Dalam kasus ini, probabilitas prior adalah **1%**.

   $$P(\text{penyakit}) = 0.01$$

   

2. Menghitung Probabilitas Posterior:

   Probabilitas posterior dihitung menggunakan Teorema Bayes.

   - **Probabilitas Tes Positif pada Individu Sakit:** 

     Probabilitas tes positif pada individu yang benar-benar sakit adalah **98%**.

     $$P(\text{positif}|\text{sakit}) = 1 - \text{tingkat kesalahan negatif palsu}$$

     

   - **Probabilitas Tes Negatif pada Individu Sehat:** 

     Probabilitas tes negatif pada individu yang tidak sakit adalah **95%**.

     $$P(\text{negatif}|\text{sehat}) = 1 - \text{tingkat kesalahan positif palsu}$$

     

   - **Probabilitas Tes Positif Secara Keseluruhan:** Probabilitas tes positif secara keseluruhan dihitung dengan hukum total probabilitas, dan didapatkan **0.0593**.

     $$P(\text{positif}) = P(\text{positif}|\text{sakit}) \times P(\text{sakit}) + P(\text{positif}|\text{sehat}) \times P(\text{sehat})$$

     

   - **Menggunakan Teorema Bayes:** 
   
     $$P(H|X) = \frac{{P(X | H) \times P(H)}}{{P(X)}}$$
   
     Di mana:
     
     - `P(H|X)` adalah probabilitas posterior dari hipotesis \( H \) setelah diberikan data \( X \).
     - `P(X | H)` adalah probabilitas likelihood dari data \( X \) jika hipotesis \( H \) benar.
     - `P(H)` adalah probabilitas prior dari hipotesis \( H \).
     - `P(X)` adalah probabilitas dari data \( X \) secara keseluruhan.
     
     Rumus ini digunakan untuk memperbarui probabilitas prior dengan informasi baru yang diberikan oleh data, sehingga menghasilkan probabilitas posterior yang diperbarui.
     
     Dengan menggunakan rumus Teorema Bayes, probabilitas posterior dihitung dan didapatkan **0.16526**.

### Kesimpulan

Probabilitas posterior **16.526%** menunjukkan bahwa ada kemungkinan **16.526%** pasien yang mendapat tes positif benar-benar memiliki penyakit tersebut. Informasi ini membantu dokter dalam mendiagnosis penyakit dengan memberikan panduan tambahan dalam menetapkan diagnosis dan memilih langkah-langkah pengobatan yang sesuai. Semakin tinggi probabilitas posterior, semakin besar kemungkinan pasien memiliki penyakit tersebut, dan dokter mungkin perlu melakukan lebih banyak tes atau pengamatan untuk mengonfirmasi diagnosis.

Hasil probabilitas posterior ini sangat penting dalam konteks medis karena memberikan perkiraan yang lebih akurat tentang kemungkinan seorang pasien menderita penyakit tertentu setelah hasil tes laboratorium. Informasi ini membantu dokter dalam proses diagnosa penyakit dengan memberikan panduan tambahan selain hanya hasil tes itu sendiri. Dengan memperhitungkan probabilitas posterior, dokter dapat membuat keputusan yang lebih tepat tentang tindakan medis yang diperlukan, seperti mengirim pasien untuk lebih banyak tes atau memulai perawatan yang sesuai lebih awal. Ini mengoptimalkan penggunaan sumber daya kesehatan dan meningkatkan kesempatan untuk pengobatan yang berhasil.

### Jupyter Notebook 

Kunjungi notebook interaktif berikut untuk solusi dan penjelasan lebih lanjut!
https://github.com/dikhimartin/probabilitas-posterior-teorema-bayes-diagnosa-medis/blob/master/main.ipynb

Cara menjalankan 
---------------
Saya merekomendasikan penggunaan Visual Studio Code untuk mengakses file `.ipynb`. karena sudah dilengkapi dengan Jupyter notebook dan terminal. Namun, jika Anda lebih suka menggunakan terminal + server jupyterlab, juga di perbolehkan. Silakan ikuti langkah-langkah berikut untuk menyiapkan envinronment agar dapat menjalankan file:

Mulailah dengan menginstal [Anaconda](https://www.anaconda.com/products/distribution) (atau [Miniconda](https://docs.conda.io/en/latest/miniconda.html)), [git](https://git-scm.com/downloads), 

Selanjutnya, clone repositori ini dengan membuka terminal dan mengetikkan perintah berikut (jangan ketik tanda $ pertama pada setiap baris, itu hanya menunjukkan bahwa ini adalah perintah terminal):

    $ git clone https://github.com/dikhimartin/probabilitas-posterior-teorema-bayes-diagnosa-medis
    $ cd probabilitas-posterior-teorema-bayes-diagnosa-medis

Selanjutnya, jalankan perintah-perintah berikut:

    $ conda env create -f environment.yml
    $ conda activate bol_datascience_course
    $ python -m ipykernel install --user --name=bol_datascience_course

Jika Anda tidak menggunakan Visual Studio Code, Anda perlu memulai Jupyter Lab untuk dapat membuka notebook ipynb.

    $ jupyter lab

Catatan :
 Untuk mengaktifkan environment ini, menggunakan

     $ conda activate bol_datascience_course

 Untuk menonaktifkan environment yang aktif , gunakan

     $ conda deactivate    



Referensi
--------

Muehlemann, N., Zhou, T., Mukherjee, R., Hossain, M. I., Roychoudhury, S., & Russek-Cohen, E. (2023). A Tutorial on Modern Bayesian Methods in Clinical Trials. *Therapeutic Innovation and Regulatory Science*, *57*(3), 402–416. https://doi.org/10.1007/s43441-023-00515-3

Verma, V., Mishra, A. K., & Narang, R. (2019). Application of Bayesian analysis in medical diagnosis. *Journal of the Practice of Cardiovascular Sciences*, *5*(3), 136. https://doi.org/10.4103/jpcs.jpcs_51_19

*Conditional probability with Bayes’ Theorem*. (n.d.). [Video]. Khan Academy. https://www.khanacademy.org/math/ap-statistics/probability-ap/stats-conditional-probability/v/bayes-theorem-visualized

Kelik, A., Dan, N., & Wardoyo, R. (2013). Sistem Pakar Menggunakan Teorema Bayes untuk Mendiagnosa Penyakit Kehamilan Expert System using Bayesian Theorem to Diagnose Pregnancy Diseases. In *Berkala MIPA* (Vol. 23, Issue 3). https://media.neliti.com/media/publications/241866-sistem-pakar-menggunakan-teorema-bayes-u-d0cb123a.pdf