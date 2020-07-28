# MyPage
## this is layout tes



- [Titles](#titles)
- [Paragraphs](#paragraphs)
- [Line Break](#line-break)
- [Emphasis](#emphasis)
- [Blockquote](#blockquote)
- [List](#list)
- [Horizontal rule](#horizontal-rule)
- [Code](#code)
- [Link](#link)
- [Image](#image)
- [Escape](#escape)
- [Table](#table)
- [Collapsible Area](#collapsible-area)
- [Task List](#task-list)
- [CSS](#css)

# Titles

```markdown
`# Title` => <h1>Title</h1>
...
`###### Title 6` => <h6>Subtitle</h6>
```


# Paragraphs

To create paragraphs, use a blank line to separate one or more lines of text.

```markdown
First line

Second line
```


# Line Break

-  To create a line break (`<br>`):
   - **Usual:** end a line with trailing space (two or more spaces), and then type return.
   - **Best:** to make the line break visible, use `<br>` instead of trailing space


# Emphasis
*test* **test**

~~test~~

```markdown
`*test*` => <em>test</em>
`**test**` => <strong>test</strong>
`***test***` => <strong><em>test</em></strong>

`~~test~~` = strikethrough text
```


# Blockquote

```markdown
> this is</br>
> a blockquote</br>
> example</br>
>
> this is a line after a blank line
>> this is nested
```

Result:

> this is</br>
> a blockquote</br>
> example</br>
>
> this is a line after a blank line
>> this is nested


# List

- To **sub itens**, indent with four spaces in ordered lists and two spaces in non-ordered lists

1. first
2. second
    1. sub first
    2. sub second
3. third

```markdown
1. first
2. second
    1. sub first
    2. sub second
3. third
```

- first
- second
  - sub first
  - sub second
- third

```markdown
- first
- second
  - sub first
  - sub second
- third
```


# Horizontal rule

---

```markdown
---

or

___
```


# Code

- Use two backticks for inline code and six for blocks of code, put the code right in the middle of them
- if you inline code contains a backslash, use double backslash in which side of the inline code

```markdown

`inline code`

``inline code containing a ` backtick``

```

```python
a = 'hello'
print(a)
```

# Link

```markdown
My favorite search engine is [Duck Duck Go](https://duckduckgo.com "this is my title tooltip")
```

```markdown
[Emphasis Link](#Emphasis)
```


# Image

![Image example](https://d33wubrfki0l68.cloudfront.net/e7ed9fe4bafe46e275c807d63591f85f9ab246ba/e2d28/assets/images/tux.png "This is my title tooltip")

```markdown
![Image example](https://d33wubrfki0l68.cloudfront.net/e7ed9fe4bafe46e275c807d63591f85f9ab246ba/e2d28/assets/images/tux.png "This is my title tooltip")
```


# Escape

Escape by:
  - adding a leading backslash in front of: ``\ ` * - {} [] () # + - . ! |``
  - using html code, e.g. `test &#96;example&#96;` => test &#96;example&#96;


# Table

- To add a table, use three or more hyphens (---) to create each column’s header, and use pipes (|) to separate each column.
- For readability sake, add pipes on either side of the table
- To align use colon, add it to the both sides of the hyphens to center align the columns

| name  |  age  |
| :---: | :---: |
| john  |  23   |
| anne  |  24   |


# Collapsible Area

Use HTML to make collapsible areas:

<details>
  <summary>Title</summary>
  Collapsible area insides
</details>

```markdown
<details>
  <summary>Title</summary>
  Collapsible area insides
</details>
```


# Task List

'x' inside completed tasks' brackets, and space inside to do tasks

- [x] completed task
- [ ] to do task

```markdown
- [x] completed task
- [ ] to do task
```


# CSS

- Inline CSS `<p style="color: red;">test</p>`
- Link to a file `<link href="./style.css" rel="stylesheet">`
- Inside a style block:

```html
<style>
  h1 {
    color: red;
  }
</style>
```