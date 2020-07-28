CodeHilite
===

CodeHilite adalah ekstensi yang menambahkan penyorotan sintaks ke blok kode.
Membutuhkan ekstensi `codehilite`
```yaml
markdown_extensions:
    - codehilite
```

## Menambahkan nomor baris

Nomor baris dapat ditambahkan ke blok kode dengan mengaktifkan `linenums` bendera mkdocs.yml atau menambahkan `linenums=1` tepat setelah pengenal bahasa,

contoh :
```
``` python linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
Hasil :

``` python linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

## Sorot garis tertentu

Baris khusus dapat disorot dengan meneruskan nomor baris ke hl_linesargumen yang ditempatkan tepat setelah pengidentifikasi bahasa. Hitungan baris dimulai dari 1.

Contoh:

```
``` python hl_lines="3 4"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
Hasil :

``` python hl_lines="3 4"
""" Bubble sort """
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```