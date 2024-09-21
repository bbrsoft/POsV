# POsV

Ini adalah contoh aplikasi mobile Android yang dirancang untuk digunakan pada Terminal POS Android di tempat penjualan.
Fitur

    Aplikasi ini dikembangkan dengan pola desain MVVM.
    Ada dua jenis pengguna dalam aplikasi: Manager dan Kasir (Manager juga merupakan kasir dengan semua hak akses).
    Pengguna dapat login ke sistem dan melakukan transaksi berdasarkan akun mereka.
    Pengguna dapat mengubah kata sandi mereka.
    Transaksi penjualan dapat dilakukan dan produk dapat ditawarkan kepada pelanggan.
    Produk dan kategori baru dapat ditambahkan dengan mudah.
    Pemilik bisnis (manajer) atau kasir (yang memiliki wewenang) dapat menambahkan kasir baru ke sistem.
    Memungkinkan untuk melihat pesanan sebelumnya dan memfilter pesanan sesuai kriteria yang diinginkan.
    Saat opsi pembayaran dengan kartu kredit dipilih, transaksi pembayaran dilakukan melalui perangkat POS.
    Setelah proses pembayaran selesai, struk fisik secara otomatis dihasilkan.
    Isi struk mencakup informasi pelanggan, informasi pesanan, dan logo aplikasi.

[![ Preview](1(1).png)](https://github.com/bbrsoft/POsV/blob/main/1%20(1).png?raw=true)
[![ Preview](1(1).png)](https://github.com/bbrsoft/POsV/blob/main/1%20(2).png?raw=true)
[![ Preview](1(1).png)](https://github.com/bbrsoft/POsV/blob/main/1%20(3).png?raw=true)
[![ Preview](1(1).png)](https://github.com/bbrsoft/POsV/blob/main/1%20(4).png?raw=true)
[![ Preview](1(1).png)](https://github.com/bbrsoft/POsV/blob/main/1%20(5).png?raw=true)
[![ Preview](1(1).png)](https://github.com/bbrsoft/POsV/blob/main/1%20(6).png?raw=true)

Perpustakaan yang Digunakan

    [Foundation]
        Android KTX - Digunakan untuk membuat aplikasi lebih mudah dibaca dan digunakan.
        AppCompat - Perpustakaan yang memastikan aplikasi Android kompatibel dengan desain material.
    [Architecture]
        Room - Digunakan untuk membuat dan mengelola database lokal.
        Lifecycles - Memudahkan pengelolaan siklus hidup aktivitas dan fragmen.
        LiveData - Digunakan untuk mengelola dan memantau aliran data.
        ViewModel - Untuk menyimpan dan berbagi data antar komponen UI.
    [UI]
        Animations & Transitions - Digunakan untuk menerapkan animasi pada transisi antar layar.
        Fragment - Digunakan sebagai komponen UI yang dapat digunakan kembali.
        Layout - Widget digunakan untuk merancang antarmuka pengguna.
    [Third Party]
        Glide - Digunakan untuk operasi pemuatan gambar.
        Kotlin Coroutines - Digunakan untuk operasi asinkron.
        Dagger-Hilt - Untuk melakukan Dependency Injection.
        SharedPreferences - Digunakan untuk menyimpan data kecil.
        Barcode Scanner - Digunakan untuk memindai barcode.

Pengaturan

Pastikan Anda telah menginstal prasyarat berikut:

    Java 17
    Android Studio
    Ponsel Android 7.0+ atau pengaturan Emulasi


bash

git clone [https://github.com/bbrsoft/PosV](https://github.com/bbrsoft/POsV.git)

Gunakan salah satu build Android Studio untuk menginstal dan menjalankan aplikasi di perangkat Anda atau simulator.
Screenshot

Halaman Login | Halaman Kategori | Halaman Produk
Halaman Keranjang Belanja | Halaman Kasir | Laporan Harian
Video Demo (Versi Lama)

Contoh Struk
Penulis

    Hasan Ali Çalışkan GitHub
    Çağrı Asan GitHub

Lisensi

Proyek ini dilisensikan di bawah MIT License. Untuk informasi lebih lanjut, silakan lihat berkas LICENSE.
Catatan Penting

    Aplikasi ini memerlukan pengguna untuk melakukan login awal di layar pertama. Informasi berikut diperlukan untuk proses ini:
        Nomor Identitas Terminal (Terminal ID)
        Nomor ID Turki atau Nomor Pajak (TCKN atau VKN)
        Nomor Identifikasi Merchant (Merchant ID)
        Kata Sandi

Biasanya, rincian ini disediakan oleh distributor untuk setiap merchant. Pada contoh aplikasi mobile ini, informasi yang diperlukan disimpan secara statis di file Constants.kt. Anda dapat memodifikasi rincian ini jika diperlukan. Untuk memasukkan informasi dengan mudah di layar, Anda dapat mengklik tombol radio "test".

    SDK untuk perangkat POS tidak disertakan dalam proyek ini karena masalah lisensi.
