Menyertai naskah versi 6, *Improved Hour-Ahead Solar Irradiance Forecasts in Indonesia Based on Himawari-8/9 Cloud Retrievals*. Setiap angka dalam naskah itu dan Online Resource 1-nya dihitung ulang dari database versi 6.10 dan dapat ditelusuri ke skrip serta berkas hasil di repositori ini.

**Ini rilis pra-submission (v0.1.0).** Naskah belum disubmit; versi catatan resmi akan diterbitkan sebagai v1.0.0 setelah diterima.

- **Tata letak:**
  - `paper_v2_clpbanten/`: helper, skrip tahap yang dipakai ulang, tahap database 93–113, analisis pendukung di tahap 114;
  - `Manuskrip_versi6/`: protokol pelatihan, analisis, hasil;
  - `training mirip/`, `data_versions/`, `figures/`.
- **Data:** database 6.10. Langit cerah dirata-ratakan per slot. CLP Himawari-8/9 diekstraksi ulang dalam kotak berpusat stasiun, dengan cakupan retrieval kotak. Meteorologi AWS diperiksa terhadap SYNOP dan dibangun ulang secara kausal. Laporan SYNOP dipertahankan 50 menit.
- **Metode:**
  - 44 prediktor;
  - delapan arsitektur × lima seed di bawah satu protokol;
  - statistik kotak dibangun ulang dan diverifikasi terhadap chip Himawari;
  - analisis pendukung dihitung ulang pada versi 6.10;
  - pemeriksa yang menghitung ulang setiap angka yang dikutip naskah.
- **Tidak didistribusikan:** observasi stasiun, database dan model frame, arsip prediksi, model terlatih, arsip ekstraksi, berkas naskah.

Rincian ada di `CHANGELOG.md`.
