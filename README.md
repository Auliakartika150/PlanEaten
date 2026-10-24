# 🥗 PlanEaten - Platform Pemesanan dan Perencanaan Catering Mingguan

**PlanEaten** adalah aplikasi berbasis web yang dirancang untuk menjawab tantangan manajemen pemesanan usaha catering dan mempermudah pelanggan dalam merencanakan pola makan harian secara fleksibel, sehat, dan terstruktur selama seminggu penuh. 
---
## Latar Belakang & Permasalahan
Berdasarkan laporan INDEF, terdapat kesenjangan digital di mana **lebih dari 80% pelaku usaha catering (terutama UMKM) masih mengandalkan sistem manual** atau platform non-spesifik. Hal ini memicu beberapa kendala utama:
1. **Sisi Pengusaha:** Risiko kesalahan pencatatan pesanan harian/mingguan tinggi, serta kesulitan melacak rekapan pesanan konsumen secara *real-time*.
2. **Sisi Pelanggan:** Terbatasnya visualisasi menu yang jelas dan kerepotan mengatur jadwal makan sehat yang bervariasi secara praktis di tengah rutinitas yang padat.

**PlanEaten** hadir sebagai solusi digital terintegrasi untuk menjembatani kebutuhan pemilik bisnis catering (pengelolaan pesanan efisien) dan kebutuhan konsumen (perencanaan menu gizi harian yang terstruktur).

---

## Fitur Utama Aplikasi Web
Aplikasi dijalankan pada lingkungan lokal (`http://localhost:5173/`) dengan fitur-fitur utama sebagai berikut:

1. **Autentikasi Pengguna (`/register` & `/login`):** Fasilitas pendaftaran akun baru bagi pengguna dan pengamanan hak akses data pribadi serta riwayat pemesanan.
2. **Daftar Menu Informatif (`/dashboard#menu`):** Menampilkan katalog variasi makanan mingguan lengkap beserta foto produk, harga, dan rating gizi.
3. **Tambah Menu Fleksibel (`/dashboard`):** Memungkinkan konsumen memasukkan menu pilihan ke keranjang secara mandiri dan menentukan hari pemesanan spesifik (Senin–Sabtu).
4. **Kelola Keranjang Kontrol Penuh (`/dashboard`):** Pengguna dapat memantau akumulasi harga total, menambah/mengurangi kuantitas porsi, atau menghapus item sebelum finalisasi.
5. **Simpan & Rekap Jadwal (`/dashboard/schedule`):** Menyimpan rekapitulasi rencana pola makan mingguan terstruktur sebagai referensi tanpa perlu memilih ulang dari awal.

---

## Struktur Database & Arsitektur Sistem
Sistem ini didukung oleh database relasional (`caneaten`) dengan entitas utama:
* **`users`:** Menyimpan kredensial akun dan data autentikasi pengguna.
* **`menu`:** Menyimpan daftar jenis masakan, harga, aset gambar, dan rating performa menu.
* **`keranjangs`:** Menyimpan antrean pesanan aktif, jumlah kuantitas, serta penugasan hari pengiriman terkait.

---
## Kesimpulan & Pengembangan ke Depan
* **Kesimpulan:** PlanEaten berhasil mendigitalkan sistem manajemen catering tradisional menjadi platform pemesanan berbasis jadwal (*schedule-based parsing*) yang mengurangi kesalahan operasional hingga mempermudah kontrol gizi personal.
* **Saran Pengembangan:** Untuk meningkatkan efisiensi transaksi, disarankan melakukan integrasi *Payment Gateway* otomatis (seperti Midtrans) agar proses rekapitulasi menu dan pembayaran akhir dapat berjalan *end-to-end* di dalam satu platform tunggal.
