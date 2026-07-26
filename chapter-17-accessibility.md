# Chapter 17: HTML Accessibility

## Learning Objectives

After completing this chapter, you will be able to:

- Understand web accessibility
- Learn why accessibility is important
- Use semantic HTML for better accessibility
- Add alternative text to images
- Create accessible forms
- Follow accessibility best practices

---

# What is Accessibility?

**Web Accessibility** means designing websites that everyone can use, including people with disabilities.

Accessibility helps users who have:

- Visual impairments
- Hearing impairments
- Physical disabilities
- Cognitive disabilities

An accessible website provides a better experience for all users.

---

# Why is Accessibility Important?

Accessibility:

- Makes websites usable by everyone
- Improves SEO
- Supports screen readers
- Enhances user experience
- Meets legal and industry standards

---

# Use Semantic HTML

Semantic elements help assistive technologies understand the structure of a webpage.

Example:

```html
<header>
    <h1>TechVidyalaya</h1>
</header>

<nav>
    <a href="#">Home</a>
    <a href="#">Courses</a>
</nav>

<main>
    <article>
        <h2>HTML Basics</h2>
        <p>Learn HTML from scratch.</p>
    </article>
</main>

<footer>
    Copyright © 2026
</footer>
```

---

# Add Alternative Text to Images

Always provide the `alt` attribute for images.

```html
<img src="student.jpg"
     alt="Student learning HTML">
```

The `alt` text is read by screen readers and displayed if the image cannot be loaded.

---

# Accessible Links

Use meaningful link text.

Incorrect:

```html
<a href="course.html">Click Here</a>
```

Correct:

```html
<a href="course.html">
    View HTML Course
</a>
```

---

# Use Proper Headings

Use heading tags in the correct order.

Correct:

```html
<h1>Main Title</h1>

<h2>Section</h2>

<h3>Topic</h3>
```

Avoid skipping heading levels.

Incorrect:

```html
<h1>Main Title</h1>

<h4>Topic</h4>
```

---

# Accessible Forms

Always associate labels with form controls.

```html
<label for="email">
    Email Address
</label>

<input
    type="email"
    id="email"
    name="email">
```

This helps screen readers identify the purpose of the input field.

---

# Buttons vs Links

Use the correct element for the correct purpose.

For navigation:

```html
<a href="courses.html">
    View Courses
</a>
```

For actions:

```html
<button>
    Submit
</button>
```

---

# Use Tables Properly

Include table headers using `<th>`.

```html
<table>

<tr>
    <th>Name</th>
    <th>Course</th>
</tr>

<tr>
    <td>Alice</td>
    <td>HTML</td>
</tr>

</table>
```

---

# Keyboard Accessibility

Users should be able to navigate a webpage using only the keyboard.

Ensure that:

- Links can receive focus.
- Buttons are keyboard accessible.
- Form fields can be reached using the **Tab** key.

---

# Colour Contrast

Choose colours with sufficient contrast.

Good:

- Black text on a white background
- Dark blue text on a light background

Poor:

- Yellow text on a white background
- Light grey text on a white background

---

# ARIA Attributes

ARIA (Accessible Rich Internet Applications) attributes improve accessibility for assistive technologies.

Example:

```html
<button aria-label="Close Menu">
    ✖
</button>
```

Use ARIA only when standard HTML cannot provide the required accessibility.

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>Accessible Webpage</title>
</head>

<body>

<header>
    <h1>TechVidyalaya</h1>
</header>

<main>

<img
    src="student.jpg"
    alt="Student learning HTML">

<form>

<label for="name">
    Name
</label>

<input
    type="text"
    id="name">

<button>
    Submit
</button>

</form>

</main>

<footer>

© 2026 TechVidyalaya

</footer>

</body>

</html>
```

---

# Common Mistakes

### Missing `alt` Attribute

Incorrect:

```html
<img src="logo.png">
```

Correct:

```html
<img
    src="logo.png"
    alt="Company Logo">
```

---

### Using Headings for Styling Only

Incorrect:

```html
<h1>Small Text</h1>
```

Use headings only to represent the document structure.

---

### Missing Form Labels

Incorrect:

```html
<input type="text">
```

Correct:

```html
<label for="username">
    Username
</label>

<input
    id="username"
    type="text">
```

---

# Best Practices

- Use semantic HTML elements.
- Add `alt` text for every meaningful image.
- Write descriptive link text.
- Use labels for form inputs.
- Maintain proper heading order.
- Ensure keyboard navigation works.
- Choose high-contrast colours.
- Use ARIA attributes only when necessary.

---

# Quick Summary

- Accessibility makes websites usable for everyone.
- Semantic HTML improves accessibility.
- Images should include `alt` text.
- Forms should use labels.
- Keyboard navigation is essential.
- Good colour contrast improves readability.
- ARIA enhances accessibility when required.

---

# Key Terms

| Term | Description |
|------|-------------|
| Accessibility | Designing websites for all users |
| Screen Reader | Software that reads webpage content aloud |
| Alt Text | Description of an image |
| Semantic HTML | HTML elements with meaningful structure |
| ARIA | Accessibility attributes for assistive technologies |

---

# Practice Questions

### Multiple Choice

**1. Which attribute describes an image for screen readers?**

A. `title`

B. `alt`

C. `src`

D. `href`

**Answer:** B

---

**2. Which element is used to label an input field?**

A. `<caption>`

B. `<legend>`

C. `<label>`

D. `<span>`

**Answer:** C

---

**3. What does ARIA stand for?**

A. Advanced Responsive Internet Application

B. Accessible Rich Internet Applications

C. Automatic Responsive Internet Access

D. Accessible Responsive Interactive Application

**Answer:** B

---

# Short Answer Questions

1. What is web accessibility?
2. Why is the `alt` attribute important?
3. Why should labels be used in forms?
4. What is the purpose of semantic HTML?
5. When should ARIA attributes be used?

---

# Hands-on Exercise

Create an accessible webpage containing:

- A semantic page layout using `<header>`, `<main>`, and `<footer>`
- An image with meaningful `alt` text
- A form with labels for every input
- Accessible navigation links
- A submit button
- Proper heading hierarchy

Test the webpage using keyboard navigation.

---

# Interview Questions

### Q1. Why is accessibility important in web development?

Accessibility ensures that websites can be used by everyone, including people with disabilities. It also improves SEO, usability, and compliance with accessibility standards.

---

### Q2. What is the purpose of the `alt` attribute?

The `alt` attribute provides alternative text for images. It is read by screen readers and displayed if the image cannot be loaded.

---

### Q3. What are ARIA attributes?

ARIA attributes provide additional accessibility information for assistive technologies when standard HTML elements are not sufficient.

---

## Chapter Summary

In this chapter, you learned:

- The importance of web accessibility
- How semantic HTML improves accessibility
- The role of `alt` text and form labels
- How to support keyboard navigation
- Best practices for building inclusive websites

In the next chapter, we will learn about **HTML5 APIs**.
