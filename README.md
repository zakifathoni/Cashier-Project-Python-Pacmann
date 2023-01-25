# Cashier-Project-Python-Pacmann
Repository ini berisi kode python untuk membuat objek transaksi yang dapat menambahkan, mengupdate, menghapus, dan menampilkan item yang dibeli serta menghitung total harga dan diskon yang diterima.

# Flowchart

  ```mermaid
graph LR
A[Transaction] --> B[__init__] --> C[add_item]
A --> C[add_item]
A --> D[update_item_name]
A --> E[update_item_qty]
A --> F[update_item_price]
A --> G[delete_item]
A --> H[reset_transaction]
A --> I[check_order]
A --> J[hitung_total_price]

B --> C
B --> D
B --> E
B --> F
B --> G
B --> H
B --> I
B --> J

C --> B
C --> D
C --> E
C --> F
C --> G
C --> H
C --> I
C --> J

D --> C
D --> B
D --> E
D --> F
D --> G
D --> H
D --> I
D --> J

E --> C
E --> D
E --> B
E --> F
E --> G
E --> H
E --> I
E --> J

F --> C
F --> D
F --> E
F --> B
F --> G
F --> H
F --> I
F --> J

G --> C
G --> D
G --> E
G --> F
G --> B
G --> H
G --> I
G --> J

H --> C
H --> D
H --> E
H --> F
H --> G
H --> B
H --> I
H --> J

I --> C
I --> D
I --> E
I --> F
I --> G
I --> H
I --> B
I --> J

J --> C
J --> D
J --> E
J --> F
J --> G
J --> H
J --> I
J --> B
  ```

# Penggunaan:

1. Import library `tabulate` dengan perintah `from tabulate import tabulate`.
2. Buat objek transaksi dengan membuat instance dari kelas `Transaction`, misal `trnsct_123 = Transaction()`.
3. Gunakan method `add_item` untuk menambahkan item ke dalam transaksi, dengan format `trnsct_123.add_item(["nama item", jumlah item, harga/item])`.
4. Gunakan method `update_item_name`, `update_item_qty`, dan `update_item_price` untuk mengupdate nama item, jumlah item, dan harga/item.
5. Gunakan method `delete_item` untuk menghapus item dari transaksi.
6. Gunakan method `reset_transaction` untuk menghapus semua item dari transaksi.
7. Gunakan method `check_order` untuk menampilkan daftar item yang dibeli dalam bentuk tabel.
8. Gunakan method `hitung_total_price` untuk menghitung total harga dan diskon yang diterima.

# Contoh Penggunaan:

1. Pertama, buat objek transaksi dengan membuat instance dari kelas `Transaction`, misal `trnsct_123 = Transaction()`.
2. Kemudian, tambahkan item ke dalam transaksi dengan menggunakan method `add_item()`. Contoh penggunaan: `trnsct_123.add_item(["Ayam Goreng", 2, 20000])`.
3. Anda juga dapat mengupdate atau menghapus item yang sudah ditambahkan dengan menggunakan method `update_item_name()`, `update_item_qty()`, `update_item_price()`, dan `delete_item()`.
4. Anda dapat menampilkan daftar item yang dibeli dengan menggunakan method `check_order()`, yang akan menampilkan daftar item dalam bentuk tabel.
5. Anda dapat menghitung total harga dan diskon yang diterima dengan menggunakan method `hitung_total_price()`.
6. Semua method yang tersedia dalam kelas `Transaction` dapat digunakan untuk mengatur dan mengelola transaksi Anda.

> Note: Pada kode di atas, diskon yang diterima ditentukan berdasarkan total harga transaksi. Jika total harga > 500_000 maka diskon yang diterima adalah 10%, jika total harga > 300_000 maka diskon yang diterima adalah 8%, dan jika total harga > 200_000 maka diskon yang diterima adalah 5%. Anda dapat mengubah persentase diskon sesuai dengan kebutuhan Anda dengan mengubah kondisi pada method `hitung_total_price()`.

Selain itu, Anda juga dapat menambahkan atau mengubah fitur lain pada kelas `Transaction` sesuai dengan kebutuhan Anda. Contohnya Anda dapat menambahkan feature untuk menambahkan customer name atau no.invoice pada transaksi.
