# 📊 Proyek Clustering dan Klasifikasi Data Pelanggan

Repositori ini merupakan implementasi lengkap untuk proyek **Clustering dan Klasifikasi** data pelanggan menggunakan Python. Proyek ini mencakup tahapan eksplorasi data, pra-pemrosesan, segmentasi pelanggan menggunakan K-Means Clustering, serta klasifikasi berdasarkan hasil segmentasi menggunakan Decision Tree dan model lainnya.

---

## ✅ Tujuan Proyek

- Menganalisis data pelanggan menggunakan **EDA** dan visualisasi.
- Membersihkan dan mempersiapkan data dengan **feature engineering**.
- Mengelompokkan pelanggan menggunakan **K-Means Clustering**.
- Menginterpretasikan hasil clustering untuk pengambilan keputusan bisnis.
- Mengklasifikasikan pelanggan berdasarkan **hasil cluster** dengan model **Decision Tree** dan lainnya.


---

## 🧪 Kriteria 1: EDA (Exploratory Data Analysis)

- ✅ `head()`, `info()`, `describe()` telah digunakan.
- ✅ Korelasi antar variabel divisualisasikan.
- ✅ Histogram semua kolom numerik dan kategorikal dibuat.
- ✅ Visualisasi rapi, tidak overlapping.

📈 Tools: `pandas`, `seaborn`, `matplotlib`

---

## 🔧 Kriteria 2: Pembersihan & Pra-Pemrosesan

- ✅ Cek dan tangani nilai null & duplikat (`isnull()`, `duplicated()`).
- ✅ Drop kolom ID: `TransactionID`, `DeviceID`, dll.
- ✅ Feature scaling: `MinMaxScaler()` / `StandardScaler()`
- ✅ Feature encoding: `LabelEncoder()` untuk kategori.
- ✅ Handling outlier dengan `IQR` / drop.
- ✅ Binning pada fitur numerik dan encode hasil binning.

📦 Tools: `sklearn.preprocessing`, `numpy`, `pandas`

---

## 📊 Kriteria 3: Model Clustering

- ✅ Dataset preprocessing digunakan untuk clustering.
- ✅ Visualisasi Elbow Method (`KElbowVisualizer`) untuk menentukan `n_clusters`.
- ✅ KMeans diterapkan (`sklearn.cluster.KMeans`)
- ✅ Model disimpan menggunakan: `joblib.dump(model_clustering)`
- ✅ Nilai Silhouette Score dihitung.
- ✅ Hasil clustering divisualisasikan.

📦 Tools: `sklearn`, `yellowbrick`, `joblib`, `PCA`

---

## 📈 Kriteria 4: Interpretasi Clustering

- ✅ Menampilkan analisis deskriptif: `mean`, `min`, `max`, `mode`.
- ✅ Invers transformasi terhadap data numerik & kategorikal.
- ✅ Interpretasi ulang hasil cluster (berdasarkan hasil inverse).
- ✅ Data hasil clustering disimpan dengan nama kolom `Target`.
- ✅ File `data_clustering_inverse.csv` telah dibuat dan disimpan.

📌 Output akhir: file `data_inisiasi.csv` dengan kolom `Target`.

---

## 🤖 Kriteria 5: Model Klasifikasi

- ✅ Dataset digunakan dari hasil clustering (`Target` sebagai label).
- ✅ Pembagian data menggunakan `train_test_split()`.
- ✅ Algoritma klasifikasi:
  - Decision Tree ✅ (`decision_tree`)
  - KNN ✅ (`explore_KNN_classification`)
- ✅ Evaluasi: Akurasi, Presisi, Recall, F1-Score ✅

📦 Tools: `sklearn.tree.DecisionTreeClassifier`, `KNeighborsClassifier`, `classification_report`, `joblib`

---
