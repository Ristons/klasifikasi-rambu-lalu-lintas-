Perangkat lunak yang dibutuhkan untuk menjalankan aplikasi ini adalah sebagai berikut:
1.	Windows 10/Windows 11
2.	Google Colaboratory
3.	Google Chrome
4.	Python 3.7.9
5.	Jupyter notebook

   
I.	Petunjuk Sinkronisasi 

Sebelum menjalankan program dilakukan penyelarasan antara google colaboratory dengan local komputer agar proses eksekusi dapat dijalankan mengunakan hardware dari local komputer sehingga proses komputasi lebih cepat dan efisien.
•	Pada lokal komputer buka command jupyter notebook pada terminal power shell
 
•	Selanjutnya pada google collab buka menu connect to a local runtime dan mengcopy token localhost pada terminal powershell yang telah dibuka agar google colab dapat diselaraskan dengan lokal komputer
  
•	Logo ceklis hijau melambangkan keberhasilan penyelarasan google colab dengan lokal komputer
 
Maka sekarang google colaboratory dapat digunakan dengan menggunakan komputasi dari hardware local komputer CPU maupun GPU.

II.	Petunjuk installasi library 
•	Untuk menjalankan program dibutuhkan beberapa library yang harus diinstal pada local komputer. Cara menginstall secara langsung dari google colaboratory dengan menbahkan kode !pip dan nama library yang dibutuhkan.
 
•	untuk menginstall library dibutuhkan akses internet sehingga pastikan komputer terdapat jaringan internet.

III.	Petunjuk menjalankan program 

Setelah library yang dibutuhkan terinstall maka file program sudah dapat dijalankan berikut tahapan petunjuk menjalankan program :
1.	upload file CNN_Klasifikasi_Rambu_lalu_lintas_ProjectRiston.ipynb kedalam google colaboratory lalu buka file tersebut.  
2.	jalankann setiap baris program yang ada pada file CNN_Klasifikasi_Rambu_lalu_lintas_ProjectRiston dengan cara ke menu diatas klik Runtime > Run all atau dengan shortcut pada keyboard Ctrl+F9, sehingga seluruh baris program dijalankan secara berurutan dari atas kebawah
3.	Pastikan path atau alamat direktori file yang dibutuhkan program seperti dataset dan label.csv sudah sesuai dengan alamat direktori file pada lokal komputer 
4.	Proses menjalankan program akan menggunakan RAM, CPU, dan GPU pada lokal komputer sehingga hindari penggunaan aplikasi yang tidak diperlukan selama proses running program dilakukan 
 

IV.	Petunjuk Penggunaan Prediksi Klasifikasi Rambu Lalu Lintas

•Setelah proses running program selesai dilakukan maka dilanjutkan dengan menguji program yang telah dilatih, dengan dilakukan prediksi klasifikasi pada gambar rambu lalu lintas yang belum pernah dilihat oleh program, dengan cara memanggil fungsi prediction yang telah dibuat lalu memasukan alamat direktori file citra rambu yang ingin di uji 
Prediction(‘Alamat direktori citra rambu berekstensi .jpg’)

•Maka program akan mengeluarkan output gambar dari file tersebut serta teks untuk mengklasifikasikan rambu tersebut dari ke 43 kelas yang ada 
Untuk melakukan prediksi klasifikasi rambu lainnya lakukan hal yang sama dengan memanggil fungsi prediction dan memasukan path file direktori citra tersebut 
