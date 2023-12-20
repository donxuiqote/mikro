<b> IMPLEMENTASI SVM SEBAGAI PENGGANTI PENGENDALI PID PADA KIT ITCLAB </b>

- Mikrokontroler, bentuk kecil komputer dalam chip IC, difungsikan sebagai pengendali dalam elektronika. Terdiri dari CPU, memori, I/O, dan unit pendukung, mikrokontroler digunakan luas dalam otomotif, perangkat rumah tangga, perangkat medis, dll. Keunggulan meliputi ukuran kecil, konsumsi daya rendah, dan harga terjangkau.

- IoT adalah konsep di mana objek dilengkapi teknologi untuk berkomunikasi melalui internet. Dengan sensor dan perangkat lunak, IoT memecahkan masalah manusia di berbagai bidang seperti pertanian, kesehatan, dan transportasi. Pentingnya keamanan dan privasi data perlu diperhatikan.

- Sistem Kendali PID menggabungkan tiga aksi kendali untuk hasil dengan risetime cepat dan error kecil. Aksi proporsional, integral, dan derivatif memiliki keunggulan masing-masing.

- Deep Learning, metode AI terinspirasi otak manusia, digunakan untuk pemahaman dan pengambilan keputusan tingkat tinggi. Diterapkan dalam mobil otonom, deep learning mengolah data kompleks dan tidak terstruktur untuk solusi inovatif.

- SVM (Support Vector Machine) adalah algoritma pembelajaran mesin untuk klasifikasi dan regresi. Memaksimalkan jarak antara kelas data yang berbeda, SVM efektif dalam ruang fitur tinggi dan aplikasi seperti pengenalan pola dan klasifikasi teks.


################################

Data dikumpulkan dengan menggunakan perangkat lunak emulasi TCLab. Emulator TCLab diatur pada kecepatan 100 kali selama tahap pengumpulan data. Setpoint suhu divariasikan selama simulasi, mencerminkan nilai target pengendalian suhu. Pembacaan sensor suhu dan penyesuaian aktuator untuk mencapai setpoint dilakukan sebanyak dijalankannya loop Emulator, yaitu 540.

Algoritma digunakan untuk prediksi atau klasifikasi pada data baru. Proses pelatihan ini melibatkan dua tahap utama: pembentukan model dan penentuan parameter.

Evaluasi kinerja antara pengendali PID tradisional, pengendali PID berbasis deep learning, dan pengendali berbasis LSTM. Tiga metrik evaluasi utama yang digunakan adalah rising time, settling time, dan overshoot.

Grafik kinerja PID berbasis deep learning memperlihatkan perbedaan antara sistem PID tradisional dan PID SVM dalam beberapa aspek kritis. PID tradisional lebih cepat dalam rising time, dengan perbedaan waktu 15 detik lebih singkat dibandingkan dengan PID SVM. Namun, pada settling time, PID SVM lebih efisien, memerlukan waktu 1 detik lebih sedikit daripada PID tradisional untuk mencapai nilai yang mendekati setpoint secara stabil.

Analisis overshoot menunjukkan bahwa PID tradisional memiliki overshoot lebih kecil (0.81%) dibandingkan dengan PID SVM. Ini menandakan bahwa PID tradisional lebih mampu menghasilkan respons yang lebih stabil dan minim overshoot dibandingkan dengan PID SVM.

Grafik kinerja memberikan gambaran komprehensif tentang keunggulan dan kelemahan masing-masing metode pengendalian, memungkinkan pemahaman yang lebih baik tentang performa keduanya dalam konteks sistem dan tujuan kontrol yang spesifik.
