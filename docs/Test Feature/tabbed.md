Tab
===
Membutuhkan ekstensi `pymdownx.tabbed` tampilannya akan seperti dibawah ini,

```yaml
markdown_extensions:
    - pymdownx.tabbed
```

!!! example "Contoh"
    === "Tab 1"
        Markdown **content**.

        Multiple paragraphs.

    === "Tab 2"
        More Markdown **content**.

        - list item a
        - list item b

``` 
=== "Tab 1"
    Markdown **content**.

    Multiple paragraphs.

=== "Tab 2"
    More Markdown **content**.

    - list item a
    - list item b

```

!!! example "Contoh"
    === "Tab 1"
        Markdown **content**.

        Multiple paragraphs.

    === "Tab 2"
        More Markdown **content**.

        - list item a
        - list item b

    ===! "Tab A"
        Different tab set.

    === "Tab B"
        ```
        More content.
        ```

```
=== "Tab 1"
    Markdown **content**.

    Multiple paragraphs.

=== "Tab 2"
    More Markdown **content**.

    - list item a
    - list item b

===! "Tab A"
    Different tab set.

=== "Tab B"
    ```
    More content.
    ```
```