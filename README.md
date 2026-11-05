# Mari Jua Jastip - Dashboard Pesanan & Invoice

Situs statis satu halaman (HTML + JavaScript), tanpa build dan tanpa server.

## Deploy ke Netlify
1. Buka https://app.netlify.com/drop
2. Seret folder hasil ekstrak zip ini (atau file zip-nya) ke halaman tersebut.
3. Selesai. Netlify memberi alamat seperti `nama-acak.netlify.app`. Nama situs bisa diganti di Site configuration.

Lewat Git: taruh isi folder ini di repo, lalu di Netlify pilih "Import from Git" dengan Build command kosong dan Publish directory `.`.

## Catatan penting
- Data pesanan disimpan di browser perangkat yang dipakai (localStorage). Browser lain atau perangkat lain tidak melihat data yang sama.
- Rutin unduh cadangan di menu Pengaturan > Cadangan data. File .json itu bisa dipulihkan di perangkat lain.
- Halaman Semua pesanan dan halaman nota punya tombol "Ekspor ke Excel" (file .xlsx berisi sheet Pesanan dan Rincian Barang). Fitur ini memuat library dari internet (cdnjs), jadi perlu koneksi.
- Jangan hapus data situs/cookie browser tanpa cadangan, karena data pesanan ikut terhapus.
- Pasang proteksi kata sandi di Netlify (Site configuration > Access) bila alamat situs tidak ingin dibuka orang lain. Data pelanggan tidak ada di server, tetapi halamannya bisa dibuka siapa saja yang punya alamat.

## Isi
- index.html : seluruh aplikasi (logo sudah tertanam)
- favicon.png : ikon tab browser
- netlify.toml : pengaturan Netlify
