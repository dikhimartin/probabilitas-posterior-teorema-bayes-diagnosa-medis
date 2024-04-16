# Diagnosa Penyakit Menggunakan Teorema Bayes

Seorang dokter di sebuah klinik medis ingin menggunakan Teorema Bayes untuk mendiagnosa penyakit tertentu. Dokter tersebut memiliki informasi dasar sebagai berikut:

1. Tingkat keparahan penyakit pada populasi umum adalah `1%`.
2. Tes laboratorium memiliki tingkat kesalahan positif palsu `5%` dan kesalahan negatif palsu `2%`.
3. Pasien datang dengan gejala yang terjadi pada orang sehat juga.
4. Dokter ingin menghitung probabilitas bahwa pasien yang mendapat tes positif juga memiliki penyakit tersebut.

**Pertanyaan:**
1. Apa probabilitas prior bahwa pasien memiliki penyakit?
2. Berapa probabilitas posterior bahwa pasien yang mendapat tes positif benar-benar memiliki penyakit?

**Langkah-langkah:**
1. Tentukan probabilitas prior.
2. Hitung probabilitas tes positif pada individu yang sakit dan sehat.
3. Hitung probabilitas tes positif secara keseluruhan.
4. Gunakan Teorema Bayes untuk menghitung probabilitas posterior.

Kunjungi notebook interaktif berikut untuk solusi dan penjelasan lebih lanjut!
https://github.com/dikhimartin/probabilitas-posterior-teorema-bayes-diagnosa-medis/blob/master/Menghitung_Probabilitas_Posterior_Menggunakan_Teorema_Bayes.ipynb

Memulai
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