# Fintech Battle: Sentiment Analysis (DANA vs OVO)

## 📊 Project Overview
Analisis sentimen ulasan aplikasi fintech **DANA** dan **OVO** dari Google Playstore.  
Label sentimen ditentukan otomatis menggunakan **IndoBERT Sentiment Classifier**, kemudian diproses dengan **TF-IDF + Random Forest** untuk klasifikasi.  
Hasil visualisasi berupa **Confusion Matrix, WordCloud, dan Distribusi Sentimen** digunakan untuk menggali insight bisnis.  

---

## 🚀 Results

### Distribusi Sentimen
| App  | Negative | Neutral | Positive |
|------|----------|---------|----------|
| DANA | 72,483   | 14,614  | 19,368   |
| OVO  | 52,787   | 13,245  | 17,150   |

- **DANA**: mayoritas review negatif (**72 ribu**) jauh lebih banyak dibanding positif (19 ribu).  
- **OVO**: sama-sama didominasi negatif (**52 ribu**), meski secara proporsi sedikit lebih baik dibanding DANA.  
- **Kesimpulan awal**: kedua aplikasi menghadapi dominasi review negatif → tanda perlu perbaikan signifikan pada kualitas layanan maupun aplikasi.  

---

### 🔎 Top 20 Kata Negatif
**DANA**  
`saya, dana, di, bisa, tidak, ini, aplikasi, ada, nya, dan, saldo, ke, sudah, gak, mau, tapi, ga, masuk, lagi, padahal`

**OVO**  
`saya, ovo, di, bisa, aplikasi, ini, ke, nya, tidak, gak, ada, mau, ga, sudah, dan, masuk, upgrade, udah, saldo, aja`

---

## 💡 Business Insights
- **DANA**  
  - Banyak keluhan terkait **saldo**, **login/masuk**, serta ketidakpuasan pengguna (kata seperti *tidak, gak, padahal* sering muncul).  
  - Perlu meningkatkan keandalan sistem transaksi dan memperbaiki pengalaman login.  

- **OVO**  
  - Kata **upgrade**, **saldo**, dan **login** sering muncul dalam review negatif.  
  - Masalah teknis saat upgrade/akses akun dan saldo yang bermasalah menjadi sorotan utama.  

- **Kedua aplikasi**  
  - Sama-sama menghadapi **trust issue** (user merasa aplikasi tidak memenuhi ekspektasi).  
  - Fokus perbaikan: stabilitas aplikasi, kejelasan fitur, serta transparansi saldo/promo.  

---

## 🛠️ Tech Stack
- **Data Processing**: Pandas, Regex, Emoji, Sastrawi  
- **Modeling**: IndoBERT (HuggingFace Transformers), Scikit-learn (TF-IDF, Random Forest)  
- **Visualization**: Matplotlib, WordCloud  

---

## 📂 Outputs
- Confusion Matrix → `confusion_matrix_rf.png`   
- WordCloud per app & sentimen → `wc_DANA_positive.png`, `wc_OVO_negative.png`, dll.  
- Distribusi Sentimen → `distribusi_sentimen.png`  

---
