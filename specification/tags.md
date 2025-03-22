# Tags specification for Dalet v1.0-preview

## 0. Element

| Property | Description |
| -------- | ----------- |
| name     | el          |
| id       | 0           |
| body     | text, tags  |
| argument | no          |

Most primitive tag. Also used if no tag is specified.

**DaletMark example**:

```DaletMark
el: I am Element
el [
  h1: I am first level heading
]
- Element also used with `- text` syntax.
```

## 1. Heading

| Property | Description        |
| -------- | ------------------ |
| name     | h                  |
| id       | 1                  |
| body     | text               |
| argument | int x; 1 <= x <= 6 |

Heading is used for text formatting.

**DaletMark example**:

```DaletMark
h1: Dalet
h2: DaletMark
h3: High level
h2: DaletPack
h3: Low level
```

## 2. Paragraph

| Property | Description |
| -------- | ----------- |
| name     | p           |
| id       | 2           |
| body     | text, tags  |
| argument | no          |

Paragraph is used for text formatting.

**DaletMark example**:

```DaletMark
p: This is a paragraph
{- Paragraph also used with this custom syntax }
```

## 3. Line break

| Property | Description |
| -------- | ----------- |
| name     | br          |
| id       | 3           |
| body     | no          |
| argument | no          |

Line break is used to insert a line break into the text.

**DaletMark example**:

```DaletMark
br
```

## 4. Unordered list

| Property | Description |
| -------- | ----------- |
| name     | ul          |
| id       | 4           |
| body     | tags        |
| argument | no          |

Unordered list is used to create a list.

**DaletMark example**:

```DaletMark
ul [
  - Item 1
  - Item 2
]
```

## 5. Ordered list

| Property | Description |
| -------- | ----------- |
| name     | ol          |
| id       | 5           |
| body     | tags        |
| argument | no          |

Ordered list is used to create a list with increasing numbers.

**DaletMark example**:

```DaletMark
ol [
  - Item
  - Item
  - Item
]
```

## 6. Row

| Property | Description                  |
| -------- | ---------------------------- |
| name     | row                          |
| id       | 6                            |
| body     | tags                         |
| argument | optional; start, center, end |

Splits the text into rows. The alignment argument specifies how the items inside the row are aligned horizontally. By default it is aligned to the start.
**DaletMark example**:

```DaletMark
row [
  - Left
  - Right
]

row "start" [
  - Left
  - Right
]
```

## 7. Link

| Property | Description |
| -------- | ----------- |
| name     | link        |
| id       | 7           |
| body     | any         |
| argument | text        |

Link to other sites. On click the link opens in new tab.

**DaletMark example**:

```DaletMark
link "https://example.com": I am Link
```

## 8. Navlink

| Property | Description |
| -------- | ----------- |
| name     | navlink     |
| id       | 8           |
| body     | any         |
| argument | text        |

Link to the same site. On click the link opens in current tab.

**DaletMark example**:

```DaletMark
navlink "/specification": I am Navlink
```

## 9. Button

| Property | Description |
| -------- | ----------- |
| name     | btn         |
| id       | 9           |
| body     | any         |
| argument | text        |

Same as link, but with button style.

**DaletMark example**:

```DaletMark
btn "https://example.com": I am Button
```

## 10. NavButton

| Property | Description |
| -------- | ----------- |
| name     | navbtn      |
| id       | 9           |
| body     | any         |
| argument | text        |

Same as navlink, but with button style.

**DaletMark example**:

```DaletMark
navbtn "https://example.com": I am NavButton
```

## 11. Image

| Property | Description |
| -------- | ----------- |
| name     | img         |
| id       | 11          |
| body     | no          |
| argument | text        |

Displays an image.

**DaletMark example**:

```DaletMark
img "/dalet.png"
```

## 12. Table

| Property | Description |
| -------- | ----------- |
| name     | table       |
| id       | 12          |
| body     | tags        |
| argument | no          |

Creates a table.

**DaletMark example**:

```DaletMark
{> table
  [ Name | Age ]
  [ Elon | 53  ]
}

table [
    tprow [
        - Name
        - Age
    ]
    trow [
        - Elon
        - 53
    ]
]
```

## 13. Table Row

| Property | Description |
| -------- | ----------- |
| name     | trow        |
| id       | 13          |
| body     | tags        |
| argument | no          |

Creates a table row.

**DaletMark example**:

```DaletMark
trow [
  - Name
  - Age
]
```

## 14. Table Primary Row

| Property | Description |
| -------- | ----------- |
| name     | tprow       |
| id       | 14          |
| body     | tags        |
| argument | no          |

