# 📄 Laporan Preprocessing Data
**Judul:** *Eksplorasi Outlier pada Data Minat Baca Orang Indonesia (2020–2023)*  

---

## 1. Latar Belakang
Dataset **`TGM_2020-2023_eng.csv`** berisi informasi mengenai minat baca orang Indonesia pada periode 2020–2023.  
Namun, pada data ditemukan adanya **outlier (data pencilan)** yang berpotensi memengaruhi hasil analisis.  
Oleh karena itu, dilakukan **data preprocessing** menggunakan metode **IQR (Interquartile Range)** untuk mendeteksi dan menghapus outlier.  

---

## 2. Metode IQR
Langkah-langkah deteksi outlier dengan **IQR**:  
1. Hitung **Q1 (kuartil bawah)** dan **Q3 (kuartil atas)**.  
2. Hitung **IQR = Q3 – Q1**.  
3. Tentukan batas bawah dan atas:  
   - Batas bawah = Q1 – 1.5 × IQR  
   - Batas atas = Q3 + 1.5 × IQR  
4. Data di luar rentang tersebut dianggap **outlier** → dihapus.  

---

---

## 3. File dalam Repository
- Dataset asli (raw).  
- Dataset setelah preprocessing (outlier dihapus) = 
- Notebook Python/Colab untuk preprocessing + visualisasi = https://colab.research.google.com/drive/1BOa7uEN58Bkg85dvsr_4RtBvABmEv832 
- **`README.md`** → Laporan singkat (dokumen ini).  

---

## 4. Kesimpulan
- Outlier ditemukan di beberapa kolom numerik pada dataset.  
- Dengan metode **IQR**, data lebih bersih dan siap digunakan untuk analisis lanjutan.  
- Hasil ini membantu analisis tren minat baca menjadi lebih akurat.  
