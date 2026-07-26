# Chapter 13: HTML Block and Inline Elements

## Learning Objectives

After completing this chapter, you will be able to:

- Understand block and inline elements
- Differentiate between block and inline elements
- Use common block-level elements
- Use common inline elements
- Choose the correct element for different situations
- Follow HTML best practices

---

# What are HTML Elements?

HTML elements are broadly classified into two categories:

- Block Elements
- Inline Elements

Understanding the difference helps create well-structured webpages.

---

# Block Elements

A block element always starts on a new line and occupies the full available width of its parent container.

Example:

```html
<h1>Welcome</h1>

<p>This is a paragraph.</p>

<p>This is another paragraph.</p>
```

Output:

```
Welcome

This is a paragraph.

This is another paragraph.
```

Each element appears on a new line.

---

# Characteristics of Block Elements

- Starts on a new line
- Takes the full available width
- Can contain block and inline elements
- Used to structure webpage layout

---

# Common Block Elements

| Element | Purpose |
|----------|---------|
| `<div>` | Generic container |
| `<h1>`–`<h6>` | Headings |
| `<p>` | Paragraph |
| `<section>` | Content section |
| `<article>` | Independent content |
| `<header>` | Page header |
| `<footer>` | Page footer |
| `<nav>` | Navigation |
| `<main>` | Main content |
| `<aside>` | Sidebar |
| `<form>` | Form |
| `<table>` | Table |
| `<ul>` | Unordered list |
| `<ol>` | Ordered list |

---

# Example of Block Elements

```html
<div>

<h2>Java Course</h2>

<p>Learn Java from scratch.</p>

</div>
```

---

# Inline Elements

Inline elements do not start on a new line.

They occupy only the space required by their content.

Example:

```html
<p>

Welcome to <strong>HTML</strong> Tutorial.

</p>
```

Output:

```
Welcome to HTML Tutorial.
```

The text remains on the same line.

---

# Characteristics of Inline Elements

- Does not start on a new line
- Takes only the required width
- Usually contains text or small pieces of content
- Cannot generally contain block elements

---

# Common Inline Elements

| Element | Purpose |
|----------|---------|
| `<span>` | Generic inline container |
| `<a>` | Hyperlink |
| `<img>` | Image |
| `<strong>` | Important text |
| `<em>` | Emphasized text |
| `<b>` | Bold text |
| `<i>` | Italic text |
| `<u>` | Underlined text |
| `<mark>` | Highlighted text |
| `<small>` | Small text |
| `<sub>` | Subscript |
| `<sup>` | Superscript |

---

# Example of Inline Elements

```html
<p>

Learn <strong>HTML</strong>,
<em>CSS</em>,
and <span>JavaScript</span>.

</p>
```

---

# Block vs Inline

| Feature | Block Element | Inline Element |
|----------|---------------|----------------|
| Starts on new line | Yes | No |
| Takes full width | Yes | No |
| Width | Full available width | Content width |
| Used for | Page structure | Formatting content |

---

# The `<div>` Element

The `<div>` element is a generic block-level container.

```html
<div>

<h2>About Us</h2>

<p>Welcome to our website.</p>

</div>
```

It is commonly used for grouping elements and page layout.

---

# The `<span>` Element

The `<span>` element is a generic inline container.

```html
<p>

Welcome to
<span>TechVidyalaya</span>

</p>
```

It is commonly used for styling a specific part of text.

---

# Combining Block and Inline Elements

```html
<div>

<h2>Programming</h2>

<p>

Learn
<strong>HTML</strong>,
<em>CSS</em>,
and JavaScript.

</p>

</div>
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>

<title>Block and Inline</title>

</head>

<body>

<div>

<h1>TechVidyalaya</h1>

<p>

Learn
<strong>HTML</strong>,
<span>CSS</span>,
and JavaScript.

</p>

</div>

</body>

</html>
```

---

# Common Mistakes

### Using Block Elements Inside Inline Elements

Incorrect:

```html
<span>

<div>Hello</div>

</span>
```

Correct:

```html
<div>

<span>Hello</span>

</div>
```

---

### Using `<div>` for Everything

Instead of:

```html
<div>

<div>

<div>

</div>

</div>

</div>
```

Use semantic elements where appropriate:

```html
<header>

<nav>

<main>

<footer>
```

---

# Best Practices

- Use block elements to structure your webpage.
- Use inline elements for small pieces of content.
- Prefer semantic elements over unnecessary `<div>` tags.
- Use `<span>` only when an inline container is needed.
- Keep HTML clean and well organised.

---

# Quick Summary

- Block elements start on a new line.
- Inline elements remain on the same line.
- `<div>` is a block-level container.
- `<span>` is an inline container.
- Semantic elements should be preferred whenever possible.

---

# Key Terms

| Term | Description |
|------|-------------|
| Block Element | Starts on a new line and takes full width |
| Inline Element | Stays on the same line as surrounding content |
| `<div>` | Generic block container |
| `<span>` | Generic inline container |
| Semantic Element | Element with meaningful purpose |

---

# Practice Questions

### Multiple Choice

**1. Which of the following is a block element?**

A. `<span>`

B. `<a>`

C. `<div>`

D. `<strong>`

**Answer:** C

---

**2. Which element is an inline container?**

A. `<section>`

B. `<div>`

C. `<span>`

D. `<article>`

**Answer:** C

---

**3. Which statement is true?**

A. Inline elements always start on a new line.

B. Block elements occupy the full available width.

C. `<span>` is a block element.

D. `<div>` is an inline element.

**Answer:** B

---

# Short Answer Questions

1. What is a block element?
2. What is an inline element?
3. What is the difference between `<div>` and `<span>`?
4. Why should semantic elements be preferred over `<div>`?
5. Give three examples of block elements and three examples of inline elements.

---

# Hands-on Exercise

Create a webpage containing:

- A `<div>` with a heading and paragraph
- A paragraph with bold, italic, and highlighted text
- A hyperlink using the `<a>` tag
- A `<span>` to highlight a single word
- An image displayed inside a paragraph

Observe which elements appear on new lines and which remain inline.

---

# Interview Questions

### Q1. What is the difference between block and inline elements?

Block elements start on a new line and occupy the full available width, while inline elements remain on the same line and occupy only the space required by their content.

---

### Q2. What is the purpose of the `<div>` element?

The `<div>` element is a generic block-level container used to group HTML elements for layout, styling, or scripting.

---

### Q3. When should you use the `<span>` element?

Use the `<span>` element to group or style a small portion of inline content without affecting the document structure.

---

## Chapter Summary

In this chapter, you learned:

- The difference between block and inline elements
- Common examples of each type
- The purpose of `<div>` and `<span>`
- How to combine block and inline elements
- Best practices for writing clean and semantic HTML

In the next chapter, we will learn about **HTML IDs and Classes**.
