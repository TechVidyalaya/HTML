# Chapter 15: HTML Iframes

## Learning Objectives

After completing this chapter, you will be able to:

- Understand what an iframe is
- Embed webpages inside another webpage
- Display YouTube videos using iframes
- Use common iframe attributes
- Follow iframe security and best practices

---

# What is an HTML Iframe?

An **iframe (Inline Frame)** is used to embed another webpage or external content inside the current webpage.

Examples include:

- YouTube videos
- Google Maps
- Online documents
- Other websites

The `<iframe>` tag creates an embedded frame.

---

# Basic Syntax

```html
<iframe src="https://example.com"></iframe>
```

Output:

```
+--------------------------------------+
|                                      |
|      Embedded Webpage                |
|                                      |
+--------------------------------------+
```

---

# Displaying a Webpage

```html
<iframe
    src="https://www.example.com"
    width="600"
    height="400">
</iframe>
```

The webpage is displayed inside the frame.

---

# Setting Width and Height

```html
<iframe
    src="about.html"
    width="500"
    height="300">
</iframe>
```

---

# Adding a Border

```html
<iframe
    src="about.html"
    style="border:2px solid black;">
</iframe>
```

Or remove the border:

```html
<iframe
    src="about.html"
    style="border:none;">
</iframe>
```

---

# Embedding a YouTube Video

YouTube provides an embed URL.

```html
<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/VIDEO_ID"
    title="YouTube Video"
    allowfullscreen>
</iframe>
```

Replace `VIDEO_ID` with the actual YouTube video ID.

---

# Embedding Google Maps

Google Maps also provides an embed code.

Example:

```html
<iframe
    src="https://www.google.com/maps/embed?...">
</iframe>
```

---

# Loading Local HTML Pages

Project structure:

```
project/
│── index.html
│── about.html
```

Display `about.html` inside `index.html`.

```html
<iframe
    src="about.html"
    width="600"
    height="300">
</iframe>
```

---

# The `title` Attribute

Always provide a title for accessibility.

```html
<iframe
    src="about.html"
    title="About Page">
</iframe>
```

---

# Loading Attribute

Improve page performance using lazy loading.

```html
<iframe
    src="about.html"
    loading="lazy">
</iframe>
```

The iframe loads only when it is about to become visible.

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML Iframe</title>
</head>

<body>

<h1>Welcome</h1>

<iframe
    src="about.html"
    width="600"
    height="300"
    title="About Page">
</iframe>

</body>

</html>
```

---

# Common Iframe Attributes

| Attribute | Purpose |
|-----------|---------|
| `src` | Source URL |
| `width` | Frame width |
| `height` | Frame height |
| `title` | Accessibility description |
| `loading` | Lazy loading |
| `allowfullscreen` | Enables full-screen mode for videos |

---

# Common Mistakes

### Missing Title

Incorrect:

```html
<iframe src="about.html"></iframe>
```

Correct:

```html
<iframe
    src="about.html"
    title="About Page">
</iframe>
```

---

### Using Large Dimensions

Incorrect:

```html
<iframe
    width="2000"
    height="1500">
</iframe>
```

Choose dimensions appropriate for the webpage layout.

---

# Best Practices

- Always provide a `title`.
- Use `loading="lazy"` when possible.
- Embed only trusted websites.
- Use responsive dimensions for different screen sizes.
- Avoid embedding unnecessary content.

---

# Quick Summary

- `<iframe>` embeds another webpage.
- `src` specifies the page to display.
- `width` and `height` control the frame size.
- `title` improves accessibility.
- `loading="lazy"` improves performance.
- `allowfullscreen` enables full-screen viewing.

---

# Key Terms

| Term | Description |
|------|-------------|
| Iframe | Embedded webpage |
| Source | URL loaded in the iframe |
| Embed | Display external content |
| Lazy Loading | Load content only when needed |
| Full Screen | Displays content across the entire screen |

---

# Practice Questions

### Multiple Choice

**1. Which tag is used to embed another webpage?**

A. `<embed>`

B. `<frame>`

C. `<iframe>`

D. `<window>`

**Answer:** C

---

**2. Which attribute specifies the webpage to display?**

A. `href`

B. `src`

C. `link`

D. `url`

**Answer:** B

---

**3. Which attribute improves iframe accessibility?**

A. `title`

B. `caption`

C. `name`

D. `alt`

**Answer:** A

---

# Short Answer Questions

1. What is an iframe?
2. What is the purpose of the `src` attribute?
3. Why should every iframe have a `title` attribute?
4. What is lazy loading?
5. Name two common uses of iframes.

---

# Hands-on Exercise

Create a webpage that contains:

- An embedded local HTML page
- A YouTube video using an iframe
- A Google Map
- An iframe with `loading="lazy"`
- An iframe with a custom border

Run the webpage and verify the output.

---

# Interview Questions

### Q1. What is an iframe?

An iframe is an HTML element used to display another webpage or external content inside the current webpage.

---

### Q2. What are some common uses of iframes?

Common uses include embedding YouTube videos, Google Maps, online documents, dashboards, and other webpages.

---

### Q3. Why should `loading="lazy"` be used?

Lazy loading delays loading of the iframe until it is needed, improving page load speed and reducing unnecessary network requests.

---

## Chapter Summary

In this chapter, you learned:

- What an iframe is
- How to embed webpages and external content
- How to embed YouTube videos and Google Maps
- Common iframe attributes
- Best practices for accessibility and performance

In the next chapter, we will learn about **HTML Entities and Symbols**.
