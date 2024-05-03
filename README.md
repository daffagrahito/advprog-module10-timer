# Module 10 - Asynchronous Programming - Timer

> ##### Muhammad Daffa Grahito Triharsanto - 2206820075 - Pemrograman Lanjut B

## 1.2. Understanding how it works.
![Image 1.2](assets/images/1.2.png)
Berdasarkan gambar tersebut terlihat bahwa print statement "hey hey" lebih dulu daripada "howdy!" dan "done!". Print statement hey hey tidak berada di dalam asynchronous tasknya melainkan di main thread. Jadi, sampai executor nya memanggil function `run()` maka `spawner.spawn(async {...});` belum akan meng-*execute* tasknya itu.