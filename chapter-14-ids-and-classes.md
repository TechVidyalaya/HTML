# Chapter 14: HTML IDs and Classes

## Learning Objectives

After completing this chapter, you will be able to:

- Understand IDs and Classes
- Differentiate between IDs and Classes
- Apply IDs and Classes to HTML elements
- Use IDs for navigation
- Prepare HTML for CSS and JavaScript
- Follow best practices

---

# What are IDs and Classes?

IDs and Classes are attributes used to identify HTML elements.

They are mainly used for:

- CSS styling
- JavaScript manipulation
- Page navigation
- Organising HTML elements

---

# ID Attribute

The `id` attribute uniquely identifies an HTML element.

Syntax:

```html
<h1 id="title">Welcome</h1>
```

Each ID should be **unique** within a webpage.

---

# Example of an ID

```html
<h2 id="about">About Us</h2>

<p>Welcome to TechVidyalaya.</p>
```

---

# Class Attribute

The `class` attribute groups multiple elements together.

Syntax:

```html
<p class="course">Java</p>

<p class="course">Python</p>

<p class="course">HTML</p>
```

All three paragraphs belong to the same class.

---

# Difference Between ID and Class

| ID | Class |
|----|-------|
| Unique | Can be reused |
| One element only | Multiple elements |
| Uses `id` | Uses `class` |
| CSS selector: `#id` | CSS selector: `.class` |

---

# Using Multiple Classes

An element can have multiple classes.

```html
<p class="course active">

Java Full Stack

</p>
```

---

# Using IDs for Bookmarks

IDs can be used to jump to a section of the webpage.

```html
<h2 id="contact">

Contact Us

</h2>
```

Link:

```html
<a href="#contact">

Go to Contact

</a>
```

---

# IDs with JavaScript

JavaScript can access an element using its ID.

```html
<p id="message">

Welcome

</p>
```

Example:

```javascript
document.getElementById("message");
```

---

# Classes with JavaScript

JavaScript can access all elements with the same class.

```html
<p class="course">Java</p>

<p class="course">Python</p>
```

Example:

```javascript
document.getElementsByClassName("course");
```

---

# IDs and CSS

Example:

```html
<h1 id="title">

Welcome

</h1>
```

CSS:

```css
#title {
    color: blue;
}
```

---

# Classes and CSS

HTML:

```html
<p class="highlight">

Important Note

</p>
```

CSS:

```css
.highlight {
    background-color: yellow;
}
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>

<title>ID and Class Example</title>

<style>

#title {
    color: blue;
}

.course {
    color: green;
}

</style>

</head>

<body>

<h1 id="title">

TechVidyalaya

</h1>

<p class="course">

Java

</p>

<p class="course">

Python

</p>

<p class="course">

HTML

</p>

</body>

</html>
```

---

# Naming Conventions

Good IDs:

```html
id="header"

id="studentForm"

id="footer"
```

Good Classes:

```html
class="button"

class="menu"

class="highlight"
```

Avoid:

```html
id="123"

class="###"

id="abc!"
```

---

# Common Mistakes

### Duplicate IDs

Incorrect:

```html
<h1 id="title">

Welcome

</h1>

<h2 id="title">

Courses

</h2>
```

Correct:

```html
<h1 id="title">

Welcome

</h1>

<h2 id="courses">

Courses

</h2>
```

---

### Using IDs Instead of Classes

Incorrect:

```html
<p id="course">Java</p>

<p id="course">Python</p>
```

Correct:

```html
<p class="course">Java</p>

<p class="course">Python</p>
```

---

# Best Practices

- Keep IDs unique.
- Use classes for reusable styling.
- Choose meaningful names.
- Avoid spaces in IDs and class names.
- Use lowercase and hyphens or camelCase consistently.

---

# Quick Summary

- `id` uniquely identifies an element.
- `class` groups multiple elements.
- IDs are used once per page.
- Classes can be reused.
- Both are commonly used with CSS and JavaScript.

---

# Key Terms

| Term | Description |
|------|-------------|
| ID | Unique identifier for an element |
| Class | Reusable group identifier |
| CSS Selector | Targets HTML elements for styling |
| JavaScript Selector | Finds HTML elements dynamically |

---

# Practice Questions

### Multiple Choice

**1. Which attribute should be unique on a webpage?**

A. class

B. id

C. name

D. value

**Answer:** B

---

**2. Which CSS selector is used for a class?**

A. `#`

B. `.`

C. `@`

D. `*`

**Answer:** B

---

**3. Which attribute can be shared by multiple elements?**

A. id

B. class

C. href

D. src

**Answer:** B

---

# Short Answer Questions

1. What is the purpose of the `id` attribute?
2. What is the difference between `id` and `class`?
3. Why should IDs be unique?
4. When should you use a class instead of an ID?
5. How are IDs used for bookmarks?

---

# Hands-on Exercise

Create a webpage with:

- A heading using an ID
- Three paragraphs using the same class
- A bookmark link that jumps to the footer
- CSS styling for both the ID and the class

Run the webpage and verify the output.

---

# Interview Questions

### Q1. What is the difference between an ID and a class?

An ID uniquely identifies a single HTML element, while a class can be assigned to multiple elements for shared styling or behaviour.

---

### Q2. Why are IDs commonly used in JavaScript?

IDs uniquely identify elements, making it easy to access and manipulate a specific element using methods such as `document.getElementById()`.

---

### Q3. Can an HTML element have multiple classes?

Yes. An element can belong to multiple classes by separating class names with spaces.

Example:

```html
<p class="course active">
    Java Full Stack
</p>
```

---

## Chapter Summary

In this chapter, you learned:

- What IDs and Classes are
- The differences between them
- How to use IDs for unique elements
- How to use Classes for reusable styling
- How IDs and Classes work with CSS and JavaScript
- Best practices for naming and using IDs and Classes

In the next chapter, we will learn about **HTML Iframes**.
