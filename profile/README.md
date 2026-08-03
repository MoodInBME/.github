<!-- Profil publik organisasi: MoodInBME. File ini WAJIB berada di path .github/profile/README.md -->

<div align="center">

# MoodIn · Tim VisionaryX

### Smart Mirror untuk Klasifikasi Mood Berbasis Graph Convolutional Network dan remote Photoplethysmography

*Personal Wellness Coach — memantau mood harian secara non-intrusive, tanpa kontak.*

![GEMASTIK](https://img.shields.io/badge/GEMASTIK%20XIX-Divisi%209%20·%20Piranti%20Cerdas%20%26%20IoT-red)
![Status](https://img.shields.io/badge/status-on--going-yellow)
![Institusi](https://img.shields.io/badge/Institut%20Teknologi%20Sepuluh%20Nopember-004b87)

</div>

---

## Tentang Kami

Kami sedang membangun sebuah cermin pintar (smart mirror) yang mampu mengenali kondisi afektif penggunanya secara **contactless**, dan memberikan intervensi mikro sebagai *personal wellness coach*.

Model kami mengekstrak dua kanal sensorik untuk mendapatkan satu keputusan:

| Kanal | Metode | Yang diukur |
|---|---|---|
| Biomekanik wajah | **ST-GCN + Graph Transformer** atas 68 landmark iBUG | Valence dan Arousal dari dinamika ekspresi |
| Fisiologis | **STC-rPPG** atas ROI dahi dan pipi | Denyut jantung, HRV, laju napas |

Kedua fitur tersebut digabung lewat *late fusion* pada bidang circumplex Russell, menghasilkan 5 kelas mood: **Ceria, Rileks, Cemas, Tertekan, Netral**.

Seluruh proses inferensi berjalan secara **real-time di perangkat edge** (NVIDIA Jetson Orin Nano Super, 8 GB). Citra wajah dan data biometrik mentah tidak pernah dikirimkan ke cloud (hanya nilai numerik saja), memastikan kepatuhan terhadap prinsip privasi dan perlindungan data (UU PDP No. 27/2022).

## Repositori

| Repo | Fungsi |
| --- | --- |
| [MoodIn-master](https://github.com/MoodInBME/MoodIn-master) | Hub proyek: dokumentasi, ADR, rencana integrasi lintas-repo |
| [Hardware-Connections](https://github.com/MoodInBME/Hardware-Connections) | Skema kabel, konfigurasi CSI kamera, daya, termal, dan perakitan |
| [Software-Architecture](https://github.com/MoodInBME/Software-Architecture) | Model ST-GCN dan STC-rPPG, pipeline data, fusi fitur, evaluasi |
| [Interface-Display](https://github.com/MoodInBME/Interface-Display) | Antarmuka UI cermin (PySide6 + QML) dan integrasi mock pub/sub |

> Tautan repo di atas hanya dapat diakses publik bila repo bersangkutan berstatus *public*. Repo yang masih *private* akan menampilkan 404 bagi pengunjung anonim.

## Teknologi

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-DL-EE4C2C?logo=pytorch&logoColor=white)
![Qt](https://img.shields.io/badge/PySide6%20%2B%20QML-UI-41CD52?logo=qt&logoColor=white)
![Jetson Orin Nano Super](https://img.shields.io/badge/NVIDIA%20Jetson%20Orin%20Nano-Super-76B900?logo=nvidia&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-TLS-660066?logo=mqtt&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-landmarks-0097A7)

## Tim VisionaryX

| Nama | Peran |
| --- | --- |
| Jeremia Christ Immanuel Manalu | Ketua, arsitektur perangkat lunak |
| Tanuhita Setya Dhanurendra | Anggota, model dan pemrosesan sinyal |
| Nozomi Crystalle Padilla Malle | Anggota, antarmuka dan integrasi |

**Dosen Pembimbing:** Nada Fitrieyatul Hikmah, S.T., M.T.

## Dampak

Mendukung Sustainable Development Goals **SDG 3** (Kesehatan yang Baik dan Kesejahteraan), **SDG 4** (Pendidikan Berkualitas), dan **SDG 9** (Industri, Inovasi, dan Infrastruktur).

<div align="center">

— Departemen Teknik Biomedik, Fakultas Teknologi Industri dan Rekayasa Sistem —
Institut Teknologi Sepuluh Nopember · Surabaya, Indonesia

</div>
