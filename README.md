# Simulasi Tata Surya Imersif dan Interaktif

Halo! Selamat datang di proyek **Simulasi Tata Surya Imersif dan Interaktif** saya.

Perkenalkan, saya **Muhammad Zaky Zikra Nur** dengan **NIM 23404044**. Proyek ini disusun sebagai bagian dari pemenuhan tugas mata kuliah Media Digital Interaktif, program studi Teknologi Rekayasa Multimedia, Politeknik Dewantara, di bawah bimbingan dosen pengampu, **Ibu Nabila Febriyanti, S.Pd., M.Pd.**

## Tentang Proyek

Simulasi Tata Surya ini merupakan sebuah aplikasi berbasis web yang dirancang untuk menciptakan pengalaman menjelajahi keajaiban tata surya kita secara lebih seru, imersif, dan edukatif. Dengan antarmuka yang interaktif dan visual yang menarik, pengguna diajak untuk mengenal lebih dekat berbagai objek langit. Proyek ini telah melalui serangkaian iterasi pengembangan, dimulai dari visualisasi dasar hingga penambahan fitur-fitur interaktif yang kompleks dan desain ulang antarmuka pengguna.

## Alur Pengembangan dan Fitur Utama

Evolusi proyek ini dapat dirangkum dalam beberapa tahap utama:

1.  **Fondasi Awal:** Tahap ini meliputi pembuatan visual dasar planet-planet dan Matahari, lengkap dengan pewarnaan, ukuran relatif, serta simulasi gerakan rotasi dan orbit. Panel informasi sederhana juga diimplementasikan, bersama dengan kontrol dasar seperti jeda/mulai animasi, suara, dan tema visual (siang/malam).

2.  **Peningkatan Interaktivitas dan Detail Visual:** Iterasi selanjutnya berfokus pada memperkaya pengalaman pengguna. Fitur seperti visualisasi garis orbit dan poros rotasi (yang dapat di-toggle) ditambahkan. Interaksi dengan objek langit ditingkatkan melalui:
    * **Efek Hover:** Planet dan bulan akan berhenti bergerak dan sedikit di-zoom (menggunakan perubahan FOV kamera) saat kursor diarahkan, disertai efek cahaya lembut (kecuali untuk Matahari yang tidak memiliki hover glow).
    * **Efek Klik:** Objek yang diklik (termasuk Matahari) akan memicu zoom kamera otomatis ke arahnya dan menampilkan panel informasi yang lebih rinci. Efek cahaya "shiny" yang intens juga muncul di belakang objek yang diklik; Matahari mendapatkan efek "terbakar" yang dinamis pada teksturnya dan glow permanen yang diperkuat saat panelnya terbuka.
    * **Tooltip:** Nama objek muncul saat di-hover untuk identifikasi cepat.
    * **Panel Informasi:** Konten panel diperkaya dengan data detail dan fakta unik, serta perbaikan tata letak.

3.  **Desain Ulang Antarmuka dan Kontrol Lanjutan:** Tahap terkini melibatkan perombakan besar pada antarmuka pengguna untuk pengalaman yang lebih modern dan intuitif:
    * **Menu Kapsul Terpusat:** Semua tombol kontrol utama kini terintegrasi dalam satu tombol "Menu" berbentuk kapsul di tengah bawah layar, dengan ikon "grid" yang berubah menjadi "close" saat aktif.
    * **Tombol Fitur Pop-Out:** Saat menu utama dibuka, tombol-tombol fitur lainnya (kontrol orbit, poros, latar, zoom, kecepatan, pause/play, suara, tema) muncul secara animasi di sekitarnya, masing-masing dengan ikon dan teks yang jelas.
    * **Kontrol Zoom dan Kecepatan:** Tombol "Zoom" dan "Kecepatan" di menu fitur kini memiliki sub-menu pop-out sendiri untuk kontrol yang lebih presisi (Zoom In/Out, Percepat/Perlambat).
    * **Pengaturan Latar Belakang:** Fitur untuk mengatur visibilitas dan kepadatan elemen latar seperti bintang, galaksi jauh, dan lubang hitam. Visual lubang hitam juga disempurnakan agar lebih realistis.
    * **Konsistensi UI:** Gaya "glassmorphism" diterapkan pada semua elemen kontrol, dan font Roboto digunakan untuk meningkatkan keterbacaan.

