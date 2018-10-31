# Database _Indexing_
Banyak orang mengeluhkan tentang lambatnya performa akses data pada database, padahal sudah merasa membuat index. 
Padahal belum tentu index yang sudah dibuat itu bisa digunakan oleh si DBMS ketika mengakses data menggunakan query yang diberikan.

Supaya terhindar dari pembuatan index yang sia-sia, pada tutorial ini kita akan belajar bagaimana membuat index yang tepat guna, yang akan membuat hidup kita lebih bahagia :)

## Kenapa melakukan _indexing_?

_Indexing_ diperlukan untuk mempercepat performa _query_ data pada _database_. _Query_ yang dimaksud adalah pengambilan / pembacaaan data.
Bagaimana dengan penulisan data? Apakah akan terbantu juga dengan adanya _indexing_? Sayangnya **tidak**. 
Justru _indexing_ akan menambah beban proses ketika melakukan penulisan data pada _database_, karena terjadi penulisan selain pada tabel juga pada index-nya.

Bingung maksudnya? Tenang, di bagian selanjutnya akan dibahas kok. 

## Saya _developer_ perangkat lunak, buat apa paham _indexing_?
Index akan membantu query hanya jika ia tepat guna. Index dikatakan tepat guna atau tidak itu bergantung pada **bagaimana suatu perangkat lunak
mengakses data** atau **bagaimana suatu perangkat lunak meng-query data**.

Siapa yang paling paham tentang bagaimana aplikasi mengakses data? Ya tentu saja _developer_-nya.
