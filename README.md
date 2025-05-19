# Simulasi Tata Surya Imersif dan Interaktif

Halo! Selamat datang di proyek **Simulasi Tata Surya Imersif dan Interaktif** saya.

Perkenalkan, saya **Muhammad Zaky Zikra Nur** dengan **NIM 23404044**. Proyek ini disusun sebagai bagian dari pemenuhan tugas mata kuliah Media Digital Interaktif, program studi Teknologi Rekayasa Multimedia, Politeknik Dewantara, di bawah bimbingan dosen pengampu, **Ibu Nabila Febriyanti, S.Pd., M.Pd.**

## Tentang Proyek

Simulasi Tata Surya ini merupakan sebuah aplikasi berbasis web yang dirancang untuk menciptakan pengalaman menjelajahi keajaiban tata surya kita secara lebih seru, imersif, dan edukatif. Dengan antarmuka yang interaktif dan visual yang menarik, pengguna diajak untuk mengenal lebih dekat berbagai objek langit. Proyek ini telah melalui serangkaian iterasi pengembangan, dimulai dari visualisasi dasar hingga penambahan fitur-fitur interaktif yang kompleks dan desain ulang antarmuka pengguna.

<div style="border: 1px solid #30363d; border-radius: 6px; padding: 16px; margin: 20px auto; background-color: #0d1117; color: #c9d1d9; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji'; max-width: 680px;">
    <div style="text-align: center; margin-bottom: 16px;">
        <h2 style="color: #58a6ff; margin-top: 0; margin-bottom: 8px; font-size: 1.75em; font-weight: 600;">
            🌌 Simulasi Tata Surya Interaktif 🪐
        </h2>
        <p style="font-size: 1.1em; color: #8b949e; margin-bottom: 16px;">
            Jelajahi keajaiban tata surya kita secara imersif, interaktif, dan edukatif!
        </p>
    </div>
    <div style="background-color: #161b22; padding: 12px; border-radius: 6px; margin-bottom: 20px;">
        <h3 style="color: #58a6ff; margin-top: 0; margin-bottom: 10px; border-bottom: 1px solid #30363d; padding-bottom: 6px; font-size: 1.3em;">Fitur Unggulan:</h3>
        <ul style="list-style-type: '🌠 '; padding-left: 20px; font-size: 1em; color: #adbac7;">
            <li style="margin-bottom: 8px;">Visualisasi 3D Planet & Matahari yang Detail.</li>
            <li style="margin-bottom: 8px;">Kontrol Interaktif: Zoom, Kecepatan Orbit, Garis Orbit & Sumbu, Tema.</li>
            <li style="margin-bottom: 8px;">Panel Informasi Rinci dengan Fakta Unik.</li>
            <li style="margin-bottom: 8px;">Efek Visual: Hover & Klik Responsif, Latar Belakang Dinamis.</li>
            <li style="margin-bottom: 8px;">Suara Ambien Angkasa & Efek Tombol (memerlukan interaksi pengguna).</li>
        </ul>
    </div>
    <div style="text-align: center; margin-top: 20px; margin-bottom: 16px;">
        <a href="https://muhammadzakizn.github.io/Simulasi-Tata-Surya-Imersif-dan-Interaktif/" target="_blank" style="background-color: #238636; color: white; padding: 10px 20px; text-decoration: none; border-radius: 6px; font-size: 1.1em; font-weight: bold; display: inline-block; border: 1px solid #2ea043; transition: background-color 0.2s ease;">
            🚀 Lihat Simulasi Langsung!
        </a>
    </div>
    <p style="text-align: center; font-size: 0.85em; color: #8b949e; margin-top: 16px; border-top: 1px solid #30363d; padding-top: 12px;">
        Dibuat dengan <span style="color: #e53e3e;">❤️</span> menggunakan Three.js & Tone.js
    </p>
</div>

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

Untuk mendapatkan pengalaman visual dan interaktif yang optimal, disarankan untuk mengakses simulasi ini melalui perangkat dengan layar yang lebih besar seperti laptop atau komputer desktop. Browser modern seperti Chrome atau Firefox juga direkomendasikan. **Penting: Setelah halaman dimuat, lakukan klik pertama di mana saja pada area simulasi untuk mengaktifkan konteks audio dan memastikan semua fitur suara berfungsi dengan baik.**

Demikian deskripsi proyek Simulasi Tata Surya ini. Perlu dicatat bahwa proyek ini telah disempurnakan dan beberapa aspeknya digeneralisasi dengan bantuan teknologi AI untuk meningkatkan kualitas dan fungsionalitasnya.

