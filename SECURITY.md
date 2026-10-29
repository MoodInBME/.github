# Kebijakan Keamanan — MoodInBME

Berkas ini berlaku untuk semua repo di organisasi MoodInBME yang tidak punya `SECURITY.md` sendiri.

## Ruang lingkup

MoodIn adalah prototipe riset tahap Proposal Tugas Akhir (Pra-TA). Proyek ini bukan layanan produksi dan bukan alat medis. Laporan yang paling relevan:

- kredensial yang bocor (token, kata sandi, kunci API), baik di berkas maupun di riwayat git;
- data pribadi, citra wajah, atau data partisipan penelitian yang ikut ter-commit atau terpapar;
- isi dataset berlisensi yang ikut ter-commit;
- celah pada komunikasi antarperangkat (MQTT di jaringan lokal).

## Cara melapor

**Jangan membuka _issue_ publik** untuk hal di atas, karena isinya langsung terlihat oleh siapa pun.

1. Buka tab **Security** pada repo yang bersangkutan, lalu pilih **Report a vulnerability**. Laporan ini hanya terlihat oleh pengelola repo dan pelapor.
2. Sebutkan repo, path berkas, dan SHA commit. **Jangan menyalin ulang** kredensial atau data pribadinya ke dalam laporan.

Bila tombol **Report a vulnerability** tidak muncul, buka _issue_ yang hanya berisi permintaan kontak untuk laporan keamanan, tanpa rincian apa pun.

## Tindak lanjut

- Kredensial yang bocor **dicabut atau diganti lebih dulu**. Hanya cara ini yang menjamin kredensial tidak bisa dipakai, karena menghapus berkas tidak menghapus riwayat git.
- Data pribadi, citra wajah, dan data partisipan tidak bisa dicabut seperti kredensial. Berkasnya dihapus, riwayat git ditulis ulang bila perlu, dan GitHub Support dihubungi untuk menghapus salinan yang masih tersimpan.
- Paparan data partisipan penelitian juga dilaporkan dan ditangani sesuai protokol yang disetujui Komite Etik Penelitian (KEP) ITS.
- Berkas yang bermasalah dihapus dari branch `main`.
- Penulisan ulang riwayat git dipertimbangkan per kasus, karena branch `main` dilindungi dari _force push_.
