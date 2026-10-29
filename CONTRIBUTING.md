# Panduan Kontribusi — MoodInBME

Berkas ini berlaku untuk semua repo di organisasi MoodInBME yang tidak punya `CONTRIBUTING.md` sendiri.

## Status proyek

MoodIn dikembangkan sebagai **Proposal Tugas Akhir (Pra-TA) individual** oleh Jeremia Christ Immanuel Manalu (Departemen Teknik Biomedik, Fakultas Teknologi Elektro dan Informatika Cerdas, Institut Teknologi Sepuluh Nopember). Karena itu:

- **Hanya Jeremia yang membuat commit dan push.** Anggota tim GEMASTIK dan calon dosen pembimbing punya akses baca.
- **_Pull request_ dari luar tidak diterima.** Hasil Pra-TA dan Tugas Akhir harus dapat dipertanggungjawabkan sebagai karya penulisnya.
- **_Issue_ boleh dibuka** untuk melaporkan error, tautan mati, atau pertanyaan. Gunakan templat yang tersedia.
- Masalah keamanan atau data pribadi dilaporkan sesuai [SECURITY.md](SECURITY.md), **bukan** lewat _issue_ publik.

## Aturan kerja penulis

### Branch dan tag

- Branch default setiap repo adalah `main`. Ruleset GitHub membuat branch ini tidak bisa dihapus dan tidak menerima _force push_.
- Tag `gemastik-*` menandai arsip era GEMASTIK dan tidak bisa dihapus atau dipindah.
- Paling banyak **satu branch kerja aktif per repo**, dengan awalan `feat/`, `fix/`, `docs/`, atau `exp/`. Hapus branch itu, lokal dan remote, setelah di-merge.

### Pesan commit

Format [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) dalam bahasa Indonesia:

```text
<tipe>(<cakupan, opsional>): <ringkasan singkat, huruf kecil, tanpa titik>
```

- Tipe yang dipakai: `feat`, `fix`, `docs`, `test`, `refactor`, `perf`, `chore`, `ci`.
- **Tanpa baris `Co-authored-by:`** dan tanpa atribusi alat AI. _Pre-push hook_ di mesin penulis menolak commit seperti itu.

### Perubahan lintas repo

Perubahan yang memengaruhi repo lain, misalnya kontrak pesan MQTT, nama topik, struktur folder yang dirujuk, atau skrip yang dipindah:

1. Kontrak pesan antar-repo diubah lebih dulu di MoodIn-master, baru implementasinya.
2. Perubahan dicatat di `CHANGELOG.md` **setiap** repo yang terdampak, dengan penanda **[lintas repo]**.
3. Penulis juga mencatatnya di log internal (kode `ISU-###` untuk masalah dan `CHG-###` untuk perubahan).

### Yang tidak boleh masuk repo

- Berkas dataset dan turunannya: video, sinyal, _landmark_, anotasi, fitur, dan _cache_ tensor. Pemakaian dataset terikat perjanjian lisensi (EULA).
- Citra atau video wajah siapa pun.
- Token, kata sandi, kunci API, dan berkas kredensial seperti `kaggle.json` atau `.env`.
- Data pribadi: NRP, nomor identitas, foto KTP/KTM, nomor telepon, dan email pribadi di dalam dokumen.
- Bobot model berukuran besar. Simpan di luar git dan tuliskan cara mendapatkannya di README.

Bila terlanjur masuk, cabut atau ganti kredensialnya lebih dulu, lalu tangani sesuai [SECURITY.md](SECURITY.md). Menghapus berkas dari commit terbaru tidak menghapusnya dari riwayat git.

### Standar teknis

- Kode Python memakai Python 3.12.
- Kode Flutter mengikuti versi yang dikunci di repo Interface-App.
- Pengujian dan pemeriksaan gaya kode mengikuti ketentuan di README repo masing-masing.

## Lisensi

Setiap repo mengikuti berkas `LICENSE` miliknya. Repo tanpa berkas `LICENSE` belum dilisensikan untuk dipakai ulang; lisensinya menunggu keputusan bersama calon dosen pembimbing.
