# Chapter 4: HTML Text Formatting

## Learning Objectives

After completing this chapter, you will be able to:

- Format text using HTML tags
- Make text bold, italic, and underlined
- Highlight important text
- Display superscript and subscript
- Write semantic HTML for better accessibility

---

# What is Text Formatting?

HTML provides formatting tags to change the appearance and meaning of text.

Text formatting improves:

- Readability
- User experience
- Accessibility
- SEO

---

# Bold Text

Use the `<b>` tag to display bold text.

```html
<p>This is <b>bold</b> text.</p>
```

Output:

```
This is bold text.
```

---

# Strong Text

The `<strong>` tag indicates that the text is important.

```html
<p>Please <strong>read carefully</strong>.</p>
```

Output:

```
Please read carefully.
```

> **Note:** Browsers usually display `<strong>` as bold, but it also conveys importance to search engines and screen readers.

---

# Italic Text

Use the `<i>` tag to display italic text.

```html
<p>This is <i>italic</i> text.</p>
```

Output:

```
This is italic text.
```

---

# Emphasized Text

The `<em>` tag adds emphasis to text.

```html
<p>This is <em>important</em>.</p>
```

Output:

```
This is important.
```

> **Note:** `<em>` usually appears in italics but also provides semantic meaning.

---

# Underlined Text

Use the `<u>` tag to underline text.

```html
<p>This is <u>underlined</u> text.</p>
```

Output:

```
This is underlined text.
```

---

# Highlighted Text

The `<mark>` tag highlights text.

```html
<p>Learn <mark>HTML</mark> first.</p>
```

Output:

```
Learn HTML first.
```

---

# Small Text

The `<small>` tag displays smaller text.

```html
<p>This is <small>small text</small>.</p>
```

Output:

```
This is small text.
```

---

# Deleted Text

The `<del>` tag represents deleted text.

```html
<p>Price: <del>£100</del> £80</p>
```

Output:

```
Price: ~~£100~~ £80
```

---

# Inserted Text

The `<ins>` tag represents inserted text.

```html
<p><ins>New Feature Added</ins></p>
```

Output:

```
New Feature Added
```

---

# Subscript

The `<sub>` tag displays text below the normal line.

Example:

```html
<p>H<sub>2</sub>O</p>
```

Output:

```
H₂O
```

---

# Superscript

The `<sup>` tag displays text above the normal line.

Example:

```html
<p>x<sup>2</sup></p>
```

Output:

```
x²
```

---

# Combining Formatting Tags

```html
<p>
<b>Bold</b>,
<i>Italic</i>,
<u>Underline</u>,
<mark>Highlight</mark>
</p>
```

---

# Real-World Example

```html
<h2>Course Details</h2>

<p>
<strong>Course:</strong> Full Stack Java
</p>

<p>
Duration: <mark>6 Months</mark>
</p>

<p>
Fees:
<del>£500</del>
<strong>£350</strong>
</p>

<p>
Certificate Available <sup>*</sup>
</p>
```

---

# Semantic vs Visual Tags

| Visual Tag | Semantic Tag | Purpose |
|------------|--------------|---------|
| `<b>` | `<strong>` | Important text |
| `<i>` | `<em>` | Emphasized text |

Prefer semantic tags because they improve accessibility and SEO.

---

# Best Practices

- Use `<strong>` instead of `<b>` when text is important.
- Use `<em>` instead of `<i>` when emphasis is intended.
- Avoid excessive formatting.
- Use formatting only where it adds meaning.
- Keep content easy to read.

---

# Quick Summary

- `<b>` makes text bold.
- `<strong>` marks important text.
- `<i>` displays italic text.
- `<em>` adds emphasis.
- `<u>` underlines text.
- `<mark>` highlights text.
- `<sub>` creates subscript.
- `<sup>` creates superscript.

---

# Key Terms

| Term | Description |
|------|-------------|
| Bold | Thick text |
| Italic | Slanted text |
| Highlight | Marked text |
| Subscript | Text below baseline |
| Superscript | Text above baseline |
| Semantic Tag | Tag that provides meaning |

---

# Practice Questions

### Multiple Choice

**1. Which tag is used for important text?**

A. `<b>`

B. `<strong>`

C. `<u>`

D. `<i>`

**Answer:** B

---

**2. Which tag highlights text?**

A. `<mark>`

B. `<small>`

C. `<del>`

D. `<sub>`

**Answer:** A

---

**3. Which tag is used for superscript?**

A. `<sub>`

B. `<sup>`

C. `<small>`

D. `<mark>`

**Answer:** B

---

# Short Answer Questions

1. What is the difference between `<b>` and `<strong>`?
2. When should `<em>` be used instead of `<i>`?
3. What is the purpose of the `<mark>` tag?
4. Explain the use of `<sub>` with an example.
5. Explain the use of `<sup>` with an example.

---

# Hands-on Exercise

Create a webpage containing:

- Bold text
- Strong text
- Italic text
- Emphasized text
- Underlined text
- Highlighted text
- Deleted text
- Inserted text
- H₂O using subscript
- x² using superscript

Run the webpage and observe the formatting.

---

# Interview Questions

### Q1. What is the difference between `<b>` and `<strong>`?

`<b>` only changes the appearance of text, while `<strong>` indicates that the text is important and provides semantic meaning.

---

### Q2. Why should semantic formatting tags be preferred?

Semantic tags improve accessibility, help search engines understand content, and make HTML more meaningful.

---

### Q3. Give examples of subscript and superscript.

- Subscript: `H<sub>2</sub>O` → H₂O
- Superscript: `x<sup>2</sup>` → x²

---

## Chapter Summary

In this chapter, you learned:

- How to format text using HTML
- The difference between visual and semantic formatting tags
- How to highlight, underline, and emphasise text
- How to display subscript and superscript
- Best practices for writing accessible and meaningful HTML

In the next chapter, we will learn about **HTML Links**.
