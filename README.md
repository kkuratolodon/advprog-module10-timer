## 1.2. Understanding how it works.
![alt text](image.png)

Berdasarkan Gambar di atas, yang pertama muncul di output adalah "Irfan's Computer: hey hey!" karena baris ini dieksekusi sebelum memanggil fungsi drop(spawner) dan executor.run(). Artinya, pesan ini dicetak langsung pada thread utama sebelum executor mulai menjalankan task yang ada di dalam spawner. Ketika executor dimulai, task yang telah disiapkan sebelumnya baru akan dijalankan. Output kemudian akan menunjukkan "Irfan's Computer: howdy!" dan setelah menunggu dua detik, akan menampilkan "Irfan's Computer: done!". Dengan demikian, "Irfan's Computer: hey hey!" muncul pertama karena dieksekusi langsung di thread utama sebelum executor menjalankan task asinkron yang telah diatur.

