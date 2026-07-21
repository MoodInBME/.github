<!-- Profil publik organisasi: MoodInBME. File ini WAJIB berada di path .github/profile/README.md -->

<div align="center">

# MoodIn · Tim VisionaryX

### Smart Mirror untuk Klasifikasi Mood berbasis Graph Convolutional Network & remote Photoplethysmography

*Personal Wellness Coach — memantau mood harian secara non-intrusive, tanpa kontak.*

![GEMASTIK](https://img.shields.io/badge/GEMASTIK%20XIX-Divisi%209%20·%20Piranti%20Cerdas%20%26%20IoT-red)
![Status](https://img.shields.io/badge/status-on--going-yellow)
![Institusi](https://img.shields.io/badge/Institut%20Teknologi%20Sepuluh%20Nopember-004b87)

</div>

---

## Tentang

**MoodIn** adalah cermin pintar (smart mirror) yang mengklasifikasikan mood pengguna secara real-time dengan menggabungkan dua sinyal tanpa kontak:

- **Ekspresi wajah** — diproses dengan Graph Convolutional Network (ST-GCN / Graph-Transformer) untuk mengestimasi **valence–arousal** ekspresi (pendekatan VA-bridge).
- **Sinyal fisiologis** — detak & variabilitas jantung (HR/HRV) diestimasi dari wajah lewat remote Photoplethysmography (rPPG).

Keduanya difusikan di ruang **valence–arousal** — valence diambil dari ekspresi wajah, arousal dari gabungan ekspresi & rPPG — lalu satu pemetaan kuadran mengklasifikasikannya ke **5 kelas**: Ceria, Cemas, Tertekan, Rileks, Netral — lengkap dengan tren mingguan dan micro-intervention sebagai wellness coach personal.

## Repositori

| Repo | Fungsi |
| --- | --- |
| [MoodIn-master](https://github.com/MoodInBME/MoodIn-master) | Hub proyek: dokumentasi, proposal, konvensi lintas-repo |
| [Hardware-Connections](https://github.com/MoodInBME/Hardware-Connections) | Wiring, enclosure, kamera, daya, protokol komunikasi |
| [Software-Architecture](https://github.com/MoodInBME/Software-Architecture) | Model deep learning, feature fusion, training, evaluasi |
| [Interface-Display](https://github.com/MoodInBME/Interface-Display) | Antarmuka kiosk (PySide6 + QML) pada perangkat |

> Tautan repo di atas hanya dapat diakses publik bila repo bersangkutan berstatus *public*. Repo yang masih *private* akan menampilkan 404 bagi pengunjung anonim.

## Teknologi

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-DL-EE4C2C?logo=pytorch&logoColor=white)
![Qt](https://img.shields.io/badge/PySide6%20%2B%20QML-UI-41CD52?logo=qt&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi%205-edge-A22846?logo=raspberrypi&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-TLS-660066?logo=mqtt&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-landmarks-0097A7)

## Tim VisionaryX

| Nama | Peran |
| --- | --- |
| Jeremia Christ Immanuel Manalu | Ketua |
| Tanuhita Setya Dhanurendra | Anggota |
| Nozomi Crystalle Padilla Malle | Anggota |

**Dosen Pembimbing:** Nada Fitrieyatul Hikmah, S.T., M.T.

## Dampak

Mendukung Sustainable Development Goals **SDG 3** (kesehatan & kesejahteraan), **SDG 4** (pendidikan berkualitas), dan **SDG 9** (industri, inovasi, infrastruktur).

<div align="center">

— Institut Teknologi Sepuluh Nopember · Surabaya, Indonesia —

</div>
