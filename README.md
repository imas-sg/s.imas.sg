# Pemendek pranala IMAS

Repositori pemendek pranala untuk keperluan komunitas [IMAS](https://imas.sg)

Pemendek pranala ini memanfaatkan [fitur _redirect_ dari Netlify](https://www.netlify.com/docs/redirects/).

## Cara penggunaan

### Manual

Silakan tambahkan baris baru di _file_ [`_redirects`](./_redirects) dengan format sebagai berikut:

```_redirects
/pranala-pendek   https://contoh.com/pranala-panjang
```

Lalu _push_ langsung ke cabang `main` atau kirim _pull request_ jika Anda tidak memiliki akses _push_ langsung ke `main`.

### Otomatis

Ikuti petunjuk di [netlify-shortener](https://github.com/kentcdodds/netlify-shortener#usage), dengan syarat Anda memiliki akses _push_ langsung ke `main`.

---

# Panduan Administrasi Saung IMAS via Zoom dan Live Youtube

Tugas administrator Saung IMAS dibagi menjadi setidaknya dua tahapan: Persiapan Sebelum Hari H, dan Saat Hari H. Terdapat pula tahapan Gladi Resik yang sebaiknya dilakukan di antara keduanya. 

Silakan terlebih dahulu menghubungi owner (saat ini adalah Mas Zain) untuk meminta akses kredensial sebagai berikut:
- Akses edit pemendek pranala IMAS pada Github
- Akses login akun Zoom IMAS
- Akses login akun Gmail IMAS untuk Youtube Live (Zoom belum mendukung fitur Shared Channel)

### Persiapan Sebelum Hari H

1. **Login Zoom IMAS**  
Coba untuk melakukan login Zoom dengan menggunakan akun Zoom IMAS.

2. **Jadwalkan Zoom Meeting**  
Lakukan penjadwalan Zoom meeting baru dengan detail berikut:
```
Topic      : Saung Istiqamah Online IMAS #XX bersama XX (Silakan ganti XX dengan yang bersesuaian)
Timing     : (Sesuaikan dengan waktu tepatnya Saung IMAS dilaksanakan, biasanya berdurasi 2 jam)
Meeting ID : Generate Automatically

Security   : (Biarkan dengan setting default)
Video      : Host OFF dan Participants OFF
Audio      : Telephone and Computer Audio
Calendar   : Google Calendar

Advanced Options:
- YES : Allow participants to join anytime
- YES : Mute participants upon entry
- NO  : Automatically record meeting
- NO  : Approve or block entry for users from specific countries/regions
```

3. **Persiapkan Link Tanya-Jawab Slido**  
Tanyakan kepada owner mengenai link tanya-jawab [sli.do](https://app.sli.do/) yang akan digunakan pada Saung IMAS yang bersesuaian.

4. **Perbarui pemendek pranala IMAS**  
Edit berkas [`_redirects`](./_redirects) dengan menambahkan tiga baris berikut dan mengganti XX dengan yang bersesuaian:
```
/tanya-XX                <diisi dengan link tanya-jawab Slido>
/saung-online-XX         s.imas.sg
/saung-online-XX-zoom    <diisi dengan link zoom meeting>
```

5. **Login Youtube IMAS**  
Coba untuk melakukan login Youtube dengan menggunakan akun Youtube IMAS. Apabila diminta one-time authentication, silakan hubungi owner untuk melakukan autentikasi.

### Saat Hari H

1. **Login dan Masuk Zoom Meeting Saung IMAS**  
Coba untuk melakukan login Zoom dengan menggunakan akun Zoom IMAS, lalu masuk ke dalam Zoom meeting Saung IMAS. Tidak menutup kemungkinan pula bahwa akan ada beberapa peserta yang sudah masuk meskipun Saung IMAS belum dimulai.

2. **Persiapan Pra-Live**  
Persiapkan hal-hal berikut sebelum Pra-Live:

    - Buka Slide yang akan digunakan oleh pengisi acara. Sangat direkomendasikan berbentuk PDF, namun boleh pula PPT.
    - Apabila tidak ada Slide, maka buka poster Saung IMAS.
    - Di windows browser lain (selain yang digunakan untuk Slide/poster), bersiap untuk memperbarui pemendek pranala IMAS (atau klik saja link [berikut](https://github.com/zainfathoni/s.imas.sg/edit/main/_redirects).)
    - Di windows tersebut pula, siapkan lagu nasyid apa pun untuk dimainkan saat Pra-Live (misalnya playlist Raihan atau Snada).

3. **Sekitar 10 Menit Sebelum Saung IMAS: Pra-Live**  
Lakukan hal-hal berikut sekitar 10 menit sebelum Saung IMAS dilaksanakan:

    - Beri aba-aba bahwa Youtube sudah akan mulai Livestream. Sembari menunggu, Slide/poster akan disajikan beserta lantunan lagu nasyid.
    - Share screen Slide/poster, lalu centang ON untuk Share Audio (di pojok kiri bawah.)
    - Nyalakan lagu nasyid pilihan.
    - More > Live on Youtube.
    - Silakan gunakan akun Gmail IMAS, lalu visibility video di-set sebagai "Public".
    - Perbarui pemendek pranala IMAS dengan link Youtube.
```
/saung-online-XX         <ganti s.imas.sg dengan link Youtube>
```
    
4. **Live Saung IMAS**  
Saat Saung IMAS dimulai, Stop Share Screen, kemudian alihkan ke Slide atau pengisi acara dengan centang OFF untuk Share Audio.

5. **Saat Saung IMAS berlangsung hingga Sesi Tanya-Jawab**  
Atur laju Slide, lalu juga tidak lupa memberikan link Tanya-Jawab Slido ke kolom chat Zoom maupun Youtube Live. Saat sesi Tanya-Jawab, pantau Zoom dan juga Slido untuk pertanyaan-pertanyaan.

6. **Selesai Saung IMAS**  
Setelah ditutup, jangan lupa untuk mematikan Youtube Live: More > End/Stop Live on Youtube.

### (Opsional) Gladi Resik

Gladi Resik bersifat opsional namun sangat dianjurkan untuk dilakukan sebelum hari H agar Saung IMAS bisa berjalan dengan lebih lancar baik dari sisi penyelenggara maupun pengisi acara.

Gladi Resik dijalankan seperti melakukan administrator pada saat hari H, namun dengan beberapa perbedaan berikut:

- Tidak perlu menggunakan Zoom meeting yang sudah dijadwalkan untuk Saung IMAS. Administrator bisa membuat Zoom meeting baru atau sekadar klik "New Meeting" dengan format bebas.
- Saat melakukan Live Youtube, visibility dapat di-set sebagai "Unlisted".
- Video Live Youtube dapat dihapus setelah Gladi Resik selesai dilaksanakan.
