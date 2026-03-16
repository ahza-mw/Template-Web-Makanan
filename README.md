# Template-Web-Makanan
Template web yang bisa diedit
Jika bingung maka copas dibawah ini ke Chatgpt

Berikut panduan lengkap semua bagian yang bisa diedit di file template-toko.html:

1. Identitas Toko
Cari bagian ini di file:
jsnama_toko:    "DAPUR KITA",
tagline:      "Masakan Rumahan, Cita Rasa Bintang Lima",
deskripsi:    "Kami menyajikan masakan rumahan...",
logo_emoji:   "🍳",
Ganti teks di antara tanda kutip "..." sesuai nama dan info toko kamu.

2. Kontak
jsalamat:   "Jl. Mawar No. 12, Purwakarta, Jabar",
telepon:  "0812-9999-0000",
email:    "halo@dapurkita.id",
jam_buka: "Senin–Sabtu, 08.00–20.00 WIB",
whatsapp: "6281299990000",
Nomor whatsapp harus format internasional tanpa +, contoh: 628123456789. Ini yang dipakai tombol pesan via WA.

3. Warna Tema
jswarna: {
  utama:      "#1A1A2E",   // navbar, footer, tombol utama
  aksen:      "#E94560",   // badge, harga, tombol CTA
  aksen_muda: "#FFEEF1",   // background muda aksen
  bg:         "#F8F7F4",   // background halaman
  kartu:      "#FFFFFF",   // background kartu produk
  teks:       "#1A1A2E",   // teks utama
  teks_redup: "#7A7A8C",   // teks deskripsi/sekunder
},
Cara ganti warna: buka g.co/colorpicker di Google, pilih warna, copy kode Hex (#xxxxxx), paste di sini.

4. Hero (Bagian Atas Halaman)
jshero: {
  judul_baris1: "Masakan",
  judul_baris2: "Rumahan",
  judul_aksen:  "Terbaik",    // kata yang diwarnai aksen
  teks_cta:     "Pesan Sekarang",
  teks_cta2:    "Lihat Menu",
  gambar_hero:  "🍲",         // emoji besar di hero
  stats: [
    { angka: "150+", label: "Menu Tersedia" },
    { angka: "4.8★", label: "Rating" },
    { angka: "500+", label: "Pelanggan" },
  ],
},

5. Kategori
jskategori: [
  { ikon: "🍚", nama: "Makanan Berat", jumlah: "32 menu" },
  { ikon: "🥘", nama: "Lauk Pauk",     jumlah: "45 menu" },
  ...
],
Untuk tambah kategori, copy satu baris { ikon: ..., nama: ..., jumlah: ... }, dan paste di bawahnya. Untuk hapus, hapus satu baris beserta komanya.

6. Produk
jsproduk: [
  {
    ikon:        "🍲",
    kategori:    "Makanan Berat",
    nama:        "Soto Ayam Kampung",
    deskripsi:   "Soto bening dengan ayam kampung segar...",
    harga:       28000,           // angka, tanpa titik/koma/Rp
    harga_coret: 35000,           // harga asli, isi null jika tidak ada
    badge:       "Terlaris",      // isi null jika tidak pakai badge
    badge_tipe:  "hits",          // hits / baru / promo / null
  },
],
Untuk tambah produk baru, copy satu blok { ... }, dari produk yang sudah ada, paste setelahnya, lalu ubah isinya.

7. Banner Promo
jspromo: {
  judul:      "Gratis Ongkir Setiap Hari",
  sub:        "Minimal order Rp 50.000 · Radius 5 km",
  kode:       "GRATISONGKIR",
  keterangan: "Berlaku setiap hari tanpa batas",
  aktif:      true,    // ganti false untuk sembunyikan banner
},
Cukup ganti aktif: true jadi aktif: false untuk menyembunyikan banner tanpa menghapus datanya.

8. Ulasan Pelanggan
jsulasan: [
  {
    nama:    "Budi Hartono",
    kota:    "Purwakarta",
    inisial: "B",       // 1–2 huruf untuk foto avatar bulat
    bintang: 5,         // angka 1–5
    teks:    "Soto ayam kampungnya beda banget...",
  },
],

9. Metode Pembayaran
jsmetode_bayar: ["GoPay", "OVO", "DANA", "BRI", "BCA", "COD"],
Tambah atau hapus nama metode pembayaran sesuai yang tersedia di toko kamu.

10. Sosial Media
jssosmed: {
  instagram: "https://instagram.com/namaakunmu",
  whatsapp:  "",    // kosong = otomatis pakai nomor di atas
  tiktok:    "https://tiktok.com/@namaakunmu",
  facebook:  "",    // kosong = tombol tidak muncul
},
Kosongkan "" untuk menyembunyikan tombol sosmed yang tidak dipakai.

Tips umum:

Teks selalu di antara tanda kutip "..."
Angka (harga, bintang) ditulis langsung tanpa kutip
true / false tanpa kutip
Setelah edit, simpan file lalu refresh browser
Kalau ada error, cek apakah ada tanda kutip atau koma yang terhapus tidak sengaja
