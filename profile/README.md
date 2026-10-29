<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/hero-dark.png">
  <img alt="MoodIn, cermin pintar untuk mengenali suasana hati dan tingkat stres. Proposal Tugas Akhir (Pra-TA), dalam pengembangan." src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/hero-light.png" width="100%">
</picture>

<p>
  <a href="#tentang-moodin">Tentang</a> ·
  <a href="#yang-dikenali-moodin">Keluaran</a> ·
  <a href="#alur-pemeriksaan">Alur</a> ·
  <a href="#prinsip">Prinsip</a> ·
  <a href="#repositori">Repositori</a> ·
  <a href="#tim">Tim</a>
</p>

</div>

## Tentang MoodIn

MoodIn adalah cermin pintar untuk _check-in_ singkat terhadap kondisi emosional. Pengguna cukup duduk di depan cermin selama beberapa saat. Kamera yang tersembunyi di balik cermin dua arah membaca isyarat dari wajah tanpa sensor yang menempel di tubuh, lalu cermin menampilkan perkiraan **kategori suasana hati** (_mood_) dan **tingkat stres**. Riwayat pemeriksaan dapat dilihat kembali melalui aplikasi pendamping di ponsel.

Organisasi ini menampung seluruh kode dan dokumen MoodIn. Saat ini MoodIn dikembangkan sebagai **Proposal Tugas Akhir (Pra-TA)** di Departemen Teknik Biomedik, Fakultas Teknologi Elektro dan Informatika Cerdas (FTEIC), Institut Teknologi Sepuluh Nopember. Proposal masih direvisi bersama calon dosen pembimbing, sehingga rancangan dan isi repositori dapat berubah.

> [!IMPORTANT]
> MoodIn adalah prototipe riset untuk refleksi diri, **bukan alat diagnosis medis**. Hasilnya tidak menggantikan penilaian psikolog, psikiater, atau tenaga kesehatan lain.

### Mengapa cermin?

<img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/mengapa.png" width="44" align="right" alt="">

Masalah kesehatan mental banyak dialami anak muda di Indonesia. Survei kesehatan mental remaja nasional (I-NAMHS) mencatat bahwa satu dari tiga remaja (34,9%) menunjukkan gejala masalah kesehatan mental dalam 12 bulan terakhir, dan 5,5% mengalami gangguan mental. Perubahan suasana hati dan stres sering tidak disadari sejak awal, padahal pemantauan rutin membantu seseorang mengenali polanya lebih dini.

<sub>Sumber: A. E. Wahdi, S. A. Wilopo, dan H. E. Erskine, "The Prevalence of Adolescent Mental Disorders in Indonesia: An Analysis of Indonesia–National Mental Health Survey (I-NAMHS)," <i>Journal of Adolescent Health</i>, 2023 (<a href="https://beph.fkkmk.ugm.ac.id/publikasi/the-prevalence-of-adolescent-mental-disorders-in-indonesia-an-analysis-of-indonesia-national-mental-health-survey-i-namhs/">ringkasan di BEPH FK-KMK UGM</a>).</sub>

Cara pemantauan yang umum punya kendala. Kuesioner bergantung pada laporan diri, sedangkan sensor yang menempel di tubuh terasa merepotkan bila dipakai setiap hari. Cermin sudah menjadi bagian dari rutinitas harian, sehingga MoodIn memanfaatkan momen bercermin untuk pemeriksaan singkat yang tidak mengganggu.

## Yang dikenali MoodIn

<table>
  <tr>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/mood.png" width="44" alt=""><br>
      <b>Kategori suasana hati</b><br>
      Lima kategori yang mudah dipahami: Ceria, Rileks, Netral, Cemas, dan Tertekan. Kategori diperkirakan dari gerak dan ekspresi wajah selama pemeriksaan.
    </td>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/stres.png" width="44" alt=""><br>
      <b>Tingkat stres</b><br>
      Diperkirakan dari sinyal denyut jantung yang terbaca dari video wajah (<i>remote photoplethysmography</i>, rPPG) dan variabilitas denyut jantung (HRV). Pembagian tingkat stres masih dibahas dalam bimbingan.
    </td>
  </tr>