## Saran Penggunaan

Untuk mendapatkan pengalaman visual dan interaktif yang optimal, disarankan untuk mengakses simulasi ini melalui perangkat dengan layar yang lebih besar seperti laptop atau komputer desktop.

Demikian deskripsi proyek Simulasi Tata Surya ini. Perlu dicatat bahwa proyek ini telah disempurnakan dan beberapa aspeknya digeneralisasi dengan bantuan teknologi AI untuk meningkatkan kualitas dan fungsionalitasnya.

Anda dapat mengakses simulasi ini secara langsung melalui tautan berikut:
[https://muhammadzakizn.github.io/Simulasi-Tata-Surya-Imersif-dan-Interaktif/](https://muhammadzakizn.github.io/Simulasi-Tata-Surya-Imersif-dan-Interaktif/)

Terima kasih atas perhatiannya!

## Riwayat perubahan 
### **V1.0: Dasar Simulasi (Iterasi Awal)**

* **Fitur Utama:**
    * Visualisasi dasar planet-planet Tata Surya (Merkurius hingga Neptunus) dan Matahari.
    * Implementasi pewarnaan, ukuran relatif, dan jarak orbit dasar untuk setiap objek.
    * Gerakan rotasi planet pada porosnya dan revolusi (orbit) mengelilingi Matahari.
    * Kamera perspektif dengan pandangan awal ke seluruh sistem.
    * Pencahayaan ambient dan titik (dari Matahari) untuk menerangi scene.
    * Latar belakang bintang statis sederhana.
* **Interaksi:**
    * Panel informasi awal muncul saat planet diklik, menampilkan data dasar (nama, deskripsi singkat).
* **Kontrol Pengguna:**
    * Tombol untuk menjeda/melanjutkan animasi orbit dan rotasi.
    * Tombol untuk mengaktifkan/menonaktifkan suara ambient angkasa (menggunakan Tone.js).
    * Tombol untuk mengganti tema visual antara mode terang (siang) dan gelap (malam).

---

### **V2.0: Peningkatan Interaksi & Visual (Iterasi Menengah)**

* **Peningkatan Visual Objek Langit:**
    * Tekstur Matahari dibuat lebih dinamis menyerupai bola api dengan efek permukaan yang bergejolak.
    * Penambahan cincin untuk Saturnus.
    * Penambahan Bulan sebagai satelit Bumi, dengan orbit dan rotasinya sendiri.
* **Fitur Garis Orbit & Poros:**
    * Visualisasi garis orbit yang jelas untuk setiap planet.
    * Implementasi visualisasi poros rotasi (berupa silinder tipis) pada setiap planet dan Bulan, dengan kemiringan aksial yang sesuai.
    * Penambahan tombol kontrol terpisah untuk menampilkan/menyembunyikan garis orbit dan poros rotasi.
* **Peningkatan Interaksi Pengguna:**
    * **Efek Hover:**
        * Planet (dan bulannya) berhenti berotasi/mengorbit saat kursor mouse diarahkan ke atasnya (kecuali jika panel info sedang terbuka untuk objek tersebut atau simulasi dijeda global).
        * Efek cahaya lembut (hover glow) berwarna kebiruan muncul di belakang planet/bulan saat di-hover (tidak berlaku untuk Matahari).
        * Kamera melakukan zoom-in optik (FOV menyempit sekitar 10%) saat hover pada planet/bulan (tidak untuk Matahari).
    * **Efek Klik:**
        * Efek cahaya "shiny" (click glow) yang lebih intens muncul di belakang planet/Matahari saat panel informasinya terbuka. Untuk Matahari, glow ini berwarna "berapi-api".
        * Kamera secara otomatis melakukan zoom ke objek yang diklik.
    * **Tooltip Nama:** Tooltip muncul menampilkan nama objek saat kursor diarahkan ke atasnya.
* **Panel Informasi yang Disempurnakan:**
    * Perbaikan masalah teks yang terpotong.
    * Penambahan informasi yang lebih detail dan rinci untuk setiap objek langit (deskripsi, jarak, periode orbit, diameter, suhu, gravitasi, bulan, atmosfer, penemuan, ciri khas).
    * Styling khusus dengan box untuk bagian "Fakta Unik".
* **Kontrol Kamera:**
    * Integrasi `OrbitControls` dari Three.js untuk memungkinkan pengguna melakukan zoom in/out dengan roda mouse, menggeser (pan) dengan tombol kanan mouse, dan memutar (orbit) kamera dengan tombol kiri mouse.
    * Animasi kamera otomatis awal (orbit perlahan) akan berhenti setelah pengguna mulai berinteraksi dengan `OrbitControls`.
    * Transisi zoom-out yang lebih mulus saat panel informasi ditutup, mengembalikan kamera ke pandangan awal yang lebih luas.

---

### **V3.0: Desain Ulang Antarmuka & Kontrol Lanjutan (Iterasi Terbaru)**

* **Desain Ulang Menu Utama:**
    * Semua tombol kontrol disatukan dalam satu tombol "Menu" utama berbentuk kapsul yang terletak di tengah bawah layar.
    * Ikon tombol menu utama berupa "grid" (kotak-kotak) dan berubah menjadi ikon "close" (X) saat menu aktif.
    * Animasi dinamis pada tombol menu utama saat diklik.
* **Tombol Fitur Pop-Out:**
    * Tombol-tombol fitur (Toggle Orbit, Toggle Poros, Pengaturan Latar, Zoom, Kecepatan, Pause/Play, Suara, Tema) muncul secara animasi dengan efek staggered di samping kiri dan kanan tombol menu utama.
    * Semua tombol fitur berbentuk kapsul dengan ikon dan teks judul yang jelas.
    * Jarak vertikal antara tombol menu utama dan barisan tombol fitur disesuaikan agar lebih rapat.
* **Fungsionalitas Tombol Zoom yang Disempurnakan:**
    * Tombol "Zoom" di menu fitur berfungsi sebagai toggle untuk menampilkan/menyembunyikan tombol "Zoom In" dan "Zoom Out" yang lebih kecil, yang muncul di dekat tombol "Zoom".
    * Tombol "Zoom In" dan "Zoom Out" aktif mengontrol perbesaran kamera menggunakan `controls.dollyIn()` dan `controls.dollyOut()`.
* **Fitur Kontrol Kecepatan Orbit:**
    * Tombol fitur "Kecepatan" ditambahkan ke menu.
    * Saat diklik, menampilkan tombol "Percepat" dan "Perlambat" orbit yang fungsional, menyesuaikan faktor kecepatan global.
* **Kontrol Latar Belakang Lanjutan:**
    * Tombol "Pengaturan Latar" di menu fitur.
    * Panel pop-up untuk menampilkan/menyembunyikan Lubang Hitam, Galaksi Jauh, dan Bintang Latar.
    * Kontrol untuk menambah/mengurangi kepadatan bintang dan galaksi jauh.
* **Penyempurnaan Visual Latar Belakang:**
    * Visual galaksi jauh disempurnakan agar lebih menyebar dan tidak menggumpal, dengan variasi warna yang lebih halus.
    * Representasi visual lubang hitam menggunakan `TorusGeometry` untuk cakram akresi yang lebih realistis dan detail, dengan bagian tengah yang gelap pekat.
* **Konsistensi UI dan Perbaikan Bug:**
    * Penggunaan font Roboto sebagai font utama.
    * Styling glassmorphism diterapkan secara konsisten pada tombol dan panel.
    * Perbaikan berkelanjutan pada bug zoom, terutama konflik antara animasi otomatis dan interaksi pengguna.
    * Memastikan semua tombol fitur memiliki struktur HTML yang konsisten untuk `icon-container` dan `text-container` guna mencegah perubahan ukuran yang tidak diinginkan.

---
