# Chapter 3: HTML Headings and Paragraphs

## Learning Objectives

After completing this chapter, you will be able to:

- Understand HTML headings
- Create paragraphs
- Use line breaks and horizontal lines
- Write well-structured content
- Follow best practices for headings

---

# HTML Headings

Headings define the titles and subtitles of a webpage.

HTML provides **six heading levels**.

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

Output:

```
Heading 1
 Heading 2
  Heading 3
   Heading 4
    Heading 5
     Heading 6
```

---

# Heading Levels

| Tag | Purpose |
|------|---------|
| `<h1>` | Main heading |
| `<h2>` | Section heading |
| `<h3>` | Subsection |
| `<h4>` | Smaller heading |
| `<h5>` | Minor heading |
| `<h6>` | Smallest heading |

---

# Best Practice

Use only **one `<h1>`** per page.

Example:

```html
<h1>TechVidyalaya</h1>

<h2>Java Course</h2>

<h2>Python Course</h2>

<h3>Course Duration</h3>
```

---

# HTML Paragraph

The `<p>` tag is used to display paragraphs.

Example:

```html
<p>HTML is the foundation of web development.</p>
```

Output:

```
HTML is the foundation of web development.
```

---

# Multiple Paragraphs

```html
<p>Welcome to HTML.</p>

<p>This is the second paragraph.</p>

<p>Practice every day.</p>
```

Output:

```
Welcome to HTML.

This is the second paragraph.

Practice every day.
```

---

# HTML Ignores Extra Spaces

HTML automatically removes multiple spaces.

Example:

```html
<p>Hello          Students</p>
```

Output:

```
Hello Students
```

---

# HTML Ignores Multiple Lines

```html
<p>
Welcome
to
HTML
Course
</p>
```

Output:

```
Welcome to HTML Course
```

---

# Line Break

The `<br>` tag inserts a line break.

Example:

```html
<p>
Hello<br>
Welcome<br>
Students
</p>
```

Output:

```
Hello
Welcome
Students
```

---

# Horizontal Line

The `<hr>` tag creates a horizontal line.

Example:

```html
<h2>About</h2>

<p>Learn HTML Basics.</p>

<hr>

<h2>Contact</h2>

<p>Email us anytime.</p>
```

Output:

```
About
Learn HTML Basics.
----------------------
Contact
Email us anytime.
```

---

# Combining Headings and Paragraphs

```html
<h1>TechVidyalaya</h1>

<p>Welcome to our learning platform.</p>

<h2>Courses</h2>

<p>Java, Python and Web Development.</p>

<h2>Contact</h2>

<p>contact@techvidyalaya.com</p>
```

---

# Real-World Example

```html
<h1>Online Book Store</h1>

<p>Find thousands of books online.</p>

<h2>Programming</h2>

<p>Java, Python, HTML, CSS.</p>

<h2>Data Science</h2>

<p>Machine Learning and AI.</p>
```

---

# Common Mistakes

### Using Multiple `<h1>` Tags

```html
<h1>Home</h1>

<h1>Products</h1>
```

Better:

```html
<h1>Home</h1>

<h2>Products</h2>
```

---

### Using Headings for Styling

Incorrect:

```html
<h3>This text is small.</h3>
```

Use headings only for document structure, not for changing text size.

---

# Best Practices

- Use one `<h1>` per page.
- Maintain a logical heading hierarchy.
- Use paragraphs for normal text.
- Use `<br>` only for line breaks, not spacing.
- Use `<hr>` to separate sections when appropriate.

---

# Quick Summary

- HTML provides six heading levels.
- `<h1>` is the most important heading.
- `<p>` creates paragraphs.
- `<br>` inserts a new line.
- `<hr>` creates a horizontal divider.
- HTML ignores extra spaces and blank lines.

---

# Key Terms

| Term | Description |
|------|-------------|
| Heading | Title of a section |
| Paragraph | Block of text |
| `<br>` | Line break |
| `<hr>` | Horizontal line |
| Hierarchy | Order of headings |

---

# Practice Questions

### Multiple Choice

**1. Which tag represents the main heading?**

A. `<h6>`

B. `<h3>`

C. `<h1>`

D. `<head>`

**Answer:** C

---

**2. Which tag creates a paragraph?**

A. `<para>`

B. `<p>`

C. `<text>`

D. `<body>`

**Answer:** B

---

**3. Which tag inserts a line break?**

A. `<hr>`

B. `<br>`

C. `<lb>`

D. `<line>`

**Answer:** B

---

# Short Answer Questions

1. What is the purpose of HTML headings?
2. Why should a webpage have only one `<h1>` tag?
3. What does the `<p>` tag do?
4. What is the difference between `<br>` and `<hr>`?
5. How does HTML handle extra spaces?

---

# Hands-on Exercise

Create a webpage that contains:

- One `<h1>` heading
- Two `<h2>` headings
- Three paragraphs
- One line break using `<br>`
- One horizontal line using `<hr>`

Open the webpage in your browser and observe the output.

---

# Interview Questions

### Q1. How many heading tags are available in HTML?

HTML provides six heading tags: `<h1>` to `<h6>`.

---

### Q2. What is the difference between `<h1>` and `<p>`?

`<h1>` is used for the main heading of a webpage, while `<p>` is used to display paragraph text.

---

### Q3. What is the purpose of the `<br>` tag?

The `<br>` tag inserts a single line break without starting a new paragraph.

---

## Chapter Summary

In this chapter, you learned:

- How to use HTML headings
- How to create paragraphs
- The purpose of `<br>` and `<hr>`
- The importance of heading hierarchy
- Best practices for structuring webpage content

In the next chapter, we will learn about **HTML Text Formatting**.
