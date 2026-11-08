ABSENSI SISWA - PETUNJUK

ISI ZIP
- index.html : halaman website absensi
- config.js  : tempat mengisi konfigurasi EmailJS

MENJALANKAN WEBSITE
1. Ekstrak file ZIP.
2. Buka folder hasil ekstrak.
3. Buka index.html menggunakan browser (Chrome disarankan).
4. Jam dan tanggal tampil otomatis mengikuti WIB.

AGAR TOMBOL KIRIM MENGIRIM EMAIL
1. Buat akun di https://www.emailjs.com/
2. Tambahkan Email Service dan hubungkan email pengelola.
3. Buat Email Template dengan isi contoh:

   Nama siswa: {{student_name}}
   Status: {{attendance_status}}
   Tanggal: {{attendance_date}}
   Waktu: {{attendance_time}} ({{timezone}})

4. Salin Public Key, Service ID, dan Template ID dari dashboard EmailJS.
5. Buka config.js lalu ganti:
   ISI_PUBLIC_KEY_KAMU
   ISI_SERVICE_ID_KAMU
   ISI_TEMPLATE_ID_KAMU
   dengan nilai dari akunmu.
6. Simpan, lalu unggah semua file (index.html dan config.js) ke hosting yang mendukung website statis.

CATATAN
- Sebelum konfigurasi EmailJS diisi, form tidak mengirim email.
- Jangan memasukkan password email ke dalam file.
- Public Key EmailJS memang digunakan pada sisi browser; atur pembatasan domain di dashboard EmailJS bila tersedia.
- Ini adalah implementasi mandiri yang meniru tampilan dan fungsi utama video, bukan salinan kode asli pembuat video.
