---
title: "Gambaran Fitur"
linkTitle: "Features overview"
second_title: "Referensi API GroupDocs.Redaction untuk Python via .NET"
description: "GroupDocs.Redaction untuk Python via .NET menghapus informasi sensitif dari dokumen melalui satu API yang independen format — teks, metadata, area gambar, anotasi, dan seluruh halaman — dan menyimpan hasilnya dalam format asli atau sebagai PDF yang disanitasi."
type: docs
url: /id/python-net/guides/features-overview/
is_root: false
weight: 30
---


GroupDocs.Redaction untuk Python via .NET menghapus atau secara permanen menyamarkan informasi sensitif di berbagai [supported document formats](). Setiap redaksi mengikuti alur kerja yang sama: buka dokumen dengan [`Redactor`](/redaction/python-net/groupdocs.redaction/redactor/), terapkan satu atau lebih redaksi dengan `apply()`, kemudian `save()` hasil yang telah dibersihkan baik dalam format aslinya maupun sebagai PDF yang disanitasi. Kemampuan di bawah ini dapat digabungkan secara bebas dalam satu proses.

## Text redaction

Temukan dan ganti teks dengan frasa tepat atau dengan ekspresi reguler, mencakup baik kata lengkap maupun pola kompleks seperti alamat e‑mail, nomor telepon, atau nomor KTP. Teks yang cocok dapat diganti dengan teks pengganti atau ditutupi oleh kotak berwarna sehingga konten asli tidak dapat dipulihkan. Di spreadsheet Anda dapat mempersempit pencarian ke satu lembar kerja atau kolom. Lihat [Text Redactions]().

## Metadata redaction

Hapus atau tulis ulang metadata dokumen — penulis, judul, perusahaan, komentar, dan data EXIF pada gambar — sehingga tidak ada detail sensitif yang bocor melalui properti dokumen. Anda dapat menghapus semua metadata, menargetkan bidang tertentu, atau mengganti nilai dengan yang baru. Lihat [Metadata Redactions]().

## Image-area redaction

Tutup area persegi panjang pada gambar tersemat atau halaman yang dipindai dengan menggambar kotak berisi di atas area tertentu — berguna untuk menyembunyikan tanda tangan, foto, header, atau footer di mana data rahasia diperkirakan muncul. Lihat [Image Redactions]().

## Annotation redaction

Tulis ulang atau hapus anotasi, komentar, dan catatan. Anda dapat menghapus semua anotasi atau menggunakan ekspresi reguler untuk mencocokkan hanya yang berisi teks sensitif. Lihat [Annotation Redactions]().

## Page removal

Hapus seluruh halaman dari dokumen PDF, slide dari presentasi, dan lembar kerja dari spreadsheet. Anda menentukan halaman mulai dan jumlah, bersama dengan arah relatif terhadap titik mulai. Lihat [Remove Page Redactions]().

## Rasterization to PDF

Simpan dokumen yang telah dibersihkan sebagai PDF yang halamannya dirender sebagai gambar raster. File yang dihasilkan tidak mengandung teks yang dapat dicari dan tidak ada metadata asli, sehingga konten yang dihapus tidak dapat dipulihkan. Rasterisasi adalah pilihan tepat ketika Anda harus menyerahkan dokumen ke pihak ketiga atau mematuhi regulasi yang mengharuskan PDF. Anda dapat memilih halaman tertentu dan meminta kepatuhan PDF/A melalui opsi rasterisasi lanjutan. Lihat [Save in Rasterized PDF]() dan [Advanced Rasterization Options]().

## Redaction policies

Kelompokkan beberapa redaksi menjadi kebijakan yang dapat digunakan kembali dan terapkan set aturan yang sama secara konsisten pada banyak dokumen — ideal untuk tugas berulang seperti membersihkan sekumpulan bidang standar sebelum dipublikasikan. Lihat [Use Redaction Policies]().

## Loading and saving

Muat dokumen dari jalur lokal atau dari aliran, termasuk file yang dilindungi kata sandi, dan secara opsional pra‑rasterisasi dokumen sebelum melakukan redaksi. Saat menyimpan, pertahankan format asli untuk penyuntingan lebih lanjut, timpa file asli, rasterisasi ke PDF, atau tulis ke aliran. Lihat [Loading Documents]() dan [Saving Documents]().

## On-premise

GroupDocs.Redaction untuk Python via .NET berjalan sepenuhnya di infrastruktur Anda sendiri — dokumen Anda tidak pernah meninggalkan lingkungan Anda. Paket ini adalah wheel mandiri yang menggabungkan semua yang dibutuhkan, sehingga tidak perlu menginstal Microsoft Office, OpenOffice, Adobe Acrobat, atau runtime terpisah. Lihat [System Requirements]() untuk platform yang didukung dan dependensi native.
