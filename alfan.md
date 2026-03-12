Nama : Alfan Maulana 
Kelas : C3, S1-Informatika 
Matkul : Pemrograman Phyton (Machine Learning)
Tugas Pertemuan 2
Classification

![alt text](Picture1.png)
 
Test and Score
 
a. Which model had the highest AUC?
Model yang memiliki nilai AUC tertinggi adalah Random Forest karena memiliki nilai sebesar 0.858
b. Which model had the highest F1?
Model dengan nilai F1 tertinggi adalah Random Forest, memiliki nilai sebesar 0.811
c. Are these the same model? Which would you choose and why?
Model yang memiliki nilai AUC dan F1 Score tertinggi adalah Random Forest, sehingga model ini dipilih sebagai model terbaik dalam proses klasifikasi karena Random Forest menunjukkan performa yang paling baik dibandingkan dengan model lain yang diuji dapat dilihat dari nilai AUC sebesar 0.858 dan F1 Score sebesar 0.811 merupakan nilai tertinggi di antara semua model. Selain itu, Random Forest juga memiliki nilai accuracy (CA) tertinggi yaitu 0.813 nilai-nilai tersebut menunjukkan bahwa Random Forest mampu melakukan klasifikasi data dengan lebih baik dan lebih seimbang dalam memprediksi kelas dibandingkan model lainnya, sehingga model ini menjadi pilihan yang paling tepat untuk digunakan pada dataset tersebut.
d. How many passengers did the best model incorrectly predict as 'survived' when they did not?
 
•	Total Actual 0 = 546
•	Persentase yang diprediksi 1 = 12.1%
•	12.1% × 546 ≈ 66
Model terbaik yaitu Random Forest secara salah memprediksi sekitar 66 penumpang sebagai selamat padahal sebenarnya tidak selamat. Kesalahan ini disebut False Positive, yaitu ketika model memprediksi kelas positif tetapi kenyataannya termasuk kelas negatif.

Regression
 
Test and Score
 
a. Which model had the lowest MAE? By how much?
Model yang memiliki nilai MAE paling rendah adalah Random Forest, yaitu sebesar 51036.845. Nilai ini sekitar 1004.575 lebih kecil dibandingkan kNN dan sekitar 15219.581 lebih kecil dibandingkan Linear Regression, sehingga Random Forest menghasilkan rata-rata kesalahan prediksi paling kecil.
b. Which model had the best R²?
Model dengan nilai R² terbaik adalah Random Forest dengan nilai 0.824, yang berarti model tersebut mampu menjelaskan sekitar 82.4% variasi pada data harga rumah.
c. Open Predictions for your best model. Find the row with the largest error. Predicted vs actual?
 
Baris dengan error terbesar terdapat pada baris ke-8, di mana model Random Forest memprediksi nilai 814205, sedangkan nilai sebenarnya adalah 980700. Selisih antara nilai prediksi dan nilai aktual adalah sekitar 166495, yang menunjukkan bahwa model melakukan kesalahan prediksi terbesar pada data tersebut.
d. What does this suggest about what the model struggles with?
Perbedaan yang besar antara nilai prediksi dan nilai sebenarnya menunjukkan bahwa model mengalami kesulitan dalam memprediksi data dengan nilai harga rumah yang sangat tinggi.
Hal ini kemungkinan disebabkan oleh:
•	adanya nilai ekstrem (outlier) pada dataset
•	jumlah data dengan harga rumah sangat tinggi yang relatif sedikit
•	pola data yang tidak sepenuhnya dapat ditangkap oleh model
Sehingga model Random Forest terkadang meng-underestimate harga rumah pada nilai yang sangat tinggi.
