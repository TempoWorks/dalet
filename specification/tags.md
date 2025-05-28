# Tags specification for Dalet v1.0-preview

## Element

Default element without styles.

| Property | Allowed types |
| -------- | ------------- |
| body     | text, tags    |

**DaletMark example**:

```daletmark
todo
```

## Heading

Bold, big text with vertical margin.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |
| heading  | HeadingLevel  |

**DaletMark example**:

```daletmark
todo
```

## Paragraph

Paragraph with vertical margin.

| Property | Allowed types |
| -------- | ------------- |
| body     | text, tags    |

**DaletMark example**:

```daletmark
todo
```

## Link

Link to another resource. Opens in new tab.

| Property | Allowed types      |
| -------- | ------------------ |
| body     | Optional text/tags |
| dref     | text               |

**DaletMark example**:

```daletmark
todo
```

## NavLink

Link to another resource. Opens in current tab.

| Property | Allowed types      |
| -------- | ------------------ |
| body     | Optional text/tags |
| dref     | text               |

**DaletMark example**:

```daletmark
todo
```

## Button

Link to another resource with button style. Opens in new tab.

| Property | Allowed types      |
| -------- | ------------------ |
| body     | Optional text/tags |
| dref     | text               |

**DaletMark example**:

```daletmark
todo
```

## NavButton

Link to another resource with button style. Opens in current tab.

| Property | Allowed types      |
| -------- | ------------------ |
| body     | Optional text/tags |
| dref     | text               |

**DaletMark example**:

```daletmark
todo
```

## Image

Image with optional alt text.

| Property | Allowed types |
| -------- | ------------- |
| src      | text          |
| alt      | Optional text |

**DaletMark example**:

```daletmark
todo
```

## Table

Table element.

| Property | Allowed types |
| -------- | ------------- |
| body     | TableRows     |

**DaletMark example**:

```daletmark
todo
```

## List

List with custom marker style.

| Property | Allowed types |
| -------- | ------------- |
| body     | tags          |
| style    | ListStyle     |

**DaletMark example**:

```daletmark
todo
```

## Bold

Bold text.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |

**DaletMark example**:

```daletmark
todo
```

## Italic

Italic text.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |

**DaletMark example**:

```daletmark
todo
```

## Strikethrough

Strikethrough text.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |

**DaletMark example**:

```daletmark
todo
```

## Superscript

Superscript text.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |

**DaletMark example**:

```daletmark
todo
```

## Subscript

Subscript text.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |

**DaletMark example**:

```daletmark
todo
```

## Mono

Monospace text.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |

**DaletMark example**:

```daletmark
todo
```

## FootLink

Link to a footnote.

| Property | Allowed types |
| -------- | ------------- |
| footnote | u64           |

**DaletMark example**:

```daletmark
todo
```

## FootNote

Footnote content.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |
| footnote | u64           |

**DaletMark example**:

```daletmark
todo
```

## Anchor

Anchor for links.

| Property | Allowed types |
| -------- | ------------- |
| id       | text          |

**DaletMark example**:

```daletmark
todo
```

## BlockQuote

Blockquote element.

| Property | Allowed types |
| -------- | ------------- |
| body     | text, tags    |

**DaletMark example**:

```daletmark
todo
```

## Code

Code block with syntax highlighting.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |
| language | Optional text |

**DaletMark example**:

```daletmark
todo
```

## InlineCode

Inline code with syntax highlighting.

| Property | Allowed types |
| -------- | ------------- |
| body     | text          |
| language | Optional text |

**DaletMark example**:

```daletmark
todo
```

## Block

Block with lighter background and padding.

| Property | Allowed types |
| -------- | ------------- |
| body     | tags          |

**DaletMark example**:

```daletmark
todo
```

## Flex

Flex container.

| Property | Allowed types  |
| -------- | -------------- |
| body     | tags           |
| wrap     | bool           |
| align_x  | Optional Align |
| align_y  | Optional Align |

**DaletMark example**:

```daletmark
todo
```

## Grid

Grid container.

| Property | Allowed types  |
| -------- | -------------- |
| body     | tags           |
| align_x  | Optional Align |
| align_y  | Optional Align |

**DaletMark example**:

```daletmark
todo
```

## Disclosure

Collapsible block with optional title.

| Property | Allowed types |
| -------- | ------------- |
| body     | text, tags    |
| title    | Optional text |

**DaletMark example**:

```daletmark
todo
```

## Carousel

Carousel of blocks with navigation buttons.

| Property | Allowed types |
| -------- | ------------- |
| body     | tags          |

**DaletMark example**:

```daletmark
todo
```

## Variable

Displays variable from page context.

| Property | Allowed types |
| -------- | ------------- |
| idx      | u64           |

**DaletMark example**:

```daletmark
todo
```

## HorizontalBreak

Horizontal line divider.

**DaletMark example**:

```daletmark
todo
```
