# 07 — VISUAL QA & VERIFICATION AUDIT

**Tanggal & Tema:** 1 November 2026 — *Panggilan untuk Menjadi Teladan*  
**Konsep Terpilih:** Concept 1 — Pelayanan Tangan dan Bimbingan Kasih di Bengkel Tenda Tesalonika  
**Status Audit:** **STAGE B — PROMPTS GENERATED (ASET GAMBAR: NOT TESTED / PENDING RENDERING)**

---

## 1. Quality Gates Checklist

| Parameter Audit | Standar Evaluasi | Status Saat Ini | Catatan Verifikasi |
| :--- | :--- | :---: | :--- |
| **1. Fidelitas 4:3 Master & Painterly 3D** | Volume 3D skulptural, tekstur sapuan kuas gouache/impasto terlihat jelas di semua material, matte, tanpa CGI plastik | **NOT TESTED** *(Prompt Ready)* | Menunggu hasil render gambar master dari image generator pengguna. |
| **2. Keterbacaan Layar Jemaat (Screen-Distance)** | Siluet figur utama tegas, gestur tangan menjahit dan bimbingan kebapaan terbaca dari jarak 10x–20x lebar layar | **NOT TESTED** *(Prompt Ready)* | Komposisi subjek telah dikunci di 2/3 bawah dengan kontras lampu minyak yang terpusat. |
| **3. Integritas Zona Negatif Judul** | 35%–40% area atas dan kiri-atas kanvas 4:3 bersih dan tenang untuk penempatan judul | **PASS (By Specification)** | Spesifikasi prompt mengunci dinding bata temaram tanpa ornamen mengganggu di sepertiga atas. |
| **4. Integritas Ekspansi Kanvas 16:9** | 4:3 master terkunci di 75% tengah lebar, sayap kanan-kiri (12.5% masing-masing) hanya melanjutkan dinding dan rak | **NOT TESTED** *(Prompt Ready)* | Prompt melarang penambahan karakter baru di sayap; wajib diaudit setelah di-outpaint. |
| **5. Pelaporan Kejujuran Teknis Outpaint** | Kejujuran status penguncian piksel (Pixel-Locked vs Regenerated) | **PENDING** | Verifikasi apakah tool melakukan inpainting terkunci atau resintesis penuh saat render dijalankan. |
| **6. Ketepatan Tipografi Judul Indonesia** | Huruf, spasi, ejaan verbatim: *"Panggilan untuk Menjadi Teladan"*, isolasi alpha bersih / flat black | **PASS (By Specification)** | Ejaan dijamin 100% verbatim; warna ivory (#F5E8D3) diselaraskan dengan lampu minyak. |
| **6b. Ketepatan Tipografi Judul Toraja** | Ejaan verbatim: *"Ditambai mendadi Sangka’ (Pa’tuladanan)"*, tanda glottal stop (`’`) terjaga rapi | **PASS (By Specification)** | Khusus Ibadah Bahasa Toraja (Minggu Pertama); siap pakai pada [06b_toraja_title_prompt.md](file:///d:/codex/mjgt2026/themes/2026-11-01-panggilan-untuk-menjadi-teladan/06b_toraja_title_prompt.md). |
| **7. Larangan Teks di Dalam Ilustrasi** | Kanvas master 4:3 dan 16:9 bebas total dari huruf, tanda, watermark, atau logo | **PASS (By Specification)** | Negative prompt dan prompt utama melarang keras segala bentuk teks pada kanvas ilustrasi. |
| **8. Fidelitas Historis & Teologis** | Setting bengkel abad ke-1 akurat tanpa anakronisme; menghidupi karakter *hosios, dikaios, amemptos* | **PASS (By Specification)** | Bebas dari jubah mewah, halo mistis, atau simbol fantastis; mencerminkan kerja nyata rasul. |

---

## 2. Instruksi Verifikasi Lanjutan (Setelah Gambar Dihasilkan)
Setelah gambar di-render dan diunggah ke workspace:
1. Periksa siluet kedua tangan Paulus dan jarum penusuk; pastikan tidak ada jari berlebih atau anatomi terdistorsi.
2. Uji tumpang tindih (*overlay*) grafis judul di atas zona negatif kanvas 4:3 dan 16:9; pastikan keterbacaan teks kontras dan tidak menutupi wajah Paulus atau muridnya.
3. Potong kanvas 16:9 kembali ke 75% tengah (*crop-back test*); pastikan komposisi master 4:3 tidak terpotong atau tergeser.

