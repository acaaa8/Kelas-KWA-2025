# Juice Shop Christmas Special

1. Buka aplikasi Burp Suite dan atur proxy di browser kamu agar semua lalu lintas request dari browser melewati Burp Suite.
2. Buka situs OWASP Juice Shop dan navigasikan ke halaman pencarian produk.
3. Di browser, cari kata kunci apa pun (misalnya, a). Burp Suite akan menangkap request pencarian ini.
4. Di Burp Suite, temukan request dengan URL yang mengandung /rest/products/search.
5. Pada bagian request di Burp Suite, ubah nilai parameter q. Hapus kata kunci yang tadi kamu ketik, lalu masukkan payload SQL Injection:' UNION SELECT * FROM PRODUCTS WHERE deleted=1 --
   <img width="740" height="169" alt="image" src="https://github.com/user-attachments/assets/62305a3c-073f-4f6d-9596-7aba4f2964bb" />
6. Setelah payload dimasukkan, Send to Repeater atau Send to Intruder.
7. Cari produk yang namanya berhubungan dengan "Christmas Special"