Anda dapat mengakses simulasi ini secara langsung melalui tautan berikut:
[https://muhammadzakizn.github.io/Simulasi-Tata-Surya-Imersif-dan-Interaktif/](https://muhammadzakizn.github.io/Simulasi-Tata-Surya-Imersif-dan-Interaktif/)

Terima kasih atas perhatiannya!

## Riwayat Perubahan

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
* **Fitur Garis Orbit & Poros (Awal):**
    * Visualisasi garis orbit yang jelas untuk setiap planet.
    * Implementasi awal visualisasi poros rotasi pada setiap planet dan Bulan.
    * Penambahan tombol kontrol terpisah untuk menampilkan/menyembunyikan garis orbit dan poros rotasi.
* **Peningkatan Interaksi Pengguna (Awal):**
    * **Efek Hover (Dasar):** Planet (dan bulannya) berhenti berotasi/mengorbit saat kursor mouse diarahkan ke atasnya.
    * **Efek Klik (Dasar):** Kamera melakukan zoom-in optik (FOV menyempit) saat objek diklik.
    * **Tooltip Nama:** Tooltip muncul menampilkan nama objek saat kursor diarahkan ke atasnya.
* **Panel Informasi yang Disempurnakan:**
    * Perbaikan masalah teks yang terpotong pada versi awal.
    * Penambahan informasi yang lebih detail untuk setiap objek langit.
    * Styling khusus dengan box untuk bagian "Fakta Unik".
* **Kontrol Kamera:**
    * Integrasi `OrbitControls` dari Three.js untuk memungkinkan pengguna melakukan zoom in/out dengan roda mouse, menggeser (pan) dengan tombol kanan mouse, dan memutar (orbit) kamera dengan tombol kiri mouse.
    * Animasi kamera otomatis awal (orbit perlahan) akan berhenti setelah pengguna mulai berinteraksi dengan `OrbitControls`.
    * Transisi zoom-out yang lebih mulus saat panel informasi ditutup.

---

### **V3.0: Desain Ulang Antarmuka, Kontrol Lanjutan, & Interaktivitas Ditingkatkan**

* **Desain Ulang Menu Utama (Fokus UI/UX):**
    * Semua tombol kontrol disatukan dalam satu tombol "Menu" utama berbentuk kapsul yang terletak di tengah bawah layar, menggantikan tata letak sebelumnya.
    * Ikon tombol menu utama berupa "grid" (kotak-kotak) dan berubah menjadi ikon "close" (X) saat menu aktif, memberikan umpan balik visual yang jelas.
    * Animasi dinamis pada tombol menu utama saat diklik untuk pengalaman yang lebih responsif.
* **Tombol Fitur Pop-Out yang Intuitif:**
    * Saat menu utama dibuka, tombol-tombol fitur lainnya (Toggle Orbit, Toggle Poros, Pengaturan Latar, Zoom, Kecepatan, Pause/Play, Suara, Tema) muncul secara animasi dengan efek staggered di samping kiri dan kanan tombol menu utama.
    * Semua tombol fitur berbentuk kapsul dengan ikon dan teks judul yang jelas untuk identifikasi fungsi yang mudah.
* **Peningkatan Interaksi Objek Langit:**
    * **Efek Hover Lebih Responsif:** Planet, Matahari, dan Bulan akan melambat secara signifikan saat kursor diarahkan ke atasnya (kecuali jika panel info terbuka atau simulasi dijeda).
    * **Tooltip Nama:** Label nama objek muncul secara instan saat kursor diarahkan ke atasnya untuk identifikasi cepat.
* **Fitur Fullscreen Terintegrasi:**
    * Tombol fullscreen ditambahkan di dalam pop-up kontrol zoom untuk akses mudah.
    * Saat mode fullscreen aktif, menu utama bertransformasi menjadi tombol bulat minimalis di pojok kiri bawah layar.
    * Tombol-tombol fitur di dalam menu fullscreen juga menjadi bulat dan hanya menampilkan ikon, mengoptimalkan ruang layar.
    * Perbaikan definisi fungsi terkait fullscreen (`updateFullscreenButtonIcon`, `toggleFullscreenMode`, `handleFullscreenChange`).
* **Kontrol Visualisasi Tambahan:**
    * **Garis Sumbu (Poros Rotasi):**
        * Visualisasi garis sumbu ditambahkan untuk setiap planet, Matahari, dan Bulan, yang merepresentasikan kemiringan aksial masing-masing (data `axialTilt` ditambahkan ke `planetData`).
        * Tombol toggle "Garis Sumbu" di dalam pop-up "Pengaturan Tema Visual" untuk menampilkan/menyembunyikan garis-garis ini.
        * Panjang garis sumbu disesuaikan menjadi lebih proporsional (sekitar 1.6 kali radius objek) untuk semua objek langit dan opasitasnya ditingkatkan menjadi 0.6.
    * **Garis Orbit:**
        * Visibilitas garis orbit kini dapat diatur melalui tombol toggle "Garis Orbit" di dalam pop-up "Kecepatan Orbit & Animasi".
        * Opasitas default garis orbit ditingkatkan menjadi `0.5` agar lebih jelas terlihat.
* **Fungsionalitas Kontrol yang Disempurnakan:**
    * **Kontrol Zoom Lanjutan:** Tombol "Zoom" di menu fitur kini berfungsi sebagai toggle untuk menampilkan/menyembunyikan tombol "Zoom In" dan "Zoom Out" yang lebih kecil, yang muncul di dekat tombol "Zoom" utama.
    * **Kontrol Kecepatan Orbit Presisi:** Tombol fitur "Kecepatan" ditambahkan ke menu, yang saat diklik, menampilkan tombol "Percepat" dan "Perlambat" orbit.
* **Pengaturan Latar Belakang yang Lebih Kaya:**
    * Tombol "Pengaturan Latar" di menu fitur.
    * Panel pop-up untuk menampilkan/menyembunyikan Lubang Hitam, Galaksi Jauh, dan Bintang Latar.
    * Kontrol untuk menambah/mengurangi kepadatan bintang dan galaksi jauh.
* **Penyempurnaan Visual Latar Belakang:**
    * Visual galaksi jauh disempurnakan agar lebih menyebar dan tidak menggumpal, dengan variasi warna yang lebih halus.
    * Representasi visual lubang hitam menggunakan `TorusGeometry` untuk cakram akresi yang lebih realistis dan detail, dengan bagian tengah yang gelap pekat.
* **Konsistensi UI dan Perbaikan Bug:**
    * Penggunaan font Roboto sebagai font utama untuk meningkatkan keterbacaan di seluruh antarmuka.
    * Styling glassmorphism diterapkan secara konsisten pada semua elemen kontrol (tombol dan panel pop-up).
    * Perbaikan berkelanjutan pada bug terkait zoom, interaksi hover, dan logika panel informasi.
    * Memastikan semua objek langit (termasuk Bulan) memiliki data yang diperlukan (`axialTilt`, dll.) untuk fitur-fitur baru.
    * Perbaikan fungsi `handleMouseWheelZoom` yang hilang pada iterasi sebelumnya.

---

### **V4.0: Optimalisasi Audio & Inisialisasi Lanjutan**

* **Peningkatan Suara Ambien Angkasa:**
    * Implementasi suara latar angkasa yang lebih imersif menggunakan `NoiseSynth` dengan tipe 'brown' dari Tone.js.
    * Penambahan `AutoFilter` dengan LFO (Low-Frequency Oscillator) yang lambat untuk memberikan efek "sapuan" atau "nafas" pada suara, menciptakan nuansa ruang angkasa yang lebih dinamis.
    * Penggunaan `Reverb` untuk menambah kesan ruang yang luas pada suara ambien.
    * Node `Volume` terpisah untuk mengontrol level keseluruhan suara ambien ini.
* **Perbaikan Inisialisasi Audio (Autoplay & Stabilitas):**
    * `Tone.start()` (untuk mengaktifkan konteks audio browser) kini dipanggil hanya setelah pengguna melakukan interaksi pertama (klik di mana saja pada halaman) untuk mematuhi kebijakan autoplay browser modern dan mencegah error "The AudioContext was not allowed to start".
    * Semua *synthesizer* (suara klik dan ambien) diinisialisasi hanya setelah `Tone.start()` berhasil dijalankan (di dalam blok `.then()` dan setelah `Tone.loaded()` untuk memastikan semua komponen siap).
    * Suara ambien akan berusaha dimulai secara otomatis setelah inisialisasi berhasil dan jika volume tidak di-*mute*.
    * Fungsi `applyCurrentVolumeToSynth` disempurnakan untuk hanya mengatur volume dan status *mute* pada *synthesizer* yang sudah ada, dan tidak mencoba memulainya berulang kali untuk mencegah error.
* **Sinkronisasi Animasi Intro Menu:**
    * Animasi intro untuk menu utama (munculnya tombol-tombol dari bawah layar) sekarang diaktifkan dari JavaScript setelah konteks audio berhasil dimulai, memastikan pengalaman pengguna yang lebih mulus dan mencegah UI macet jika ada masalah dengan audio.
* **Perbaikan Stabilitas dan Debugging:**
    * Penambahan `console.log` yang lebih detail untuk membantu diagnosis masalah terkait audio dan urutan inisialisasi.
    * Penyesuaian CSS untuk memastikan posisi tombol menu utama tetap di tengah bawah layar secara default sebelum animasi intro dijalankan.

---
