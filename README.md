Analisis
kita membangun model CNN sederhana dengan tiga lapisan konvolusi, lapisan max-pooling, dan lapisan Dense (fully connected) untuk klasifikasi. Kami menggunakan aktivasi ReLU di lapisan konvolusi dan lapisan Dense, dan menggunakan softmax pada lapisan keluaran. Kami juga melatih model selama 10 epoch dengan optimizer Adam.

- Epoch dan Waktu Pelatihan: Proses pelatihan model ini terdiri dari 10 epoch (iterasi melalui seluruh dataset) dan masing-masing epoch memakan waktu yang berbeda-beda

- Loss (Kerugian): Nilai loss pada epoch awal (Epoch 1) adalah  1.6413, dan secara bertahap menurun hingga mencapai  0.4889 pada Epoch 10. Ini menunjukkan bahwa model semakin baik dalam mengurangi kesalahan prediksi seiring dengan berjalannya waktu dan pelatihan.

- Akurasi: Akurasi awal model pada Epoch 1 adalah 0.4013 , yang berarti model hanya memprediksi dengan benar sekitar 40.13% dari data pelatihan. Namun, seiring dengan pelatihan, akurasi meningkat secara signifikan menjadi  0.8304 pada Epoch 10. Ini menunjukkan bahwa model semakin baik dalam mengklasifikasikan data pelatihan dengan benar.

- Val Loss (Kerugian Validasi) dan Val Accuracy (Akurasi Validasi): Selama pelatihan, selain melihat kinerja pada data pelatihan, kita juga memantau kinerja model pada data validasi yang terpisah. Val Loss mengalami fluktuasi, tetapi secara keseluruhan, cenderung meningkat pada tahap akhir pelatihan. Val Accuracy juga mengalami peningkatan, tetapi cenderung menurun sedikit pada akhirnya. Hal ini bisa mengindikasikan adanya overfitting, di mana model mungkin terlalu fokus pada data pelatihan dan kurang mampu menggeneralisasi pada data baru.
