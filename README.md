# Undangan Alya & Raka — GitHub Pages

Versi HTML statis siap diunggah ke GitHub Pages. File foto berada di repository sendiri. Tidak memakai hosting GPT dan tidak perlu npm atau proses build.

## Pasang di GitHub

1. Buat repository GitHub bernama `undangan`. Pilih Public bila memakai GitHub Free.
2. Ekstrak ZIP ini di komputer.
3. Di repository, pilih **Add file → Upload files**. Unggah `index.html`, folder `assets`, dan README ini. Pastikan `index.html` berada langsung di halaman utama repository, bukan di dalam folder tambahan. Sertakan `.nojekyll` jika terlihat; opsional untuk susunan file ini.
4. Klik **Commit changes**.
5. Buka **Settings → Pages**. Pada Source pilih **Deploy from a branch**, lalu **main** dan **/(root)**. Klik **Save**.
6. Tunggu proses penerbitan selesai. URL tampil di Settings → Pages, biasanya `https://putabintang8-coder.github.io/undangan-/`.

## Ganti foto sendiri lewat browser

Buka folder **assets/foto** di repository, pilih **Add file → Upload files**, lalu unggah foto baru dengan nama file yang sama persis seperti daftar ini. Klik **Commit changes** ke `main`. GitHub Pages akan menerbitkan perubahannya. Jika foto lama masih terlihat setelah penerbitan selesai, muat ulang halaman dengan Ctrl+Shift+R.

| Nama file | Letak di undangan |
| --- | --- |
| `sampul.jpg` | Foto pasangan di halaman utama |
| `wanita.jpg` | Foto mempelai wanita |
| `pria.jpg` | Foto mempelai pria |
| `kisah.jpg` | Bagian kisah cinta |
| `galeri-1.jpg` | Foto galeri pertama |
| `galeri-2.jpg` | Foto galeri kedua |
| `galeri-3.jpg` | Foto galeri ketiga |
| `galeri-4.jpg` | Foto galeri keempat |

Gunakan berkas JPEG sungguhan dengan nama huruf kecil dan akhiran `.jpg`. Ekspor/konversi PNG atau HEIC ke JPEG sebelum unggah; jangan sekadar mengganti ekstensi. Lebar 1200–1600 piksel sudah cukup. Foto mempelai cocok dengan komposisi vertikal dan wajah di tengah. Foto bawaan adalah foto contoh dari Unsplash; ganti dengan foto sendiri.

## Edit isi dan musik

Edit `index.html` lewat tombol pensil di GitHub untuk mengganti nama, tanggal, alamat, rekening, tautan Instagram, dan cerita. Tanggal hitung mundur ada di `CONFIG.date` (zona waktu +07:00). Teks tanggal yang tampil juga perlu diganti di HTML.

Musik saat ini memakai file `JALARANING TRESNA - ILHAM PRADANA (OFFICIAL MUSIC VIDEO) __ PUSPITA KANG MANIS AYU.mp3` di sebelah `index.html`. Untuk mengganti musik, upload MP3 baru dengan nama file yang sama. Jika ingin nama lain, sesuaikan atribut `src` di dalam elemen `<audio id="bg-music">` pada `index.html`. Tanpa file musik yang bisa diputar, undangan memakai melodi instrumental bawaan.

Nama tamu dapat diisi melalui URL, misalnya `https://putabintang8-coder.github.io/undangan-/?to=Nadia%20dan%20Keluarga`.

## Catatan fungsi

Form ucapan saat ini menambah ucapan hanya di halaman yang sedang dibuka; belum menyimpan RSVP atau ucapan ke server dan belum membagikannya ke tamu lain. GitHub Pages menyajikan file statis. Untuk menyimpan respons bersama, perlu layanan formulir atau backend terpisah.

Animasi, font, dan Tailwind masih dimuat dari CDN publik. Foto sudah berada di folder lokal repository. Versi ini belum diterbitkan ke GitHub; langkah Settings → Pages di atas perlu dilakukan di repository milik Anda.

Dokumentasi: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
