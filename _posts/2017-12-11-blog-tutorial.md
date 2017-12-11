---
layout: post
section-type: post
title: Setting up the Blog
category: tech
tags: [ 'tutorial' ]
---


Sebuah situs web benar-benar pribadi jika host blog Anda juga, tempat internet ini
Di mana Anda dapat menempatkan pikiran Anda tentang apapun!

### Pratinjau postingan terbaru di Index page

Pertama-tama, Anda mendapatkan preview dari posting terbaru dalam indeks, untuk menarik pengunjung mengunjungi blog Anda.
Ukuran pratinjau ini ditentukan oleh:

<pre><code data-trim class="yaml">
post-preview-words: 96
</code></pre>

Jangan ragu untuk bereksperimen dengan ukuran yang berbeda, dan pilih yang terbaik untuk Anda: senyuman:

### Arsipkan

Sebuah blog diharapkan menjadi tuan rumah banyak posting, jadi Anda memerlukan arsip dengan pagination,
yang singkatnya adalah pengelompokan posting Anda di halaman, secara terbalik kronologis
memesan. Anda dapat menentukan jumlah posting yang ditampilkan per halaman dengan mengubah:

<pre><code data-trim class="yaml">
paginate: 5
</code></pre>

### Tombol berbagi

Banyak tombol berbagi tersedia dan dapat diaktifkan atau dinonaktifkan dengan menyetel yang berikut:

<pre><code data-trim class="yaml">
email-share: True
fb-share: True
twitter-share: True
linkedin-share: True
reddit-share: True
google-plus-share: True
tumblr-share: True
pinterest-share: True
pocket-share: True
vkontakte-share: True
</code></pre>

### Komentar

Anda dapat mengaktifkan komentar <a href="http://www.disqus.com" target="\blank"> Disqus </a> dengan hanya menyetel nama pengguna Disqus Anda di sini:

<pre><code data-trim class="yaml">
disqus-shortname: "nama pengguna Disqus Anda"
</code></pre>

### RSS feed

Umpan RSS dibuat secara otomatis dan ditempatkan di /feed.xml.

### Sitemap

Peta Situs dibuat secara otomatis dan ditempatkan di /sitemap.xml
