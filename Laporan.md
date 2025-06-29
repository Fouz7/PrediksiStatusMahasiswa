# Menyelesaikan Permasalahan Institusi Pendidikan

## Business Understanding
Jaya Jaya Institut merupakan salah satu institusi pendidikan perguruan yang telah berdiri sejak tahun 2000. Hingga saat ini ia telah mencetak banyak lulusan dengan reputasi yang sangat baik. Akan tetapi, terdapat banyak juga siswa yang tidak menyelesaikan pendidikannya alias dropout.

### **Permasalahan Bisnis**
- **Tingkat Dropout Tinggi**: Intitusi menghadapi tantangan dalam mempertahankan siswa hingga lulus, dengan tingkat dropout yang tinggi.
- **Kesulitan Identifikasi**: Intitusi kesulitan dalam mengidentifikasi siswa yang berisiko tinggi untuk dropout sejak awal semester.
- **Kurangnya Sistem Monitoring**: Tidak adanya sistem monitoring performa akademik siswa secara prediktif yang dapat membantu pihak manajemen dalam mengambil keputusan.

### **Cakupan Proyek**
- Melakukan analisis data untuk memahami pola serta faktor yang berkorelasi dengan tingkat dropout mahasiswa.  
- Membuat dashboard performa mahasiswa yang dapat digunakan oleh pihak manajemen untuk memantau status akademik dan retensi mahasiswa.
- Membangun model machine learning untuk memprediksi status akhir mahasiswa (Dropout, Enrolled, Graduate) yang dapat digunakan melalui Streamlit.

### Persiapan

Sumber data: [link](https://github.com/dicodingacademy/dicoding_dataset/blob/main/students_performance/data.csv)

Setup environment:
```
conda create --name Education python=3.13.3
conda activate Education
pip install -r requirements.txt
```

## Menjalankan Sistem Machine Learning
Sistem prediktif ini memungkinkan pengguna memasukkan data mahasiswa dan mendapatkan prediksi status akhir secara langsung.

Cara menjalankan secara lokal:

```
streamlit run app.py
```

Atau akses prototipe online:
Streamlit App Link: [Prototipe Streamlit](https://fouz7-prediksistatusmahasiswa-app-wel5ca.streamlit.app/)


## Business Dashboard

### Metabase 
email: root@mail.com
password: root123

<img src="/fauzan_JXmL_dashboard1.png">

<img src="fauzan_JXmL_dashboard2.png">

## Conclusion
Model machine learning yang dibangun menggunakan Random Forest Classifier berhasil mencapai akurasi ~76%, dengan f1-score terbaik untuk kelas Graduate dan Dropout. Prototipe sistem ini dapat digunakan untuk:
- Mengidentifikasi mahasiswa berisiko tinggi sejak awal
- Membantu tim akademik melakukan intervensi tepat waktu
- Memberikan dasar pengambilan keputusan berbasis data

### Rekomendasi Action Items
- **Implementasi Sistem Prediksi Dropout dan Intervensi Dini** Gunakan sistem machine learning untuk mengidentifikasi mahasiswa yang berisiko tinggi mengalami dropout secara berkala. Hasil prediksi ini dapat digunakan oleh manajemen akademik untuk melakukan intervensi dini seperti konseling, dukungan finansial, atau program mentoring.
- **Optimalisasi Dukungan Akademik dan Finansial** Tingkatkan akses mahasiswa terhadap program beasiswa, terutama bagi yang mengalami kesulitan finansial agar tidak bergantung pada hutang. Selain itu, lakukan pengawasan khusus terhadap mahasiswa di kelas malam dan mereka yang menunjukkan performa akademik rendah di semester awal. 
- **Evaluasi dan Penyesuaian Kurikulum Mata Kuliah Risiko Tinggi** Lakukan analisis terhadap mata kuliah dengan tingkat kegagalan atau dropout tinggi, seperti mata kuliah manajemen. Gunakan data ini untuk meninjau kembali metode pengajaran, beban tugas, dan efektivitas kurikulum agar lebih adaptif terhadap kebutuhan mahasiswa.
