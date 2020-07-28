# FootNotes

Membutuhkan ekstensi `footnotes`

```yaml
markdown_extensions:
  - footnotes
```

## Penggunaan

Markup untuk catatan kaki mirip dengan markup Markdown standar untuk tautan.
Referensi dimasukkan dalam teks, yang kemudian dapat didefinisikan pada titik mana saja di
dokumen.

### Memasukkan referensi

Referensi catatan kaki terlampir dalam tanda kurung siku dan dimulai dengan tanda sisipan,
diikuti oleh label arbitrer yang mungkin berisi pengidentifikasi numerik [1, 2, 3,
...] atau nama [Granovetter et al. 1998]. Referensi yang diberikan selalu
nomor superscript berturut-turut.

Contoh:

```Markdown
Lorem ipsum [^1] dolor sit amet, consectetur adipiscing elite. [^2]
```

Hasil:

Lorem ipsum [^1] dolor sit amet, consectetur adipiscing elite. [^2]

### Memasukkan konten

Konten catatan kaki juga dideklarasikan dengan label, yang harus cocok dengan label
digunakan untuk referensi catatan kaki. Itu dapat dimasukkan pada posisi sewenang-wenang di
dokumen dan selalu ditampilkan di bagian bawah halaman. Selanjutnya, a
backlink secara otomatis ditambahkan ke referensi catatan kaki.

#### pada satu baris

Pernyataan singkat dapat ditulis pada baris yang sama.

Contoh:

```markdown
[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elite.
```

Hasil:

<a href="#fn:1">Jump to footnote at the bottom of the page</a>

  [^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elite.

#### pada banyak baris

Paragraf harus ditulis pada baris berikutnya. Seperti semua blok Markdown,
konten harus diindentasi oleh empat spasi.

Contoh:

```markdown
[^2]:
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor finabus non konsekuensi, justo purus auctor
    massa, nec semper lorem quam in massa.
```

Hasil:

  [^2]:
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
      nulla. Curabitur feugiat, tortor finibus non konsekuensiat, justo purus
      auctor massa, nec semper lorem quam in massa.

<a href="#fn:2"> Lompat ke catatan kaki di bagian bawah halaman </a>