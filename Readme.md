Langkah-langkah membuat program kasus 1
Langkah 1 
Install numpy, scikit-fuzzy, dan matplotlib sebelum menjalankan program.
Langkah 2 
Buat variabel input (barang_terjual, permintaan, harga_item, profit) dan output (stok_makanan) beserta range nilainya.
Langkah 3 
Tiap variabel dibagi ke beberapa kategori seperti rendah, sedang, tinggi menggunakan fungsi trimf atau trapmf.
Langkah 4 
Tulis aturan fuzzy yang menghubungkan kondisi input dengan output, misalnya jika permintaan tinggi dan profit banyak maka stok yang direkomendasikan banyak.
Langkah 5 
Kumpulkan semua rule ke dalam ControlSystem, lalu buat ControlSystemSimulation untuk menjalankannya.
Langkah 6
Masukkan nilai input, lalu panggil .compute() untuk memproses hasilnya.
Langkah 7  
Ambil hasil dari stok_simulation.output['stok_makanan'] untuk melihat jumlah stok yang direkomendasikan.
Langkah 8 — Visualisasi (opsional)
Panggil .view() pada tiap variabel dan plt.show() untuk menampilkan grafik fungsi keanggotaan.

Langkah-langkah membuat program kasus 2
Langkah 1, Definisi variabel input dan output
Buat 4 variabel input: kejelasan_informasi, kejelasan_persyaratan, kemampuan_petugas, dan ketersediaan_sarpras. Outputnya adalah kepuasan_pelayanan dengan range 0–400. Semua input punya range 0–100.
Langkah 2, Fungsi keanggotaan
Tiap variabel input dibagi ke 3 kategori: tidak_memuaskan, cukup_memuaskan, dan memuaskan menggunakan fungsi trapesium (trapmf) dan segitiga (trimf). Output punya 5 kategori: tidak_memuaskan, kurang_memuaskan, cukup_memuaskan, memuaskan, dan sangat_memuaskan.
Langkah 3, Definisi rules
Program memiliki 81 aturan yang mencakup seluruh kombinasi dari 4 input (3 kategori masing-masing = 3⁴ = 81). Setiap kombinasi menentukan output kepuasan yang dihasilkan.
Langkah 4, Buat sistem kontrol
Semua rule dikumpulkan ke dalam satu list, lalu dimasukkan ke ControlSystem dan dibungkus dengan ControlSystemSimulation.
Langkah 5, Input dan komputasi
Masukkan nilai untuk tiap variabel input, lalu panggil .compute() untuk memproses hasilnya.
Langkah 6, Output
Ambil hasil dari kepuasan_sim.output['kepuasan_pelayanan'] untuk melihat skor kepuasan pelayanan.
Langkah 7 Visualisasi (opsional)
Panggil .view(sim=kepuasan_sim) pada variabel output dan plt.show() untuk menampilkan grafik hasil defuzzifikasi.