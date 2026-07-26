# Chapter 2: HTML Document Structure

## Learning Objectives

After completing this chapter, you will be able to:

- Understand the structure of an HTML document
- Learn the purpose of each HTML tag
- Create a valid HTML5 webpage
- Understand how browsers interpret HTML
- Write clean and well-structured HTML code

---

# What is an HTML Document?

An HTML document is a text file that contains HTML tags. These tags tell the browser how to display the webpage.

Every HTML page follows a standard structure.

---

# Basic HTML Document Structure

```html
<!DOCTYPE html>
<html>
<head>
    <title>My First Web Page</title>
</head>
<body>

    <h1>Welcome to HTML</h1>
    <p>This is my first webpage.</p>

</body>
</html>
```

---

# HTML Document Structure Diagram

```
<!DOCTYPE html>
│
├── <html>
│     │
│     ├── <head>
│     │      ├── <title>
│     │      ├── <meta>
│     │      └── <link>
│     │
│     └── <body>
│            ├── Headings
│            ├── Paragraphs
│            ├── Images
│            ├── Tables
│            ├── Forms
│            └── Other Content
```

---

# Understanding Each Tag

## 1. `<!DOCTYPE html>`

This declaration tells the browser that the document uses HTML5.

```html
<!DOCTYPE html>
```

It must always be the first line of the HTML document.

---

## 2. `<html>`

The `<html>` tag is the root element of the webpage.

Everything inside the webpage is enclosed within this tag.

```html
<html>

</html>
```

---

## 3. `<head>`

The `<head>` section contains information about the webpage that is not directly displayed.

It typically includes:

- Page title
- Meta information
- CSS files
- Icons
- JavaScript files

Example:

```html
<head>
    <title>TechVidyalaya</title>
</head>
```

---

## 4. `<title>`

The `<title>` tag specifies the title shown on the browser tab.

```html
<title>HTML Tutorial</title>
```

Output:

```
Browser Tab
--------------------
HTML Tutorial
```

---

## 5. `<body>`

The `<body>` contains everything visible on the webpage.

Examples include:

- Headings
- Paragraphs
- Images
- Buttons
- Forms
- Tables

Example:

```html
<body>

<h1>Welcome</h1>

<p>Hello World!</p>

</body>
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>

    <title>Student Portal</title>

</head>

<body>

    <h1>Welcome Students</h1>

    <p>Learn HTML from scratch.</p>

</body>

</html>
```

Output:

```
Welcome Students

Learn HTML from scratch.
```

---

# HTML Nesting

HTML elements are usually placed inside other elements.

Example:

```html
<html>

<head>

<title>Example</title>

</head>

<body>

<h1>Hello</h1>

</body>

</html>
```

This is called **nesting**.

---

# Proper Indentation

Good indentation makes HTML easy to read.

Good Example:

```html
<body>
    <h1>Heading</h1>
    <p>Paragraph</p>
</body>
```

Bad Example:

```html
<body><h1>Heading</h1><p>Paragraph</p></body>
```

---

# HTML Comments

Comments are ignored by the browser.

Syntax:

```html
<!-- This is a comment -->
```

Example:

```html
<body>

<!-- Main Heading -->

<h1>Welcome</h1>

</body>
```

---

# HTML Boilerplate

Every HTML page usually starts with this template.

```html
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <title>My Website</title>

</head>

<body>

</body>

</html>
```

---

# Why Use `lang="en"`?

```html
<html lang="en">
```

It tells browsers and search engines that the page content is in English.

Benefits:

- Better accessibility
- Improved SEO
- Better screen reader support

---

# Why Use `<meta charset="UTF-8">`?

```html
<meta charset="UTF-8">
```

It allows the webpage to display characters from many languages correctly.

Example:

```
English
हिन्दी
தமிழ்
日本語
😊
```

---

# Why Use the Viewport Meta Tag?

```html
<meta name="viewport"
      content="width=device-width, initial-scale=1.0">
```

This makes the webpage responsive on mobile devices.

Without it, pages may appear zoomed out on smaller screens.

---

# Best Practices

- Start every page with `<!DOCTYPE html>`
- Use proper indentation
- Keep code organised
- Close all tags properly
- Add comments where necessary
- Include useful meta tags
- Use meaningful page titles

---

# Quick Summary

- Every HTML page has a standard structure.
- `<html>` is the root element.
- `<head>` stores page information.
- `<title>` sets the browser tab title.
- `<body>` contains visible webpage content.
- Proper indentation improves readability.

---

# Key Terms

| Term | Description |
|------|-------------|
| DOCTYPE | Declares the HTML version |
| html | Root element of the webpage |
| head | Stores metadata |
| title | Browser tab title |
| body | Visible webpage content |
| Meta Tag | Provides information about the webpage |

---

# Practice Questions

### Multiple Choice

**1. Which tag contains the visible webpage content?**

A. `<head>`

B. `<title>`

C. `<body>`

D. `<meta>`

**Answer:** C

---

**2. Which declaration should appear first in every HTML5 document?**

A. `<html>`

B. `<body>`

C. `<!DOCTYPE html>`

D. `<head>`

**Answer:** C

---

**3. Which tag defines the title displayed on the browser tab?**

A. `<meta>`

B. `<title>`

C. `<header>`

D. `<h1>`

**Answer:** B

---

# Short Answer Questions

1. What is the purpose of `<!DOCTYPE html>`?
2. What is the difference between `<head>` and `<body>`?
3. Why is the `<title>` tag important?
4. Why should HTML code be properly indented?
5. What is the purpose of the viewport meta tag?

---

# Hands-on Exercise

Create a webpage with:

- HTML5 boilerplate
- Page title **"My Portfolio"**
- One heading
- Two paragraphs
- One HTML comment

Run the page in your browser and verify the output.

---

# Interview Questions

### Q1. What is the purpose of the `<head>` section?

The `<head>` section stores metadata such as the page title, character encoding, CSS links, JavaScript files, and other information that is not directly displayed on the webpage.

---

### Q2. Why is `<!DOCTYPE html>` important?

It tells the browser to render the document using the HTML5 standard, ensuring consistent behaviour across modern browsers.

---

### Q3. What is the purpose of the viewport meta tag?

It makes webpages responsive by adjusting the layout to match the width of the user's device.

---

## Chapter Summary

In this chapter, you learned:

- The standard structure of an HTML document
- The purpose of `<!DOCTYPE html>`
- The roles of `<html>`, `<head>`, `<title>`, and `<body>`
- How to use comments and proper indentation
- The importance of HTML5 boilerplate and meta tags

In the next chapter, we will learn about **HTML Headings and Paragraphs**.
