# Chapter 11: HTML Semantic Elements

## Learning Objectives

After completing this chapter, you will be able to:

- Understand semantic HTML
- Differentiate between semantic and non-semantic elements
- Use common semantic HTML5 tags
- Build a well-structured webpage
- Improve accessibility and SEO using semantic elements

---

# What are Semantic Elements?

Semantic elements clearly describe the purpose of their content to both browsers and developers.

For example:

- A `<header>` represents the top section of a webpage.
- A `<footer>` represents the bottom section.
- A `<nav>` contains navigation links.

Semantic HTML makes webpages:

- Easier to read
- Easier to maintain
- More accessible
- Better for Search Engine Optimisation (SEO)

---

# Semantic vs Non-Semantic Elements

### Semantic Elements

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

These elements clearly describe their purpose.

---

### Non-Semantic Elements

```html
<div>

<span>
```

These elements do not describe what the content represents.

---

# Why Use Semantic HTML?

Benefits include:

- Better code readability
- Improved accessibility
- Better SEO rankings
- Easier maintenance
- Better browser understanding

---

# Common Semantic Elements

| Element | Purpose |
|----------|---------|
| `<header>` | Top section of a page |
| `<nav>` | Navigation links |
| `<main>` | Main page content |
| `<section>` | Related content section |
| `<article>` | Independent content |
| `<aside>` | Sidebar or related information |
| `<footer>` | Bottom section of a page |
| `<figure>` | Image or diagram |
| `<figcaption>` | Caption for a figure |

---

# The `<header>` Element

Represents introductory content.

Example:

```html
<header>

<h1>TechVidyalaya</h1>

<p>Learn Technology the Right Way</p>

</header>
```

---

# The `<nav>` Element

Contains navigation links.

```html
<nav>

<a href="index.html">Home</a>

<a href="courses.html">Courses</a>

<a href="contact.html">Contact</a>

</nav>
```

---

# The `<main>` Element

Contains the primary content of the webpage.

```html
<main>

<h2>Welcome</h2>

<p>This is the main content.</p>

</main>
```

A webpage should have only **one** `<main>` element.

---

# The `<section>` Element

Groups related content.

```html
<section>

<h2>Java Course</h2>

<p>Learn Core Java and Spring Boot.</p>

</section>
```

---

# The `<article>` Element

Represents independent content.

Examples:

- Blog posts
- News articles
- Forum posts

```html
<article>

<h2>HTML Basics</h2>

<p>HTML is the foundation of web development.</p>

</article>
```

---

# The `<aside>` Element

Contains related or supplementary information.

```html
<aside>

<h3>Related Courses</h3>

<ul>

<li>CSS</li>

<li>JavaScript</li>

</ul>

</aside>
```

---

# The `<footer>` Element

Represents the footer of a webpage or section.

```html
<footer>

<p>&copy; 2026 TechVidyalaya</p>

</footer>
```

---

# The `<figure>` Element

Groups media content.

```html
<figure>

<img src="student.jpg"
     alt="Student">

<figcaption>
Student Learning HTML
</figcaption>

</figure>
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>

<title>Semantic HTML</title>

</head>

<body>

<header>

<h1>TechVidyalaya</h1>

</header>

<nav>

<a href="#">Home</a>

<a href="#">Courses</a>

<a href="#">About</a>

</nav>

<main>

<section>

<h2>Latest Courses</h2>

<p>Explore our programming courses.</p>

</section>

<article>

<h2>HTML Tutorial</h2>

<p>Learn HTML from scratch.</p>

</article>

<aside>

<h3>Popular Courses</h3>

<ul>

<li>Java</li>

<li>Python</li>

</ul>

</aside>

</main>

<footer>

<p>&copy; 2026 TechVidyalaya</p>

</footer>

</body>

</html>
```

---

# Semantic Page Layout

```
---------------------------------------
|             Header                  |
---------------------------------------
|              Navigation             |
---------------------------------------
|                                     |
|     Main Content                    |
|  -------------------------------    |
|  | Section                    |     |
|  |----------------------------|     |
|  | Article                    |     |
|  -------------------------------    |
|                     Aside           |
---------------------------------------
|             Footer                  |
---------------------------------------
```

---

# Common Mistakes

### Using Only `<div>`

Incorrect:

```html
<div>

<div>

<div>

</div>

</div>

</div>
```

Better:

```html
<header>

<nav>

<main>

<footer>
```

---

### Multiple `<main>` Elements

Incorrect:

```html
<main>

</main>

<main>

</main>
```

Correct:

```html
<main>

</main>
```

---

# Best Practices

- Use semantic elements whenever possible.
- Use only one `<main>` per page.
- Keep headings inside sections.
- Use `<article>` for standalone content.
- Use `<aside>` for related information.
- Avoid unnecessary `<div>` elements.

---

# Quick Summary

- Semantic elements describe the purpose of content.
- They improve accessibility and SEO.
- `<header>` defines introductory content.
- `<nav>` contains navigation links.
- `<main>` contains the primary page content.
- `<section>` groups related content.
- `<article>` represents standalone content.
- `<aside>` displays related information.
- `<footer>` contains footer content.

---

# Key Terms

| Term | Description |
|------|-------------|
| Semantic HTML | HTML with meaningful elements |
| Header | Top section of a webpage |
| Navigation | Collection of links |
| Main | Primary webpage content |
| Section | Group of related content |
| Article | Independent content |
| Aside | Supplementary information |
| Footer | Bottom section of a webpage |

---

# Practice Questions

### Multiple Choice

**1. Which element represents the main content of a webpage?**

A. `<header>`

B. `<section>`

C. `<main>`

D. `<aside>`

**Answer:** C

---

**2. Which element contains navigation links?**

A. `<menu>`

B. `<nav>`

C. `<section>`

D. `<footer>`

**Answer:** B

---

**3. Which element is commonly used for blog posts?**

A. `<article>`

B. `<span>`

C. `<div>`

D. `<figure>`

**Answer:** A

---

# Short Answer Questions

1. What are semantic HTML elements?
2. Why are semantic elements preferred over `<div>`?
3. What is the purpose of the `<main>` element?
4. What is the difference between `<section>` and `<article>`?
5. Why is semantic HTML important for SEO?

---

# Hands-on Exercise

Create a webpage containing:

- A header with a website title
- A navigation menu
- A main section
- Two content sections
- One article
- One sidebar using `<aside>`
- A footer with copyright information

Open the webpage and verify the layout.

---

# Interview Questions

### Q1. What is semantic HTML?

Semantic HTML uses meaningful tags that describe the purpose of the content, making webpages easier to understand for developers, browsers, search engines, and assistive technologies.

---

### Q2. What is the difference between `<section>` and `<article>`?

A `<section>` groups related content within a page, while an `<article>` represents independent, self-contained content that can stand on its own, such as a blog post or news article.

---

### Q3. Why should semantic HTML be used?

Semantic HTML improves:

- Accessibility
- Search engine optimisation (SEO)
- Code readability
- Maintainability
- Browser understanding of webpage structure

---

## Chapter Summary

In this chapter, you learned:

- What semantic HTML is
- The difference between semantic and non-semantic elements
- How to use HTML5 semantic tags
- How semantic elements improve accessibility and SEO
- Best practices for creating well-structured webpages

In the next chapter, we will learn about **HTML Audio and Video**.
