<div align="center">

# MoodIn

**Tugas Akhir · Departemen Teknik Biomedik · Institut Teknologi Sepuluh Nopember**

Sistem cermin berbasis kamera untuk memperkirakan tingkat stres dan kategori _mood_ penggunanya tanpa kontak.

![Tahap](https://img.shields.io/badge/tahap-preliminary%20research-yellow)
![Riwayat](https://img.shields.io/badge/riwayat-GEMASTIK%20XIX%202026-lightgrey)

</div>

---

## Tentang

MoodIn adalah proyek Tugas Akhir (TA) individual. Kamera di balik cermin dua arah merekam wajah pengguna, lalu sistem memperkirakan dua hal:

- **tingkat stres**, dari sinyal denyut yang diekstraksi dari video wajah (_remote photoplethysmography_, rPPG) dan variabilitas denyut jantung (HRV);
- **kategori _mood_**, dari gerak _landmark_ wajah.

Pemrosesan berjalan di perangkat (NVIDIA Jetson Orin Nano Super). Citra wajah tidak disimpan dan tidak dikirim ke luar perangkat. MoodIn adalah prototipe riset, **bukan alat diagnosis medis**.

Rancangan rinci (arsitektur, parameter, dan protokol pengambilan data) ada di proposal TA dan belum dipublikasikan.

## Repositori

| Repo                                                                        | Isi                                                                                                      | Status                             |
| --------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- | ---------------------------------- |
| [MoodIn-master](https://github.com/MoodInBME/MoodIn-master)                 | Dokumen proyek: peta repo, ADR, roadmap, kontrak antar-repo, arsip GEMASTIK                              | Aktif, dokumen saja                |
| [Software-Architecture](https://github.com/MoodInBME/Software-Architecture) | Pemrosesan sinyal dan model: jalur fisiologis (rPPG → HRV → stres) dan jalur wajah (_landmark_ → _mood_) | Aktif, jalur fisiologis lebih dulu |
| [Hardware-Connections](https://github.com/MoodInBME/Hardware-Connections)   | Perangkat keras, serta integrasi dan _deployment_ di Jetson                                              | Aktif, menunggu keputusan desain   |
| [Interface-App](https://github.com/MoodInBME/Interface-App)                 | Aplikasi Flutter: tampilan cermin dan aplikasi pendamping Android                                        | Persiapan                          |
| [Interface-Display](https://github.com/MoodInBME/Interface-Display)         | UI era GEMASTIK (PySide6 + QML, kiosk web)                                                               | Arsip, _read-only_                 |

## Teknologi

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-deep%20learning-EE4C2C?logo=pytorch&logoColor=white)
![Jetson Orin Nano Super](https://img.shields.io/badge/NVIDIA%20Jetson-Orin%20Nano%20Super-76B900?logo=nvidia&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-UI-02569B?logo=flutter&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-jaringan%20lokal-660066?logo=mqtt&logoColor=white)

## Penulis dan pembimbing

- **Penulis TA:** Jeremia Christ Immanuel Manalu
- **Pembimbing 1:** Nada Fitrieyatul Hikmah, S.T., M.T.
- **Pembimbing 2:** Nabila Puspita Firdi, S.T., M.Si.

## Riwayat: GEMASTIK XIX 2026

MoodIn berawal dari proyek tim **VisionaryX** pada GEMASTIK XIX 2026, Divisi 9 (Piranti Cerdas, Sistem Benam, dan IoT), dengan pembimbing Nada Fitrieyatul Hikmah, S.T., M.T. Anggota tim:

- Jeremia Christ Immanuel Manalu (ketua)
- Tanuhita Setya Dhanurendra
- Sitti Nurhalimah
- Nozomi Crystalle Padilla Malle (anggota sebelum digantikan oleh Sitti Nurhalimah)

Akhir era GEMASTIK ditandai tag `gemastik-xix-2026` di setiap repo, misalnya [MoodIn-master pada tag itu](https://github.com/MoodInBME/MoodIn-master/tree/gemastik-xix-2026). Commit sesudah tag adalah pekerjaan TA.

<div align="center">

Departemen Teknik Biomedik · Institut Teknologi Sepuluh Nopember · Surabaya, Indonesia

</div>
