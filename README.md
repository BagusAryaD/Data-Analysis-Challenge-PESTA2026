# 📊 IBM Telco Customer Churn Prediction

**Data Analysis Challenge PESTA 2026 - Track B: Churn Prediction**

---

## 🎯 Tentang Proyek

Proyek ini membangun model klasifikasi untuk memprediksi apakah pelanggan telekomunikasi akan **churn** (berhenti berlangganan) atau tidak. Menggunakan dataset IBM Telco Customer Churn dengan 7.043 pelanggan dan analisis mendalam terhadap fitur-fitur yang paling mempengaruhi keputusan churn.

**Interactive Report:** [https://bagus-dac-report.vercel.app/](https://bagus-dac-report.vercel.app/)

---

## 📁 File Structure

```
├── Bagus_Arya_Dwipangga_Churn.ipynb   # Jupyter Notebook (analisis lengkap)
├── ibm-telco-churn-prediction.csv     # Dataset
└── README.md                          # File ini
```

---

## 📈 Dataset

| Properti | Nilai |
|----------|-------|
| Jumlah Pelanggan | 7.043 |
| Jumlah Fitur | 24 (setelah seleksi: 19) |
| Target | `churn` (0 = tidak churn, 1 = churn) |
| Distribusi | 73.5% tidak churn, 26.5% churn |

---

## 🏆 Hasil Model

| Model | F1-Score | Recall | Precision | Accuracy |
|-------|----------|--------|-----------|----------|
| Logistic Regression | **0.616** | 0.78 | 0.51 | 74.2% |
| Random Forest | 0.615 | 0.72 | 0.54 | 75.8% |

**Model Terbaik: Logistic Regression** - Dipilih karena F1-score lebih tinggi dan recall lebih baik (0.78 vs 0.72), yang kritis untuk churn prediction karena setiap false negative merepresentasikan hilangnya pelanggan tanpa intervensi.

---

## 🔍 Fitur Paling Berpengaruh

| Fitur | Koefisien | Interpretasi |
|-------|-----------|--------------|
| internet_fiber_optic | +2.22 | Pelanggan fiber optic memiliki risiko churn jauh lebih tinggi |
| contract_two_year | -1.46 | Kontrak 2 tahun menjadi proteksi kuat terhadap churn |
| tenure_months | -0.697 | Semakin lama berlangganan, semakin kecil risiko churn |
| contract_one_year | -0.76 | Kontrak 1 tahun menurunkan churn |
| internet_dsl | +1.10 | Pelanggan DSL juga berisiko lebih tinggi |

---

## 💡 Insight Utama

1. **Internet fiber optic** adalah faktor risiko churn terbesar
2. **Kontrak jangka panjang** (1-2 tahun) adalah proteksi terbaik
3. **Tenure panjang** menunjukkan loyalitas pelanggan
4. **Pembayaran electronic check** meningkatkan risiko churn
5. **Layanan keamanan dan tech support** menurunkan churn

---

## 🛠️ Teknologi yang Digunakan

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 👤 Author

**Bagus Arya Dwipangga**

---