Like table row, but with primary background.

**DaletMark example**:

```DaletMark
tprow [
  - Name
  - Age
]
```

## 15. Horizontal rule

| Property | Description |
| -------- | ----------- |
| name     | hr          |
| id       | 15          |
| body     | no          |
| argument | no          |

Creates a horizontal rule.

**DaletMark example**:

```DaletMark
hr
```

## 16. Bold

| Property | Description |
| -------- | ----------- |
| name     | b           |
| id       | 16          |
| body     | text        |
| argument | no          |

Creates **bold** text.

**DaletMark example**:

```DaletMark
b: I am Bold
```

## 17. Italic

| Property | Description |
| -------- | ----------- |
| name     | i           |
| id       | 17          |
| body     | text        |
| argument | no          |

Creates _italic_ text.

**DaletMark example**:

```DaletMark
i: I am Italic
```

## 18. Blockquote

| Property | Description |
| -------- | ----------- |
| name     | bq          |
| id       | 18          |
| body     | text, tags  |
| argument | no          |

Creates a blockquote.

**DaletMark example**:

```DaletMark
bq: I am Blockquote
```

## 19. Footnote Link

| Property | Description  |
| -------- | ------------ |
| name     | footlnk      |
| id       | 19           |
| body     | no           |
| argument | text, number |

Link to footnote.

**DaletMark example**:

```DaletMark
footlnk 1
```

## 20. Footnote

| Property | Description  |
| -------- | ------------ |
| name     | footn        |
| id       | 20           |
| body     | text         |
| argument | text, number |

Creates footnote.

**DaletMark example**:

```DaletMark
footn 1: I am Footnote
```

## 21. Anchor

| Property | Description  |
| -------- | ------------ |
| name     | a            |
| id       | 21           |
| body     | no           |
| argument | text, number |

Creates anchor. Like `<a href="#argument"></a>` in HTML.

**DaletMark example**:

```DaletMark
a0
```

## 22. Strikethrough

| Property | Description |
| -------- | ----------- |
| name     | s           |
| id       | 22          |
| body     | text        |
| argument | no          |

Creates ~~strikethrough~~ text.

**DaletMark example**:

```DaletMark
s: I am Strikethrough
```

## 23. Superscript

| Property | Description |
| -------- | ----------- |
| name     | sup         |
| id       | 23          |
| body     | text        |
| argument | no          |

Creates ^superscript^ text.

**DaletMark example**:

```DaletMark
sup: I am Superscript
```

## 24. Subscript

| Property | Description |
| -------- | ----------- |
| name     | sub         |
| id       | 24          |
| body     | text        |
| argument | no          |

Creates ~subscript~ text.

**DaletMark example**:

```DaletMark
sub: I am Subscript
```

## 25. Disclosure

| Property | Description |
| -------- | ----------- |
| name     | disc        |
| id       | 25          |
| body     | text, tags  |
| argument | text        |

Creates disclosure element.

**DaletMark example**:

```DaletMark
disc "Click to expand": I am Disclosure
```

## 26. Block

| Property | Description                  |
| -------- | ---------------------------- |
| name     | block                        |
| id       | 26                           |
| body     | text, tags                   |
| argument | optional; start, center, end |

Creates block element. Can be used for horizontal aligning. By default aligned to center.

**DaletMark example**:

```DaletMark
block: I am Block
```

Argument converts to numbers in DaletPack.

start -> 0
end -> 1

## 27. Carousel

| Property | Description |
| -------- | ----------- |
| name     | carousel    |
| id       | 27          |
| body     | tags        |
| argument | no          |

Creates carousel.

**DaletMark example**:

```DaletMark
carousel [
  - Example 1
  - Example 2
]
```

## 28. Code

| Property | Description    |
| -------- | -------------- |
| name     | code           |
| id       | 28             |
| body     | text           |
| argument | optional; text |

Creates code block.

**DaletMark example**:

```DaletMark
code "js": let code = "js"
```

## 29. Pre-formatted text

| Property | Description |
| -------- | ----------- |
| name     | pre         |
| id       | 29          |
| body     | text        |
| argument | no          |

Creates pre formatted text block. Like code but without style and highlight.

**DaletMark example**:

```DaletMark
pre: I am pre
```

## 30. Metadata

| Property | Description |
| -------- | ----------- |
| name     | meta        |
| id       | 30          |
| body     | text        |
| argument | text        |

Not displayed. Specifies metadata such as title, description. Must be before all tags if specified.

**DaletMark example**:

```DaletMark
meta "description": I am description
```
