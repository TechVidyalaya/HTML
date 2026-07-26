# Chapter 7: HTML Lists

## Learning Objectives

After completing this chapter, you will be able to:

- Understand HTML lists
- Create ordered and unordered lists
- Create description lists
- Create nested lists
- Choose the correct list type for different scenarios
- Follow best practices when using lists

---

# What are HTML Lists?

Lists are used to display related items in an organised way.

HTML provides three types of lists:

- Unordered List
- Ordered List
- Description List

---

# Types of HTML Lists

| List Type | Tag | Purpose |
|-----------|-----|---------|
| Unordered List | `<ul>` | Displays bullet points |
| Ordered List | `<ol>` | Displays numbered items |
| Description List | `<dl>` | Displays terms and descriptions |

---

# Unordered List

An unordered list displays items using bullets.

Syntax:

```html
<ul>
    <li>Java</li>
    <li>Python</li>
    <li>HTML</li>
</ul>
```

Output:

```
• Java
• Python
• HTML
```

---

# List Item

Each item inside a list is created using the `<li>` tag.

Example:

```html
<ul>

    <li>Apple</li>

    <li>Banana</li>

    <li>Mango</li>

</ul>
```

---

# Ordered List

An ordered list displays items in sequence.

```html
<ol>

    <li>Register</li>

    <li>Login</li>

    <li>Start Learning</li>

</ol>
```

Output:

```
1. Register
2. Login
3. Start Learning
```

---

# Changing the Numbering Type

### Uppercase Letters

```html
<ol type="A">

    <li>Java</li>

    <li>Python</li>

</ol>
```

Output:

```
A. Java
B. Python
```

---

### Lowercase Letters

```html
<ol type="a">

    <li>Java</li>

    <li>Python</li>

</ol>
```

---

### Roman Numbers

```html
<ol type="I">

    <li>Introduction</li>

    <li>Basics</li>

</ol>
```

Output:

```
I.
II.
```

---

### Lowercase Roman Numbers

```html
<ol type="i">

    <li>Chapter One</li>

    <li>Chapter Two</li>

</ol>
```

---

# Starting from a Different Number

Use the `start` attribute.

```html
<ol start="5">

    <li>Arrays</li>

    <li>Collections</li>

</ol>
```

Output:

```
5. Arrays
6. Collections
```

---

# Reversed Ordered List

Use the `reversed` attribute.

```html
<ol reversed>

    <li>Third</li>

    <li>Second</li>

    <li>First</li>

</ol>
```

Output:

```
3.
2.
1.
```

---

# Description List

A description list displays terms and their descriptions.

Tags used:

- `<dl>` → Description List
- `<dt>` → Description Term
- `<dd>` → Description Description

Example:

```html
<dl>

    <dt>HTML</dt>

    <dd>Markup language for webpages.</dd>

    <dt>CSS</dt>

    <dd>Styles webpages.</dd>

</dl>
```

Output:

```
HTML
    Markup language for webpages.

CSS
    Styles webpages.
```

---

# Nested Lists

Lists can be placed inside other lists.

Example:

```html
<ul>

    <li>Programming

        <ul>

            <li>Java</li>

            <li>Python</li>

        </ul>

    </li>

    <li>Database</li>

</ul>
```

Output:

```
• Programming
    • Java
    • Python

• Database
```

---

# Real-World Example

```html
<h2>TechVidyalaya Courses</h2>

<ul>

    <li>Java Full Stack</li>

    <li>Python</li>

    <li>Web Development</li>

    <li>Data Structures</li>

</ul>
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML Lists</title>
</head>

<body>

<h1>Programming Languages</h1>

<ul>

    <li>Java</li>

    <li>Python</li>

    <li>JavaScript</li>

</ul>

<h2>Learning Steps</h2>

<ol>

    <li>Learn HTML</li>

    <li>Learn CSS</li>

    <li>Learn JavaScript</li>

</ol>

</body>

</html>
```

---

# Common Mistakes

### Using `<li>` Outside a List

Incorrect:

```html
<li>Java</li>
```

Correct:

```html
<ul>

    <li>Java</li>

</ul>
```

---

### Forgetting Closing Tags

Incorrect:

```html
<ul>

<li>Java

<li>Python

</ul>
```

Correct:

```html
<ul>

    <li>Java</li>

    <li>Python</li>

</ul>
```

---

# Best Practices

- Choose the correct list type.
- Use meaningful list items.
- Keep nesting to a reasonable level.
- Indent nested lists properly.
- Close all list tags correctly.

---

# Quick Summary

- `<ul>` creates a bullet list.
- `<ol>` creates a numbered list.
- `<li>` represents a list item.
- `<dl>` creates a description list.
- Lists can be nested.
- Ordered lists support numbering styles.

---

# Key Terms

| Term | Description |
|------|-------------|
| List | Collection of related items |
| Unordered List | Bullet list |
| Ordered List | Numbered list |
| Description List | List of terms and definitions |
| Nested List | List inside another list |

---

# Practice Questions

### Multiple Choice

**1. Which tag creates a bullet list?**

A. `<ol>`

B. `<ul>`

C. `<dl>`

D. `<li>`

**Answer:** B

---

**2. Which tag represents an individual list item?**

A. `<dt>`

B. `<li>`

C. `<dd>`

D. `<item>`

**Answer:** B

---

**3. Which tag is used for a description list?**

A. `<ol>`

B. `<ul>`

C. `<dl>`

D. `<li>`

**Answer:** C

---

# Short Answer Questions

1. What is the difference between an ordered list and an unordered list?
2. What is the purpose of the `<li>` tag?
3. Explain the use of the `start` attribute.
4. What is a nested list?
5. When should you use a description list?

---

# Hands-on Exercise

Create a webpage containing:

- An unordered list of your favourite programming languages
- An ordered list of steps to build a webpage
- A description list of HTML, CSS, and JavaScript
- A nested list of courses and their topics

Run the webpage and verify the output.

---

# Interview Questions

### Q1. What are the different types of lists available in HTML?

HTML provides three types of lists:

- Unordered List (`<ul>`)
- Ordered List (`<ol>`)
- Description List (`<dl>`)

---

### Q2. What is the purpose of the `<li>` tag?

The `<li>` tag defines an individual item inside an ordered or unordered list.

---

### Q3. Can HTML lists be nested?

Yes. An ordered or unordered list can be placed inside another list item to create a hierarchical structure.

---

## Chapter Summary

In this chapter, you learned:

- The different types of HTML lists
- How to create ordered, unordered, and description lists
- How to customise ordered list numbering
- How to create nested lists
- Best practices for writing clean and organised HTML lists

In the next chapter, we will learn about **HTML Tables**.
