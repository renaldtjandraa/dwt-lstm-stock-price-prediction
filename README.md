# Prediksi Harga Saham dengan LSTM dan Discrete Wavelet Transform (DWT)

Repositori ini merupakan dokumentasi dan implementasi dari skripsi sarjana berjudul:  
**“Penerapan LSTM dalam Prediksi Harga Saham Menggunakan Preprocessing Discrete Wavelet Transform”**  
oleh **Renald Kharisma Tjandra**,  
Institut Teknologi Harapan Bangsa, 2024.

---

## Deskripsi 

Penelitian ini menggabungkan model Long Short-Term Memory (LSTM) dengan teknik transformasi sinyal **Discrete Wavelet Transform (DWT)** untuk meningkatkan akurasi dalam prediksi harga saham. DWT digunakan untuk melakukan dekomposisi data time-series sehingga dapat mengurangi noise dan menangkap pola frekuensi yang relevan sebelum diproses oleh LSTM.

---

## Tools & Teknologi

- Python
- TensorFlow / Keras
- PyWavelets
- NumPy, Pandas, Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook

--- 
## Hyperparameter yang Digunakan

Dalam proses pelatihan model LSTM, dilakukan eksperimen dengan beberapa kombinasi nilai hyperparameter untuk mendapatkan performa model terbaik. Adapun hyperparameter yang digunakan adalah sebagai berikut:

Batch Size: [16, 32]
Ukuran batch menentukan jumlah sampel data yang diproses sebelum model melakukan update terhadap bobot. Digunakan dua nilai berbeda untuk mengamati pengaruh ukuran batch terhadap konvergensi model.

Epoch: [50, 100]
Jumlah epoch mengindikasikan berapa kali seluruh dataset digunakan untuk melatih model. Nilai 50 dan 100 digunakan untuk melihat apakah model mendapatkan peningkatan performa dengan pelatihan yang lebih panjang.

Jumlah Neuron (hidden units): [20, 50]
Menentukan jumlah neuron pada lapisan tersembunyi LSTM. Nilai yang lebih tinggi berpotensi menangkap pola yang lebih kompleks, namun juga meningkatkan risiko overfitting.

Eksperimen dilakukan dengan kombinasi dari ketiga hyperparameter tersebut untuk mengevaluasi performa model berdasarkan metrik seperti MSE (Mean Squared Error) dan RMSE (Root Mean Squared Error).


