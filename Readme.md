# Langkah-langkah membuat program kasus 1

1. Install numpy, scikit-fuzzy, dan matplotlib sebelum menjalankan program.
2. Buat variabel input (barang_terjual, permintaan, harga_item, profit) dan output (stok_makanan) beserta range nilainya.
3. Tiap variabel dibagi ke beberapa kategori seperti rendah, sedang, tinggi menggunakan fungsi trimf atau trapmf.
4. Tulis aturan fuzzy yang menghubungkan kondisi input dengan output, misalnya jika permintaan tinggi dan profit banyak maka stok yang direkomendasikan banyak.
5. Kumpulkan semua rule ke dalam ControlSystem, lalu buat ControlSystemSimulation untuk menjalankannya.
6. Masukkan nilai input, lalu panggil .compute() untuk memproses hasilnya.
7. Ambil hasil dari stok_simulation.output['stok_makanan'] untuk melihat jumlah stok yang direkomendasikan.
8. Visualisasi (opsional): Panggil .view() pada tiap variabel dan plt.show() untuk menampilkan grafik fungsi keanggotaan.

# Langkah-langkah membuat program kasus 2

1. Buat 4 variabel input: kejelasan_informasi, kejelasan_persyaratan, kemampuan_petugas, dan ketersediaan_sarpras. Outputnya adalah kepuasan_pelayanan dengan range 0–400. Semua input punya range 0–100.
2. Tiap variabel input dibagi ke 3 kategori: tidak_memuaskan, cukup_memuaskan, dan memuaskan menggunakan fungsi trapesium (trapmf) dan segitiga (trimf). Output punya 5 kategori: tidak_memuaskan, kurang_memuaskan, cukup_memuaskan, memuaskan, dan sangat_memuaskan.
3. Program memiliki 81 aturan yang mencakup seluruh kombinasi dari 4 input (3 kategori masing-masing = 3^4 = 81). Setiap kombinasi menentukan output kepuasan yang dihasilkan.
4. Semua rule dikumpulkan ke dalam satu list, lalu dimasukkan ke ControlSystem dan dibungkus dengan ControlSystemSimulation.
5. Masukkan nilai untuk tiap variabel input, lalu panggil .compute() untuk memproses hasilnya.
6. Ambil hasil dari kepuasan_sim.output['kepuasan_pelayanan'] untuk melihat skor kepuasan pelayanan.
7. Visualisasi (opsional): Panggil .view(sim=kepuasan_sim) pada variabel output dan plt.show() untuk menampilkan grafik hasil defuzzifikasi.