</table>

<table align="center">
  <tr>
    <td align="center" width="20%"><img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/mood/mood-ceria.png" width="56" alt=""><br><b>Ceria</b></td>
    <td align="center" width="20%"><img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/mood/mood-rileks.png" width="56" alt=""><br><b>Rileks</b></td>
    <td align="center" width="20%"><img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/mood/mood-netral.png" width="56" alt=""><br><b>Netral</b></td>
    <td align="center" width="20%"><img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/mood/mood-cemas.png" width="56" alt=""><br><b>Cemas</b></td>
    <td align="center" width="20%"><img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/mood/mood-tertekan.png" width="56" alt=""><br><b>Tertekan</b></td>
  </tr>
</table>

## Alur pemeriksaan

Satu sesi dirancang singkat dan berurutan, dari menyapa pengguna sampai menyimpan riwayat. Alur ini mengikuti desain antarmuka era GEMASTIK dan masih dapat berubah selama Pra-TA.

<table>
  <tr>
    <td align="center" valign="top" width="20%">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/alur-duduk.png" width="48" alt=""><br>
      <sub>LANGKAH 1</sub><br>
      <b>Duduk di depan cermin</b><br>
      <sub>Cermin menyala dan menyapa pengguna.</sub>
    </td>
    <td align="center" valign="top" width="20%">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/alur-profil.png" width="48" alt=""><br>
      <sub>LANGKAH 2</sub><br>
      <b>Pilih profil</b><br>
      <sub>Masuk sebagai pengguna terdaftar atau sebagai tamu.</sub>
    </td>
    <td align="center" valign="top" width="20%">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/alur-ukur.png" width="48" alt=""><br>
      <sub>LANGKAH 3</sub><br>
      <b>Pengukuran singkat</b><br>
      <sub>Setelah pengguna setuju, cukup diam dan rileks sebentar.</sub>
    </td>
    <td align="center" valign="top" width="20%">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/alur-hasil.png" width="48" alt=""><br>
      <sub>LANGKAH 4</sub><br>
      <b>Hasil di cermin</b><br>
      <sub>Suasana hati dan tingkat stres tampil di cermin.</sub>
    </td>
    <td align="center" valign="top" width="20%">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/alur-riwayat.png" width="48" alt=""><br>
      <sub>LANGKAH 5</sub><br>
      <b>Riwayat di aplikasi</b><br>
      <sub>Tren harian dan mingguan di aplikasi pendamping.</sub>
    </td>
  </tr>
</table>

## Prinsip

Karena menyangkut wajah dan kondisi emosional seseorang, MoodIn dibangun dengan beberapa batasan. Batasan di bawah berlaku untuk cara kerja cermin dan untuk isi semua repositori di organisasi ini.

<table>
  <tr>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/prinsip-lokal.png" width="40" alt=""><br>
      <b>Diproses di dalam cermin</b><br>
      Video wajah diolah langsung oleh komputer <i>edge</i> (NVIDIA Jetson Orin Nano Super) di dalam cermin dan tidak dikirim ke luar perangkat.
    </td>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/prinsip-tanpa-citra.png" width="40" alt=""><br>
      <b>Citra wajah tidak disimpan</b><br>
      Video hanya diproses sesaat. Antarmodul hanya bertukar angka hasil, bukan gambar.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/prinsip-persetujuan.png" width="40" alt=""><br>
      <b>Atas persetujuan pengguna</b><br>
      Pengukuran baru dimulai setelah pengguna menyatakan setuju. Pemeriksaan bersifat sukarela, bukan pemantauan diam-diam.
    </td>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/prinsip-bukan-diagnosis.png" width="40" alt=""><br>
      <b>Bukan alat diagnosis</b><br>
      Hasil bersifat informatif untuk refleksi diri. Tampilan dalam mode demo atau simulasi selalu diberi penanda.
    </td>
  </tr>
