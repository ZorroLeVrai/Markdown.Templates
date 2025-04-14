---
title: "Markdown Cheat Sheet"
---

# Markdown Cheat Sheet

A quick reference for Markdown syntax.

---

## 1. Headings

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

# H1  
## H2  
### H3  
#### H4  
##### H5  
###### H6  

---

## 2. Emphasis

```markdown
*Italic* or _Italic_

**Bold** or __Bold__

***Bold and italic***

~~Strikethrough~~
```

*Italic*  
**Bold**  
***Bold and italic***  
~~Strikethrough~~

---

## 3. Lists

### Unordered List
```markdown
- Item 1
- Item 2
  - Subitem
* Item 3
```

- Item 1  
- Item 2  
  - Subitem  
* Item 3

### Ordered List
```markdown
1. First
2. Second
3. Third
```

1. First  
2. Second  
3. Third

---

## 4. Links

```markdown
[OpenAI](https://www.openai.com)
```

[OpenAI](https://www.openai.com)

---

## 5. Images

```markdown
![Pythagoras Formula](Pythagore_V1.png)
```

![Pythagoras Formula](Pythagore_V1.png)

---

## 6. Code

### Inline Code
```markdown
Use `console.log()` to debug.
```
Use `console.log()` to debug.

### Block of Code
<pre>
```javascript
function greet(name) {
  return `Hello, ${name}`;
}
```
</pre>

```javascript
function greet(name) {
  return `Hello, ${name}`;
}
```

---

## 7. Blockquotes

```markdown
> This is a quote.
>> Nested quote
```

> This is a quote.  
>> Nested quote

---

## 8. Horizontal Rule

```markdown
---
```

---

## 9. Tables

```markdown
| Name     | Age | City      |
|----------|-----|-----------|
| Alice    | 30  | New York  |
| Bob      | 25  | London    |
```

| Name     | Age | City      |
|----------|-----|-----------|
| Alice    | 30  | New York  |
| Bob      | 25  | London    |

---

## 10. Task Lists

```markdown
- [x] Write documentation
- [ ] Fix bug
- [ ] Commit changes
```

- [x] Write documentation  
- [ ] Fix bug  
- [ ] Commit changes

---

## 11. HTML inside Markdown

```markdown
<b>This is bold using HTML</b>
<details>
<summary>Click to expand</summary>
Hidden content here.
</details>
```

<b>This is bold using HTML</b>  
<details>
<summary>Click to expand</summary>
Hidden content here.
</details>

---

## 12. Footnotes

```markdown
Here's a sentence with a footnote.[^1]

[^1]: This is the footnote.
```

Here's a sentence with a footnote.[^1]

[^1]: This is the footnote.

---

## 13. Emoji (if supported)

```markdown
:rocket: :smile: :coffee:
```

:rocket: :smile: :coffee:

---

## 14. Escaping Characters

Use `\*` to escape special characters like `*`, `#`, etc.

```markdown
\*not italic\*
```

\*not italic\*

---
