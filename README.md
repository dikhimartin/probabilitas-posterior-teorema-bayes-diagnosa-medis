Tugas Pribadi 2 part 1 - Studi kasus dalam sebuah klinik medis  
==================

Dalam sebuah klinik medis, seorang dokter ingin menggunakan Teorema Bayes untuk membantu dalam mendiagnosa penyakit tertentu. Dokter tersebut memiliki beberapa informasi dasar sebagai berikut:

1. Tingkat keparahan penyakit pada populasi umum adalah 1%.
2. Tes laboratorium yang tersedia memiliki tingkat kesalahan positif palsu sebesar 5% (tes positif pada individu sehat) dan tingkat kesalahan negatif palsu sebesar 2% (tes negatif pada individu yang sakit).
3. Pasien datang dengan gejala tertentu yang dapat dikaitkan dengan penyakit ini. Tetapi, gejala tersebut dapat terjadi pada orang sehat juga.
4. Dokter ingin menghitung probabilitas bahwa seorang pasien yang mendapat tes positif pada tes laboratorium juga benar-benar memiliki penyakit tersebut.

Berdasarkan informasi yang diberikan, hitung probabilitas prior (prior probability) bahwa seorang pasien yang datang ke klinik tersebut benar-benar memiliki penyakit ini.

Gunakan Teorema Bayes untuk menghitung probabilitas posterior (posterior probability) bahwa seorang pasien yang mendapat tes positif pada tes laboratorium juga benar-benar memiliki penyakit ini.

Apa arti dari hasil probabilitas posterior ini dalam konteks medis? Bagaimana informasi ini dapat membantu dokter dalam proses diagnosa penyakit?


Memulai
---------------
Saya merekomendasikan penggunaan Visual Studio Code untuk mengakses file `.ipynb`. karena sudah dilengkapi dengan Jupyter notebook dan terminal. Namun, jika Anda lebih suka menggunakan terminal + server jupyterlab, juga di perbolehkan. Silakan ikuti langkah-langkah berikut untuk menyiapkan envinronment agar dapat menjalankan file:

Mulailah dengan menginstal [Anaconda](https://www.anaconda.com/products/distribution) (atau [Miniconda](https://docs.conda.io/en/latest/miniconda.html)), [git](https://git-scm.com/downloads), 

Selanjutnya, clone repositori ini dengan membuka terminal dan mengetikkan perintah berikut (jangan ketik tanda $ pertama pada setiap baris, itu hanya menunjukkan bahwa ini adalah perintah terminal):

    $ git clone https://github.com/dikhimartin/binus-tk-3-data-science.git
    $ cd binus-tk-3-data-science

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
* [Hands-on Machine Learning with Scikit-Learn, Keras and TensorFlow (3rd edition)](https://homl.info/er3)
