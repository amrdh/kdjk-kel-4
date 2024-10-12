# KDJKkel4

# Aplikasi Web "Shelf"

## Sekilas Tentang

**Shelf** adalah platform manajemen inventori open source yang dirancang untuk menyederhanakan pelacakan, pengorganisasian, dan pengelolaan aset untuk individu, bisnis, dan lembaga pendidikan. Dengan fitur utamanya mengelompokkan barang, melacak lokasi aset, dan mengelola informasi terkait setiap item. Aplikasi ini cocok untuk penggunaan pribadi maupun untuk bisnis kecil yang memerlukan sistem manajemen inventaris sederhana namun efektif.


## Instalasi

Clone ke repo
```
git clone https://github.com/Shelf-nu/shelf.nu.git
cd shelf.nu
```
Install Dependencies
```
npm install
```
Setup Database
1. Buat database di supabase (https://supabase.com/)
2. Install supabase CLI
   - Instalasi via NPM
     ```
     npm install supabase --save-dev
     ```
   - Jika ingin menggunakan versi beta, jalankan
     ```
     npm i supabase@beta --save-dev
     ```
   - Catatan: Jika kamu menggunakan yarn atau bun (alternative package managers), ada angkah tambahan yang perlu diperhatikan. Sebagai contoh, untuk pengguna Yarn 4, perlu menonaktifkan fitur 
     eksperimental:
     ```
     NODE_OPTIONS=--no-experimental-fetch yarn add supabase
     ```
   - Jalankan supabase CLI 
     ```
     supabase bootstrap
     ```
3. Jalankan inisial migrasi
  ```
  npm run setup
  ```
4. Mulai local server
  ```
  npm run dev
  ```

## Cara Pemakaian
1. Pengguna dapat langsung login untuk memulai aplikasinya
   ![Login](https://github.com/user-attachments/assets/6136cb8f-0c89-4f20-9b77-17afa9072adc)

2. Setelah login pengguna akan langsung masuk ke page asset, memungkinkan pengguna melacak dan menemukan peralatan mereka dengan lebih mudah. Pada page ini pengguna dapat penambahan aset baru dan lokasi yang tepat untuk setiap barang
   ![Asset tracking](https://github.com/user-attachments/assets/d1abb181-8aee-41a8-b35f-d580981ecd00)

3. Setelah membuat asset baru pada page asset, pengguna mendapat QR untuk setiap aset, sehingga memudahkan identifikasi dan pelacakan.
   ![Qr code](https://github.com/user-attachments/assets/9ff684cd-007a-449f-8d9e-59362684e779)

4. Selanjutnya pada page categories memungkinkan pengguna untuk mengelompokkan aset ke dalam kategori tertentu, memudahkan pengelolaan dan pencarian.
   ![Categories](https://github.com/user-attachments/assets/8c456a52-695f-4005-89f8-6c08477b1405)

5. Lalu ada page tags memungkinkan pengguna untuk memberi tag pada aset untuk memudahkan pencarian dan pengelompokan.
   ![Tags](https://github.com/user-attachments/assets/39022bee-98f4-4d24-a518-510479abc950)

6. Terakhir ada page locations, memungkin pengguna dapat menambahkan dan mengelola lokasi tempat aset disimpan.
   ![Location](https://github.com/user-attachments/assets/65cbc3ac-e6f8-4461-8a64-50882c08019b)



## Pembahasan
**Shelf** memiliki beberapa kelebihan yang membuatnya menarik bagi pengguna, yaitu:
1. Aplikasi ini mudah digunakan berkat antarmuka yang intuitif, sehingga memungkinkan pengguna untuk dengan cepat mencatat dan mengelola barang hanya dengan mengambil foto, menjadikannya sangat ramah bagi mereka yang tidak memiliki pengalaman teknis.
2. Fleksibilitas dalam manajemen aset, karena tidak terbatas pada satu jenis barang; pengguna dapat mengelola berbagai aset fisik seperti peralatan, produk dagangan, atau koleksi pribadi, memberikan kebebasan dalam cara penggunaannya.
3. Sifatnya yang open-source dan gratis, yang memungkinkan pengguna untuk menyesuaikan aplikasi sesuai kebutuhan mereka tanpa biaya untuk fitur dasar, menjadikannya pilihan yang menarik untuk individu dan bisnis kecil.

Namun, ada juga beberapa kekurangan yang perlu diperhatikan. Salah satunya adalah fitur yang terbatas untuk manajemen inventaris yang kompleks. Meskipun aplikasi Shelf mudah digunakan, aplikasi ini mungkin tidak memiliki fitur canggih yang dibutuhkan oleh perusahaan besar atau pengguna yang memerlukan manajemen inventaris yang lebih mendalam. Selain itu, aplikasi ini tidak dirancang khusus untuk jenis aset tertentu, seperti buku atau peralatan IT, sehingga mungkin tidak memenuhi kebutuhan pengguna yang mencari solusi yang lebih terfokus.

Jika dibandingkan dengan software management inventori lain seperti **Inventaire** , yang fokus utamanya adalah pada manajemen koleksi buku, **Shelf** menawarkan lebih banyak fleksibilitas dalam hal jenis aset yang dapat dikelola. Inventaire memiliki keunggulan dalam pengelolaan buku, berkat integrasi dengan sumber daya komunitas seperti Wikidata yang memungkinkan pengguna untuk lebih mudah berbagi dan mengakses informasi tentang buku. Namun, jika pengguna mencari aplikasi yang dapat digunakan untuk berbagai jenis inventaris, Shelf mungkin menjadi pilihan yang lebih baik. Keduanya memiliki keunggulan dan kekurangan masing-masing, sehingga pilihan antara keduanya sangat tergantung pada kebutuhan spesifik pengguna.

## Referensi
(https://www.shelf.nu/)