</table>

Pengambilan data penelitian dengan partisipan (data primer) diatur terpisah oleh protokol yang harus disetujui Komite Etik Penelitian (KEP) ITS lebih dulu, termasuk apa yang direkam, bagaimana data disimpan, dan kapan data dihapus. Data partisipan tidak pernah disimpan di repositori. Rinciannya ada di halaman [Etika penelitian dan pengelolaan data](https://github.com/MoodInBME/MoodIn-master/blob/main/docs/etika-dan-data.md).

## Repositori

Kode dan dokumen MoodIn dipisah per lapisan sistem. Antar-repositori tidak saling memanggil kode secara langsung: modul berkomunikasi lewat pesan MQTT di jaringan lokal, dengan format pesan yang disepakati di MoodIn-master.

<table>
  <tr>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/repo-master.png" width="40" alt=""><br>
      <a href="https://github.com/MoodInBME/MoodIn-master"><b>MoodIn-master</b></a><br>
      <sub>DOKUMEN · AKTIF</sub><br>
      Titik awal untuk memahami proyek: gambaran sistem, peta repositori, catatan keputusan (ADR), roadmap, kontrak pesan antar-repo, dan arsip GEMASTIK.
    </td>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/repo-software.png" width="40" alt=""><br>
      <a href="https://github.com/MoodInBME/Software-Architecture"><b>Software-Architecture</b></a><br>
      <sub>PYTHON · AKTIF (M1)</sub><br>
      Pemrosesan sinyal dan model: jalur fisiologis untuk tingkat stres dan jalur wajah untuk suasana hati, termasuk pelatihan dan evaluasinya.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/repo-hardware.png" width="40" alt=""><br>
      <a href="https://github.com/MoodInBME/Hardware-Connections"><b>Hardware-Connections</b></a><br>
      <sub>PERANGKAT KERAS · AKTIF (M2)</sub><br>
      Kamera di balik cermin, Jetson, layar, pencahayaan, dan casing, serta integrasi dan <i>deployment</i> sistem di Jetson.
    </td>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/repo-app.png" width="40" alt=""><br>
      <a href="https://github.com/MoodInBME/Interface-App"><b>Interface-App</b></a><br>
      <sub>FLUTTER · PERSIAPAN (M3)</sub><br>
      Tampilan di balik cermin dan aplikasi pendamping Android dalam satu basis kode Flutter.
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/repo-display.png" width="40" alt=""><br>
      <a href="https://github.com/MoodInBME/Interface-Display"><b>Interface-Display</b></a><br>
      <sub>ARSIP · READ-ONLY</sub><br>
      Antarmuka era GEMASTIK (PySide6 + QML dan kiosk web). Disimpan sebagai rujukan; tidak dikembangkan lagi.
    </td>
    <td width="50%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/repo-github.png" width="40" alt=""><br>
      <a href="https://github.com/MoodInBME/.github"><b>.github</b></a><br>
      <sub>BERKAS KOMUNITAS · AKTIF</sub><br>
      Profil organisasi ini serta panduan kontribusi, kebijakan keamanan, dan templat <i>issue</i> yang berlaku untuk semua repositori.
    </td>
  </tr>
</table>

<p>
  <img alt="Python 3.12" src="https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white">
  <img alt="PyTorch" src="https://img.shields.io/badge/PyTorch-deep%20learning-EE4C2C?style=flat-square&logo=pytorch&logoColor=white">
  <img alt="NVIDIA Jetson Orin Nano Super" src="https://img.shields.io/badge/NVIDIA%20Jetson-Orin%20Nano%20Super-76B900?style=flat-square&logo=nvidia&logoColor=white">
  <img alt="Flutter" src="https://img.shields.io/badge/Flutter-UI-02569B?style=flat-square&logo=flutter&logoColor=white">
  <img alt="MQTT di jaringan lokal" src="https://img.shields.io/badge/MQTT-jaringan%20lokal-660066?style=flat-square&logo=mqtt&logoColor=white">
</p>

## Status

<img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/status.png" width="44" align="right" alt="">

Tahap sekarang adalah penyusunan dan revisi Proposal Tugas Akhir (Pra-TA). Di sisi repositori, arsip GEMASTIK, tata kelola, dan dokumentasi sedang dirapikan (milestone M0). Pekerjaan teknis berikutnya dimulai dari jalur fisiologis pada dataset publik (M1). Rincian metode, parameter, dan rancangan pengujian ada di dokumen proposal dan **belum dipublikasikan**. Pengambilan data primer belum dimulai; protokolnya sedang disiapkan untuk diajukan ke KEP ITS.

Roadmap lengkap ada di [MoodIn-master/docs/roadmap.md](https://github.com/MoodInBME/MoodIn-master/blob/main/docs/roadmap.md).

## Tim

<table>
  <tr>
    <td align="center" width="33%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/tim.png" width="40" alt=""><br>
      <b>Jeremia Christ Immanuel Manalu</b><br>
      <sub>Mahasiswa pengusul Pra-TA</sub>
    </td>
    <td align="center" width="33%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/tim.png" width="40" alt=""><br>
      <b>Nada Fitrieyatul Hikmah, S.T., M.T.</b><br>
      <sub>Calon Dosen Pembimbing 1</sub>
    </td>
    <td align="center" width="33%" valign="top">
      <img src="https://raw.githubusercontent.com/MoodInBME/.github/main/profile/assets/ikon/tim.png" width="40" alt=""><br>
      <b>Nabila Puspita Firdi, S.T., M.Sc.</b><br>
      <sub>Calon Dosen Pembimbing 2</sub>
    </td>
  </tr>
</table>

Dosen pembimbing Tugas Akhir belum ditetapkan secara resmi. Selama tahap Pra-TA, kedua dosen di atas berstatus calon dosen pembimbing.

<details>
<summary><b>Riwayat: berawal dari GEMASTIK XIX 2026</b></summary>
<br>

MoodIn lahir sebagai proyek tim **VisionaryX** untuk GEMASTIK XIX 2026, Divisi 9 (Piranti Cerdas, Sistem Benam, dan IoT), dengan dosen pembimbing tim Nada Fitrieyatul Hikmah, S.T., M.T. Pada era itu, tim membangun purwarupa cermin, model awal, dan antarmuka PySide6 + QML. Anggota tim:

- Jeremia Christ Immanuel Manalu (ketua)
- Tanuhita Setya Dhanurendra
- Sitti Nurhalimah
- Nozomi Crystalle Padilla Malle (anggota sebelum digantikan oleh Sitti Nurhalimah)

Isi era GEMASTIK dibekukan dengan tag `gemastik-xix-2026` di setiap repositori, misalnya [MoodIn-master pada tag tersebut](https://github.com/MoodInBME/MoodIn-master/tree/gemastik-xix-2026). Commit sesudah tag merupakan pekerjaan tahap Pra-TA. Logo, maskot, dan ikon suasana hati di halaman ini juga berasal dari desain tim era GEMASTIK.

</details>

---

<div align="center">
<sub>
Departemen Teknik Biomedik · Fakultas Teknologi Elektro dan Informatika Cerdas (FTEIC)<br>
Institut Teknologi Sepuluh Nopember · Surabaya, Indonesia
</sub>
<br><br>
<sub>Ikon antarmuka: <a href="https://tabler.io/icons">Tabler Icons</a> (MIT). Logo, maskot, dan ikon suasana hati: desain tim MoodIn.</sub>
</div>
