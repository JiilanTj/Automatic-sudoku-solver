# Solver Sudoku dengan Python

Ini adalah kode Python sederhana yang berfungsi untuk menyelesaikan teka-teki Sudoku menggunakan rekursi dan teknik "backtracking". Berikut adalah penjelasan singkat tentang bagaimana kode ini bekerja:

1. `print_board(board)`: Fungsi ini mencetak papan Sudoku dalam format yang mudah dibaca.

2. `is_valid(board, row, col, num)`: Fungsi ini memeriksa apakah angka `num` valid untuk ditempatkan di baris `row` dan kolom `col` pada papan `board`. Ini memeriksa ketiga kondisi yang harus dipenuhi: tidak ada angka yang sama di baris yang sama, tidak ada angka yang sama di kolom yang sama, dan tidak ada angka yang sama di dalam kotak 3x3 yang sama.

3. `solve_sudoku(board)`: Fungsi ini adalah algoritma utama untuk menyelesaikan teka-teki Sudoku. Ini akan mencoba untuk menempatkan angka dari 1 hingga 9 ke dalam sel yang kosong dan memeriksa apakah angka tersebut valid menggunakan `is_valid()`. Jika angka tersebut valid, maka akan mencoba untuk menyelesaikan sisa teka-teki dengan memanggil dirinya sendiri secara rekursif. Jika solusi ditemukan, itu akan mengembalikan `True`, jika tidak, akan mengembalikan `False`.

4. `sudoku_board`: Ini adalah teka-teki Sudoku yang akan dipecahkan. Anda dapat mengganti teka-teki ini dengan teka-teki Sudoku yang berbeda.

## Menjalankan Kode

Anda dapat menjalankan kode ini dengan menggunakan interpreter Python. Pastikan Anda memiliki Python terinstal di komputer Anda.

1. Salin kode di atas dan simpan dalam sebuah file dengan ekstensi `.py`.

2. Jalankan file tersebut dengan perintah berikut melalui terminal:

   ```bash
   python nama_file.py
   ```

   Gantilah `nama_file.py` dengan nama file tempat Anda menyimpan kode ini.

## Hasil

Setelah kode dijalankan, jika ada solusi yang ditemukan, maka solusi Sudoku akan dicetak di layar. Jika tidak ada solusi yang ditemukan, maka akan mencetak pesan "Tidak ada solusi yang ditemukan."
