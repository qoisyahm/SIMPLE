# Design Direction: Sistem Informasi Pelaporan Lingkungan Kota (SIPELIK)

## 1. Identity & Purpose
- **System**: Sistem Informasi Pelaporan Lingkungan Kota (SIPELIK)
- **Scope**: Platform terpadu pelaporan kerusakan fasilitas umum dan pencemaran lingkungan berbasis web untuk warga kota dan petugas dinas terkait (Agile MPPL).
- **Core Mission**: Menghubungkan partisipasi aktif masyarakat dengan respon cepat pemerintah kota secara transparan, akuntabel, dan terukur.
- **Reading this as**: Civic-tech web application portal for urban citizens and municipal inspectors, in a clean, modern Indonesian civic-utility style.
- **Dial**: ENERGY 2 / RHYTHM 2 / MOTION 1

## 2. Palette (Strict 3 Core Colors + Accents)
- **Primary Civic Brand**: Emerald Forest (`#0d5c3a` dark / `#15803d` vibrant) - Melambangkan kelestarian lingkungan hidup dan otoritas publik yang ramah.
- **Secondary Neutral Slate**:
  - Light mode: Deep Charcoal `#0f172a`, Muted Slate `#475569`, Background `#f8fafc`, Surface `#ffffff`, Border `#e2e8f0`
  - Dark mode: Midnight `#090d16`, Surface Card `#111827`, Border `#1f2937`, Muted `#94a3b8`
- **Functional Status Palette**:
  - `Menunggu Verifikasi`: Amber Warm (`#d97706` / bg `#fef3c7`)
  - `Sedang Diproses`: Royal Sky (`#0284c7` / bg `#e0f2fe`)
  - `Selesai Ditangani`: Emerald Green (`#059669` / bg `#d1fae5`)
  - `Ditolak / Tidak Valid`: Crimson (`#e11d48` / bg `#ffe4e6`)

## 3. Typography
- **Primary Typeface**: Plus Jakarta Sans (Google Fonts), geometric clean sans-serif yang dirancang dengan keterbacaan tinggi untuk antarmuka publik modern.
- **Hierarki Skala**:
  - Judul Aplikasi: 1.5rem - 1.875rem, font-weight 700
  - Header Kartu/Bagian: 1.125rem - 1.25rem, font-weight 600
  - Body Text: 0.9375rem (15px), line-height 1.6, font-weight 400
  - Metadata & Badge: 0.75rem - 0.8125rem, font-weight 500

## 4. Layout & Rhythm (RHYTHM 2)
- **Citizen Portal**:
  1. Top Utility Header: Identitas dinas kota, tombol navigasi tab, toggle role (Warga / Petugas), toggle tema (Terang / Gelap).
  2. Quick Stats Banner: Rekapitulasi laporan real-time berdasarkan data aktif sistem (Total Aduan, Verifikasi, Diproses, Tuntas).
  3. Interactive Split Workspace:
     - Panel Kiri: Formulir Pelaporan Aduan Cepat (Upload foto dengan drag-drop/preview, pilih kategori, deskripsi, pin lokasi GPS).
     - Panel Kanan: Peta Interaktif Sebaran Laporan (Leaflet + OpenStreetMap) dengan filter kategori dan status.
  4. Pelacak Tiket Aduan Mandiri: Input kode tiket untuk melihat linimasa penanganan dan catatan resmi petugas.
  5. Daftar Laporan Terkini: Umpan transparansi publik aduan yang sedang atau telah ditangani.
- **Petugas/Admin Portal**:
  1. Ringkasan Eksekutif & Statistik Rekapitulasi Kategori dan Wilayah/Kecamatan.
  2. Meja Verifikasi & Validasi Aduan: Aksi setujui/tolak aduan, perbarui status ke 'Diproses' atau 'Selesai', dan tulis catatan resmi penanganan.
  3. Log Audit dan Info Pengembang Tim MPPL (Scrum Sprint).

## 5. Motion & Interaction (MOTION 1)
- Micro-interactions: Transisi fokus halus (150ms-200ms ease), status chip hover, leaflet marker popup pulse.
- Bebas dari animasi berlebihan atau template slide/fade mengambang yang tidak fungsional.
