Peringatan
===

## Pemakaian
membutuhkan ekstensi `admonition`
```yaml
markdown_extensions:
    - admonition
```

=== "Output"
    !!! note
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
        nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
        massa, nec semper lorem quam in massa.
=== "Markdown"
    ```
    !!! note
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
        nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
        massa, nec semper lorem quam in massa.
    ```	

### Mengubah judul

=== "Output"

    !!! note "Phasellus posuere in sem ut cursus"
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
        nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
        massa, nec semper lorem quam in massa.

=== "Markdown"
    ```
    !!! note "Phasellus posuere in sem ut cursus"
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
        nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
        massa, nec semper lorem quam in massa.
    ```

### Mengahapus judul

=== "Output"
    !!! note ""
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
        nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
        massa, nec semper lorem quam in massa.
	
=== "Markdown"
    ```
    !!! note ""
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
            nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
            massa, nec semper lorem quam in massa.
    ```
	
### Embeded Content

Peringatan dapat berisi judul, daftar, paragraf, peringatan dalam peringatan dan blok lainnya - kecuali blok kode ( yang biasanya untuk script).
Tapi kita bisa menggunakan ekstensi `pymdownx.superfences` untuk memasukkan script di dalam peringatan

```yaml
markdown_extensions:
    - pymdownx.superfences
```

!!! note ""
	#### Judul Di Dalam Peringatan
	
	paragraf **tebal** *miring* `blok biasa`.
	lorem ipsum dolor sit amet, Nulla euismod
    nulla. Curabitur, tortor non consequat finibus,
	
	!!! note "peringatan dalam peringatan"
		#### Kode Blocks
		```python
		# perlu ekstensi tambahan
		a = 'hello world'
		print(a)
		```
		
		> ini adalah blok-quotes


### Collapsible blocks

Ini membutuhkan ekstensi `pymdownx.details`

=== "Output"
    ??? note "Default tertutup"
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
        nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
        massa, nec semper lorem quam in massa.
	
=== "Markdown"    
    ```
    ??? note "Default tertutup"
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
        nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
        massa, nec semper lorem quam in massa.
    ```
Untuk yang defaultnya terbuka

=== "Output"
	???+ note "Default terbuka"
		Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
		nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
		massa, nec semper lorem quam in massa.

=== "Markdown"
	```
	???+ note "Default terbuka"
		Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
		nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
		massa, nec semper lorem quam in massa.	
	```	
	
## Jenis


### 1. note

!!! note
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 2. abstract

!!! abstract
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 3. info

!!! info
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 4. tip

!!! tip
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 5. succes

!!! success
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 6. question

!!! question
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 7. warning

!!! warning
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 8. failure

!!! failure
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 9. danger

!!! danger
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 10. bug

!!! bug
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 11. example

!!! example
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.
	
### 12. quote

!!! quote
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.