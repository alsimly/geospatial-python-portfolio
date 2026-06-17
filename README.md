# Geospatial Python Portfolio

Kumpulan project geospasial menggunakan Python, dibangun sebagai bagian dari
persiapan magang di bidang Geo-AI dan pengolahan data spasial.

**Tools:** Python, Pandas, Matplotlib, Folium, NumPy, Google Colab  
**Data:** USGS Earthquake Feed (real-time), synthetic aerial imagery  

---

## Project 1 — Earthquake Analysis & Interactive Map

Analisis dan visualisasi data gempa bumi Indonesia secara real-time dari USGS API.

**Yang dilakukan:**
- Load 1.700+ baris data gempa global dari USGS real-time feed
- Filter wilayah Indonesia menggunakan string matching pada kolom `place`
- Visualisasi scatter plot dengan color-coding dan size berdasarkan magnitudo
- Peta interaktif dengan Folium: zoom, klik per titik, popup detail gempa

**Key insight:** Konsentrasi gempa mengikuti jalur Ring of Fire Indonesia,
sesuai dengan posisi pertemuan tiga lempeng tektonik (Eurasia, Indo-Australia, Pasifik).

**Notebooks:**
- `geo_phase1_earthquake.ipynb` — analisis dan scatter plot
- `geo_phase2_folium.ipynb` — peta interaktif

---

## Project 2 — NDVI Land Cover Analysis

Analisis vegetasi dari citra menggunakan indeks NDVI (Normalized Difference
Vegetation Index), relevan untuk use case drone pemetaan.

**Yang dilakukan:**
- Ekstraksi channel RGB dari citra sebagai array NumPy
- Kalkulasi Pseudo-NDVI menggunakan rumus `(G - R) / (G + R)`
- Klasifikasi lahan otomatis: Vegetasi Lebat, Vegetasi Sedang, Tanah/Urban, Air
- Generate laporan persentase tutupan lahan per kategori

**Limitasi yang ditemukan:** RGB tidak cukup akurat untuk NDVI karena
channel Green bukan pengganti NIR yang tepat. Sensor multispektral pada
drone profesional menyelesaikan ini dengan band NIR dedicated.

**Notebook:** `geo_phase3_ndvi.ipynb`

---

## Tentang Saya

**Aldi Syarif Alhakim**  
D3 Information Technology — CEP CCIT Fakultas Teknik, Universitas Indonesia  
Background: Network Administration, Windows Server 2022, Cisco, Red Hat Linux  

📧 syarifaldi5@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/aldi-syarif-alhakim/)
