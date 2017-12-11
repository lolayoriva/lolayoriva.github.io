---
layout: post
section-type: post
title: Menulis posting
category: tech
tags: [ 'tutorial' ]
---

### Membuat posting baru

Jalankan script ./scripts/newpost dengan nama file dari pos sebagai argumen:

<pre><code data-trim class="bash">
cd <your { Personal } repo>
./scripts/newpost hello-world
</code></pre>

Template pos baru dengan nama YYYY-MM-DD-hello-world.md akan dibuat di bawah ./\_posts, dengan tanggal sekarang.

Di pos yang dibuat, cukup ganti Judul, Kategori dan Tag dan Anda bisa
mulai menulis posting Anda di markdown tepat di bawah akhir header posting.

Setiap file dengan format <i> YYYY-MM-DD-post-title.md </ i> akan diproses sebagai
posting, dengan tanggal publikasi <i> YYYY-MM-DD </ i>.

Konten dimulai dengan:

<pre><code data-trim class="yaml">
---
layout: post
section-type: post
title: Title
category: Category
tags: [ 'tag1', 'tag2' ]
---
</code></pre>

Variabel * layout * dan * section-type * digunakan oleh tema dan Anda tidak boleh menghapusnya.

### Hashtags

Jekyll menghasilkan halaman statis.
Akibatnya kita harus membuat halaman tag sebelum membangun dan menerbitkan situs.
Untuk menghasilkan halaman tag, cukup jalankan script * generate-tags * dari direktori root repo:

<pre><code data-trim class="bash">
./scripts/generate-tags
</code></pre>

Script akan mengurai semua posting Anda, dan membuat halaman tag untuk tag yang baru ditambahkan.

<small>Jika Anda tidak menggunakan GitHub Pages, Anda dapat mengotomatisasi pelaksanaan skrip ini selama waktu pembuatan.</small>

### Categories

Anda dapat mengatur posting Anda di bawah kategori. Kategori berperilaku seperti hashtag,
mereka harus dihasilkan secara offline, dengan menjalankan script /scripts/generate-categories.

Kategori posting ditentukan di header yaml, dalam kategori variabel.

NB! Hanya satu kategori yang dapat didefinisikan per pos.

### Syntax highlighting

Jika Anda ingin menunjukkan kode sumber di posting Anda, penyorotan sintaks disediakan.
Jika Anda ingin melihat bagaimana membuat kode Anda dengan sorotan, cukup periksa sumbernya
kode posting tutorial ini: smile:

<pre><code data-trim class="c">
{% raw %}
int main()
{
  printf("Hello, world of syntax highlighting!");

  return 0;
}
{% endraw %}
</code></pre>

<small>Jika Anda tidak memerlukan highlight sintaks di situs Anda, Anda dapat menonaktifkannya dengan menyetel variabel highlight-syntax ke False</small>

### Emoji support


Anda bisa menambahkan emojis ke posting Anda hanya dengan mengetik [emoji code](http://www.emoji-cheat-sheet.com/) :wink:

### Author Blurb

Anda bisa menambahkan deskripsi singkat tentang diri Anda di bawah posting Anda, dengan menetapkan dua variabel berikutnya di situs config
<pre><code data-trim class="yaml">
################
# Author Blurb #
################

# Penulis uraian pergi di bawah posting blog.
# Ini bekerja paling baik bila gambar uraian penulis Anda memiliki latar belakang transparan, atau sesuai dengan warna latar situs Anda.

# Jika author_blurb tidak diset, maka fitur ini dilewati
author_blurb: "Lola Yoriva adalah orang yang mengagumkan. Dia tinggal di Batam, dimana dia berkuliah di UIN SUSKA Riau. Diwaktu luangnya, Lola suka menonton film korea."
author_blurb_image: "/img/1451932973273.png"
</code></pre>
