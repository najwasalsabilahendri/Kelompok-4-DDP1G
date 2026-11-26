
# NutriTrack Pscilians — Aplikasi Pelacak Nutrisi dan Kesetaraan Makanan

Anggota Kelompok
- Blessing Bara Christian (NPM : 2606887582)
- Najwa Salsabila Hendri (NPM : 2606859881)
- 

Aplikasi pelacak nutrisi dan kesetaraan makanan berbasis **React, Tailwind CSS, dan Recharts** yang membantu pengguna memantau asupan kalori, menghitung kebutuhan nutrisi harian, serta menemukan alternatif makanan Indonesia berdasarkan kandungan makronutrisi.

### Latar Belakang Masalah

Banyak orang masih kesulitan mengatur pola makan karena tidak mengetahui kebutuhan kalori dan nutrisi harian mereka. Selain itu, menghitung kandungan gizi makanan dan menentukan porsi yang sesuai sering kali membutuhkan waktu serta pengetahuan khusus.

**NutriTrack Indonesia** hadir sebagai solusi untuk membantu pengguna memahami kebutuhan nutrisi tubuh, mencatat makanan yang dikonsumsi, serta memperoleh rekomendasi kesetaraan makanan berdasarkan kebutuhan Protein, Karbohidrat, Lemak, dan Serat. Dengan database makanan lokal Indonesia, pengguna dapat mengatur pola makan secara lebih praktis dan terukur.

---

## Fitur Utama

### 1. Profil Pengguna & Kalkulator Kebutuhan Nutrisi

- **Profil Pengguna:** Input Berat Badan (kg), Tinggi Badan (cm), Umur, Gender, tingkat Aktivitas, dan Tujuan Diet.
- **Kalkulator BMI:** Menghitung Body Mass Index untuk mengetahui kategori berat badan berdasarkan tinggi dan berat badan.
- **Kalkulator TDEE:** Menghitung Total Daily Energy Expenditure menggunakan formula Mifflin-St Jeor.
- **Target Nutrisi Harian:** Menghitung kebutuhan Kalori, Protein, Karbohidrat, Lemak, dan Serat berdasarkan profil dan tujuan pengguna (Turun BB, Jaga BB, atau Naik BB).

### 2. Smart Food Equivalent Engine (Fitur Utama)

- **Database Makanan Indonesia:** Menyediakan lebih dari 25 jenis makanan dengan informasi kandungan nutrisi per 100 gram, seperti Dada Ayam, Telur, Tempe, Tahu, Ikan Kembung, Daging Sapi, Nasi Putih, Nasi Merah, Kentang, Oatmeal, Brokoli, Bayam, Alpukat, dan Kacang Almond.
- **Kesetaraan Makanan Otomatis:** Menghitung jumlah gram makanan yang dibutuhkan untuk memenuhi sisa target Protein, Karbohidrat, Lemak, atau Serat pengguna.
- **Perhitungan Dinamis:** Rekomendasi porsi diperbarui secara otomatis berdasarkan sisa kebutuhan nutrisi harian.
- **Informasi Makronutrisi:** Menampilkan kandungan Protein, Karbohidrat, Lemak, Serat, dan Kalori setiap makanan.

### 3. Food Checker & Daily Food Logger

- **Pencarian Makanan:** Memungkinkan pengguna mencari makanan dari database yang tersedia.
- **Kustomisasi Porsi:** Pengguna dapat memasukkan jumlah makanan dalam satuan gram sesuai porsi yang dikonsumsi.
- **Kalkulasi Nutrisi Otomatis:** Menghitung Kalori dan seluruh makronutrisi berdasarkan berat makanan yang dimasukkan.
- **Jurnal Makanan Harian:** Menambahkan makanan ke dalam jurnal melalui tombol *Tambah ke Jurnal Hari Ini*.
- **Pelacakan Target Nutrisi:** Memperbarui progress bar Kalori, Protein, Karbohidrat, Lemak, dan Serat secara otomatis setelah makanan ditambahkan.
- **Pengurangan Sisa Target:** Seluruh makronutrisi dalam makanan ikut diperhitungkan, sehingga sisa kebutuhan harian selalu diperbarui secara akurat.

### 4. Laporan Kalori Mingguan & Bulanan

- **Dashboard Laporan:** Menampilkan riwayat konsumsi kalori dan nutrisi pengguna.
- **Filter Periode:** Pilihan tampilan laporan Mingguan dan Bulanan.
- **Grafik Kalori:** Visualisasi perbandingan asupan kalori harian dengan target kalori menggunakan Bar Chart.
- **Distribusi Makronutrisi:** Pie Chart untuk menampilkan persentase Protein, Karbohidrat, dan Lemak.
- **Riwayat Konsumsi:** Tabel catatan makanan dan asupan kalori harian.
- **Data Awal:** Menyediakan data simulasi selama 30 hari terakhir agar grafik dan laporan dapat langsung ditampilkan ketika aplikasi pertama kali dibuka.

---

## Teknologi yang Digunakan

- **Frontend:** React
- **Styling:** Tailwind CSS
- **Icons:** Lucide Icons
- **Data Visualization:** Recharts
- **Nutritional Calculation:** Mifflin-St Jeor Formula
- **Language:** JavaScript / JSX

---

## Struktur Proyek (Rancangan)

```
nutritrack-indonesia/
├── public/
│   └── assets/
│
├── src/
│   ├── components/
│   │   ├── Navbar.jsx
│   │   ├── ProfileForm.jsx
│   │   ├── BMICalculator.jsx
│   │   ├── NutritionProgress.jsx
│   │   ├── FoodEquivalent.jsx
│   │   ├── FoodChecker.jsx
│   │   ├── DailyJournal.jsx
│   │   └── NutritionCharts.jsx
│   │
│   ├── data/
│   │   └── foodDatabase.js
│   │
│   ├── utils/
│   │   ├── nutritionCalculator.js
│   │   ├── bmiCalculator.js
│   │   └── foodEquivalentCalculator.js
│   │
│   ├── pages/
│   │   ├── Dashboard.jsx
│   │   ├── FoodTracker.jsx
│   │   └── Reports.jsx
│   │
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
│
├── package.json
└── README.md
```

---

## Tujuan Pengembangan

NutriTrack Indonesia dirancang untuk membantu pengguna membangun kebiasaan makan yang lebih sehat melalui pemantauan nutrisi berbasis data. Aplikasi ini tidak hanya menghitung kalori, tetapi juga memberikan pemahaman mengenai kesetaraan makanan sehingga pengguna dapat memilih alternatif makanan lokal sesuai kebutuhan nutrisi tubuhnya.

**Catatan:** Struktur proyek di atas merupakan rancangan yang disesuaikan dengan fitur aplikasi, bukan klaim bahwa seluruh file sudah dibuat.
