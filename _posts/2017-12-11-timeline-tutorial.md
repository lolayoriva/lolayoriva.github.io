---
layout: post
section-type: post
title: Menambahkan acara kehidupan di Timeline
category: tech
tags: [ 'tutorial' ]
---
Salah satu fitur paling keren dari {Personal} adalah yang memungkinkan Anda menceritakan kisah hidup Anda
bentuk garis waktu foto, tanggal dan deskripsi teks.

Timeline dikendalikan oleh variabel berikut:

<pre><code data-trim class="yaml">

acara:
  - image: "/img/timeline/IMG_20170507_122003.jpg"
    date: "May 2017 - Today"
    description: "Seminar Enterpreneurship bersama Sistem Informasi 14"
  - image: "/img/timeline/kelas.jpg"
    date: "September 2014 - Descember 2017"
    description: "Foto bersama Sistem Informasi Kelas D"

# Citra pertama Timeline

timeline-img: "/img/timeline/default.png"
</code></pre>

Untuk setiap acara kehidupan Anda, tambahkan tupel gambar, tanggal dan deskripsi ke acara,
dan timeline akan otomatis dihasilkan!

Variabel jalur waktu-img adalah gambar yang ingin Anda tampilkan di awal Garis Waktu Anda, menjadi kreatif!

<small>Gambar persegi disarankan 😉</small>
