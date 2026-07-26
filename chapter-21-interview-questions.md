# Chapter 21: HTML Interview Questions and Answers

## Learning Objectives

After completing this chapter, you will be able to:

- Revise important HTML concepts
- Prepare for HTML interviews
- Answer common beginner and intermediate questions
- Strengthen your understanding through practical examples

---

# Interview Tips

Before attending an HTML interview:

- Understand HTML fundamentals.
- Practice writing HTML without using AI or templates.
- Know the purpose of common HTML tags.
- Be familiar with semantic HTML.
- Explain concepts with examples.
- Build at least one complete HTML project.

---

# Frequently Asked Interview Questions

## Q1. What is HTML?

**Answer:**

HTML (HyperText Markup Language) is the standard markup language used to create and structure webpages. It defines the content of a webpage using elements and tags.

---

## Q2. What is the difference between HTML and HTML5?

**Answer:**

| HTML | HTML5 |
|------|--------|
| Older version | Latest version |
| Limited multimedia support | Built-in audio and video support |
| Fewer semantic elements | New semantic elements like `<header>` and `<section>` |
| Limited APIs | Includes APIs like Geolocation and Web Storage |

---

## Q3. What is the purpose of the `<!DOCTYPE html>` declaration?

**Answer:**

It tells the browser that the document uses HTML5 and ensures the page is rendered in standards mode.

---

## Q4. What are HTML tags and elements?

**Answer:**

A **tag** is the markup enclosed in angle brackets, such as `<p>`. An **element** includes the opening tag, content, and closing tag.

Example:

```html
<p>Hello World</p>
```

---

## Q5. What are semantic HTML elements?

**Answer:**

Semantic elements describe the meaning of the content.

Examples:

- `<header>`
- `<nav>`
- `<main>`
- `<section>`
- `<article>`
- `<footer>`

---

## Q6. What is the difference between `<div>` and `<span>`?

| `<div>` | `<span>` |
|----------|-----------|
| Block element | Inline element |
| Starts on a new line | Stays on the same line |
| Used for layout | Used for styling small portions of content |

---

## Q7. What is the difference between Block and Inline elements?

**Block Elements**

- Start on a new line
- Occupy full width

Examples:

```html
<div>
<p>
<section>
```

**Inline Elements**

- Stay on the same line
- Occupy only required width

Examples:

```html
<span>
<a>
<strong>
```

---

## Q8. What are HTML attributes?

**Answer:**

Attributes provide additional information about HTML elements.

Example:

```html
<img
    src="logo.png"
    alt="Company Logo">
```

Here, `src` and `alt` are attributes.

---

## Q9. What is the difference between `id` and `class`?

| ID | Class |
|----|-------|
| Unique | Reusable |
| One element | Multiple elements |
| CSS selector: `#id` | CSS selector: `.class` |

---

## Q10. Why is the `alt` attribute important?

**Answer:**

The `alt` attribute:

- Improves accessibility
- Helps screen readers
- Displays text if the image cannot be loaded
- Improves SEO

---

## Q11. What are HTML entities?

**Answer:**

HTML entities display reserved or special characters.

Examples:

```html
&lt;
&gt;
&amp;
&copy;
```

---

## Q12. What are the new features of HTML5?

**Answer:**

HTML5 introduced:

- Semantic elements
- Audio and video support
- Canvas
- Geolocation API
- Web Storage
- Drag and Drop
- Better form controls

---

## Q13. What is the difference between `localStorage` and `sessionStorage`?

| localStorage | sessionStorage |
|--------------|----------------|
| Persistent storage | Temporary storage |
| Data remains after browser closes | Data is removed when the tab closes |

---

## Q14. What is an iframe?

**Answer:**

An iframe is used to embed another webpage or external content inside the current webpage.

Example:

```html
<iframe
    src="about.html">
</iframe>
```

---

## Q15. What is Accessibility?

**Answer:**

Accessibility means designing websites that everyone can use, including people with disabilities.

It includes:

- Semantic HTML
- Alt text
- Labels
- Keyboard navigation
- Proper colour contrast

---

## Q16. Why should semantic HTML be preferred over `<div>`?

**Answer:**

Semantic HTML:

- Improves readability
- Helps search engines understand the page
- Supports screen readers
- Makes code easier to maintain

---

## Q17. What are the most commonly used HTML form elements?

Examples:

```html
<form>
<input>
<label>
<textarea>
<select>
<option>
<button>
```

---

## Q18. What is the purpose of the `<meta>` tag?

**Answer:**

The `<meta>` tag provides information about the webpage, such as:

- Character encoding
- Viewport settings
- Description
- Keywords
- Author

Example:

```html
<meta charset="UTF-8">

<meta
    name="viewport"
    content="width=device-width, initial-scale=1.0">
```

---

## Q19. What is the difference between Absolute and Relative URLs?

**Absolute URL**

```html
https://www.example.com/about.html
```

**Relative URL**

```html
about.html
```

---

## Q20. How do you improve HTML performance?

**Answer:**

- Optimise images
- Use lazy loading
- Minimise unnecessary HTML
- Use semantic elements
- Validate HTML
- Keep CSS and JavaScript separate

---

# Practical Coding Questions

### 1. Create a registration form.

### 2. Create a table showing employee details.

### 3. Build a navigation bar.

### 4. Display a responsive image.

### 5. Create a portfolio webpage.

### 6. Embed a YouTube video.

### 7. Create an ordered and unordered list.

### 8. Build a contact page.

### 9. Display an image gallery.

### 10. Create a webpage using semantic HTML.

---

# Rapid Fire Questions

- What does HTML stand for?
- Which tag creates a hyperlink?
- Which tag displays an image?
- Which attribute specifies image text?
- Which tag creates a table row?
- Which tag creates a list item?
- Which tag embeds a webpage?
- Which tag creates a form?
- What does `id` represent?
- What does `class` represent?
- What is semantic HTML?
- What is HTML5?
- Which tag is used for navigation?
- Which tag contains the main content?
- What is the purpose of the `<title>` tag?

---

# Mini Quiz

### 1. Which HTML element represents the main content of a webpage?

A. `<body>`

B. `<main>`

C. `<section>`

D. `<article>`

**Answer:** B

---

### 2. Which attribute uniquely identifies an element?

A. class

B. id

C. src

D. href

**Answer:** B

---

### 3. Which HTML tag is used to display an image?

A. `<picture>`

B. `<img>`

C. `<photo>`

D. `<image>`

**Answer:** B

---

### 4. Which HTML5 API stores data until it is removed?

A. Cookies

B. sessionStorage

C. localStorage

D. Cache

**Answer:** C

---

### 5. Which HTML element embeds another webpage?

A. `<embed>`

B. `<frame>`

C. `<iframe>`

D. `<video>`

**Answer:** C

---

# Final Revision Checklist

✔ HTML Document Structure

✔ Headings and Paragraphs

✔ Text Formatting

✔ Links and Images

✔ Lists and Tables

✔ Forms and Input Types

✔ Semantic HTML

✔ Audio and Video

✔ Block and Inline Elements

✔ IDs and Classes

✔ Iframes

✔ HTML Entities

✔ Accessibility

✔ HTML5 APIs

✔ HTML Best Practices

✔ Portfolio Project

---

# Chapter Summary

In this chapter, you revised the most important HTML concepts through frequently asked interview questions, coding exercises, and quizzes. Completing these questions will help you build confidence for technical interviews and strengthen your HTML fundamentals.

In the next and final chapter, we will create a **Complete HTML Cheat Sheet** for quick revision before interviews and exams.
