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
  - image: "/img/timeline/spidertocat.png"
    date: "September 2013 - Today"
    description: "Saving the neighborhood!"
  - image: "/img/timeline/baracktocat.jpg"
    date: "September 2007 - August 2013"
    description: "Started coding"

# Citra pertama Timeline

timeline-img: "/img/timeline/default.png"
</code></pre>

Untuk setiap acara kehidupan Anda, tambahkan tupel gambar, tanggal dan deskripsi ke acara,
dan timeline akan otomatis dihasilkan!

Variabel jalur waktu-img adalah gambar yang ingin Anda tampilkan di awal Garis Waktu Anda, menjadi kreatif!

<small>Gambar persegi disarankan 😉</small>
