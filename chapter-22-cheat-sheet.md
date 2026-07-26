# Chapter 22: HTML Cheat Sheet

## HTML Cheat Sheet

This chapter serves as a **quick reference guide** for the most commonly used HTML tags, attributes, and concepts.

---

# Basic HTML Structure

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Webpage</title>
</head>

<body>

    <!-- Content goes here -->

</body>

</html>
```

---

# Common HTML Tags

| Tag | Purpose |
|------|---------|
| `<html>` | Root element |
| `<head>` | Metadata |
| `<title>` | Page title |
| `<body>` | Visible webpage content |
| `<h1>`–`<h6>` | Headings |
| `<p>` | Paragraph |
| `<br>` | Line break |
| `<hr>` | Horizontal line |
| `<div>` | Block container |
| `<span>` | Inline container |

---

# Text Formatting

```html
<strong>Bold</strong>

<em>Italic</em>

<u>Underline</u>

<mark>Highlight</mark>

<small>Small Text</small>

<sub>Subscript</sub>

<sup>Superscript</sup>
```

---

# Links

```html
<a href="about.html">About</a>

<a href="https://example.com" target="_blank">
    Visit Website
</a>
```

---

# Images

```html
<img
    src="images/logo.png"
    alt="Company Logo"
    width="200">
```

---

# Lists

### Ordered List

```html
<ol>
    <li>Java</li>
    <li>Python</li>
</ol>
```

### Unordered List

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
</ul>
```

---

# Tables

```html
<table>

<tr>
    <th>Name</th>
    <th>Age</th>
</tr>

<tr>
    <td>John</td>
    <td>25</td>
</tr>

</table>
```

---

# Forms

```html
<form>

<label>Name</label>

<input type="text">

<input type="email">

<input type="password">

<textarea></textarea>

<select>
    <option>HTML</option>
</select>

<button>Submit</button>

</form>
```

---

# Common Input Types

```html
text
password
email
number
date
time
radio
checkbox
file
color
range
search
url
tel
submit
reset
```

---

# Semantic Elements

```html
<header>

<nav>

<main>

<section>

<article>

<aside>

<footer>
```

---

# Audio

```html
<audio controls>

<source
    src="music.mp3"
    type="audio/mpeg">

</audio>
```

---

# Video

```html
<video controls width="500">

<source
    src="video.mp4"
    type="video/mp4">

</video>
```

---

# Iframe

```html
<iframe
    src="about.html"
    width="600"
    height="300">
</iframe>
```

---

# HTML Entities

| Character | Entity |
|-----------|--------|
| `<` | `&lt;` |
| `>` | `&gt;` |
| `&` | `&amp;` |
| `©` | `&copy;` |
| `®` | `&reg;` |
| `™` | `&trade;` |
| Space | `&nbsp;` |

---

# IDs and Classes

```html
<h1 id="title">

Welcome

</h1>

<p class="course">

HTML

</p>
```

CSS Selectors:

```css
#title { }

.course { }
```

---

# HTML5 APIs

- Geolocation API
- Web Storage API
- Drag and Drop API
- Canvas API
- Web Workers API

---

# Common Meta Tags

```html
<meta charset="UTF-8">

<meta
    name="viewport"
    content="width=device-width, initial-scale=1.0">

<meta
    name="description"
    content="Learn HTML">
```

---

# Block vs Inline Elements

| Block Elements | Inline Elements |
|----------------|-----------------|
| `<div>` | `<span>` |
| `<section>` | `<a>` |
| `<article>` | `<img>` |
| `<p>` | `<strong>` |
| `<h1>` | `<em>` |

---

# File Structure

```
project/
│── index.html
│── about.html
│── contact.html
│── css/
│     └── style.css
│── js/
│     └── script.js
│── images/
│── videos/
│── audio/
```

---

# HTML Best Practices

- Use semantic HTML.
- Keep code properly indented.
- Use meaningful file names.
- Add `alt` text to images.
- Keep HTML, CSS, and JavaScript separate.
- Optimise images and videos.
- Validate HTML before deployment.
- Use descriptive page titles.
- Test webpages on different browsers and devices.

---

# Keyboard Shortcuts (VS Code)

| Shortcut | Action |
|----------|--------|
| `! + Tab` | Generate HTML boilerplate |
| `Ctrl + /` | Comment/Uncomment |
| `Alt + Shift + F` | Format document |
| `Ctrl + Space` | IntelliSense |
| `Ctrl + S` | Save file |

---

# Frequently Used HTML Attributes

| Attribute | Purpose |
|-----------|---------|
| `id` | Unique identifier |
| `class` | Group elements |
| `src` | File location |
| `href` | Hyperlink destination |
| `alt` | Alternative image text |
| `title` | Additional information |
| `width` | Element width |
| `height` | Element height |
| `name` | Form field name |
| `value` | Input value |
| `placeholder` | Input hint |
| `required` | Mandatory field |
| `disabled` | Disable input |
| `readonly` | Read-only input |

---

# HTML Interview Revision

Remember these topics:

- HTML document structure
- Headings and paragraphs
- Text formatting
- Links and images
- Lists and tables
- Forms and input types
- Semantic HTML
- IDs and Classes
- Audio and Video
- Iframes
- HTML Entities
- Accessibility
- HTML5 APIs
- HTML Best Practices

---

# HTML Learning Roadmap

```
HTML Basics
      ↓
Text & Formatting
      ↓
Links & Images
      ↓
Lists & Tables
      ↓
Forms
      ↓
Semantic HTML
      ↓
Multimedia
      ↓
HTML5 APIs
      ↓
Accessibility
      ↓
Best Practices
      ↓
Portfolio Project
      ↓
CSS
      ↓
JavaScript
      ↓
Responsive Web Design
      ↓
Frontend Frameworks
```

---

# Final Module Summary

Congratulations! 🎉

You have completed the **TechVidyalaya HTML Module**. You have learned:

- HTML fundamentals
- Page structure
- Formatting and multimedia
- Forms and semantic HTML
- Accessibility and HTML5 APIs
- Best coding practices
- Building a complete portfolio project
- Interview preparation and revision

You are now ready to move on to the **CSS Module**, where you will learn how to style webpages, create responsive layouts, and build professional-looking websites.

**Happy Coding! 🚀**
