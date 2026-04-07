# Langkah-langkah membuat program kasus 1

1. Install numpy, scikit-fuzzy, dan matplotlib sebelum menjalankan program.
2. Buat variabel input (barang_terjual, permintaan, harga_item, profit) dan output (stok_makanan) beserta range nilainya.
3. Tiap variabel dibagi ke beberapa kategori seperti rendah, sedang, tinggi menggunakan fungsi trimf atau trapmf.
4. Tulis aturan fuzzy yang menghubungkan kondisi input dengan output, misalnya jika permintaan tinggi dan profit banyak maka stok yang direkomendasikan banyak.
5. Kumpulkan semua rule ke dalam ControlSystem, lalu buat ControlSystemSimulation untuk menjalankannya.
6. Masukkan nilai input, lalu panggil .compute() untuk memproses hasilnya.
7. Ambil hasil dari stok_simulation.output['stok_makanan'] untuk melihat jumlah stok yang direkomendasikan.
8. Visualisasi (opsional): Panggil .view() pada tiap variabel dan plt.show() untuk menampilkan grafik fungsi keanggotaan.

# Langkah-langkah membuat program kasus 1

1. Install numpy, scikit-fuzzy, dan matplotlib sebelum menjalankan program.
2. Buat variabel input (barang_terjual, permintaan, harga_item, profit) dan output (stok_makanan) beserta range nilainya.
3. Tiap variabel dibagi ke beberapa kategori seperti rendah, sedang, tinggi menggunakan fungsi trimf atau trapmf.
4. Tulis aturan fuzzy yang menghubungkan kondisi input dengan output, misalnya jika permintaan tinggi dan profit banyak maka stok yang direkomendasikan banyak.
5. Kumpulkan semua rule ke dalam ControlSystem, lalu buat ControlSystemSimulation untuk menjalankannya.
6. Masukkan nilai input, lalu panggil .compute() untuk memproses hasilnya.
7. Ambil hasil dari stok_simulation.output['stok_makanan'] untuk melihat jumlah stok yang direkomendasikan.
8. Visualisasi (opsional): Panggil .view() pada tiap variabel dan plt.show() untuk menampilkan grafik fungsi keanggotaan.
