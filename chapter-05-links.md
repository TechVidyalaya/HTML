# Chapter 5: HTML Links

## Learning Objectives

After completing this chapter, you will be able to:

- Understand HTML links
- Create hyperlinks between webpages
- Open links in a new tab
- Link to email addresses and phone numbers
- Create bookmarks within a webpage
- Follow best practices for using links

---

# What are HTML Links?

HTML links, also called **hyperlinks**, allow users to navigate from one webpage to another.

Links can connect to:

- Another webpage
- Another website
- An email address
- A phone number
- A section within the same page
- A downloadable file

The `<a>` (anchor) tag is used to create links.

---

# Basic Link Syntax

```html
<a href="https://www.google.com">Visit Google</a>
```

Output:

```
Visit Google
```

(Clicking the text opens Google's website.)

---

# The `href` Attribute

The `href` (Hypertext Reference) attribute specifies the destination of the link.

```html
<a href="about.html">About Us</a>
```

---

# Linking to Another Page

Suppose your project contains:

```
project/
│── index.html
│── about.html
│── contact.html
```

From `index.html`:

```html
<a href="about.html">About Us</a>
```

---

# Opening a Link in a New Tab

Use the `target="_blank"` attribute.

```html
<a href="https://www.youtube.com" target="_blank">
    Visit YouTube
</a>
```

---

# Adding Security with `rel`

When using `target="_blank"`, add `rel="noopener noreferrer"`.

```html
<a href="https://www.youtube.com"
   target="_blank"
   rel="noopener noreferrer">
   Visit YouTube
</a>
```

---

# Absolute URL

An absolute URL contains the complete web address.

```html
<a href="https://www.techvidyalaya.com">
    TechVidyalaya
</a>
```

---

# Relative URL

A relative URL points to another file within the same project.

```html
<a href="courses.html">
    Courses
</a>
```

---

# Email Link

Use `mailto:` to open the user's email application.

```html
<a href="mailto:info@example.com">
    Email Us
</a>
```

---

# Telephone Link

Use `tel:` for mobile devices.

```html
<a href="tel:+441234567890">
    Call Us
</a>
```

---

# Image as a Link

Images can also be clickable.

```html
<a href="index.html">
    <img src="logo.png" alt="Logo">
</a>
```

---

# Bookmark Links

Bookmarks help users jump to another section of the same webpage.

### Step 1: Create an ID

```html
<h2 id="contact">Contact</h2>
```

### Step 2: Link to It

```html
<a href="#contact">
    Go to Contact Section
</a>
```

---

# Download Link

Use the `download` attribute.

```html
<a href="notes.pdf" download>
    Download Notes
</a>
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML Links</title>
</head>

<body>

<h1>TechVidyalaya</h1>

<a href="about.html">About</a>

<br><br>

<a href="https://www.google.com"
   target="_blank"
   rel="noopener noreferrer">
   Google
</a>

<br><br>

<a href="mailto:info@example.com">
    Email Us
</a>

</body>

</html>
```

---

# Common Mistakes

### Missing `href`

Incorrect:

```html
<a>Click Here</a>
```

Correct:

```html
<a href="index.html">Click Here</a>
```

---

### Invalid URL

Incorrect:

```html
<a href="google">
    Google
</a>
```

Correct:

```html
<a href="https://www.google.com">
    Google
</a>
```

---

# Best Practices

- Use meaningful link text.
- Avoid using "Click Here" as link text.
- Use relative links for pages within the same project.
- Use `target="_blank"` only when necessary.
- Add `rel="noopener noreferrer"` with external links opened in new tabs.
- Always provide descriptive text for accessibility.

---

# Quick Summary

- `<a>` creates hyperlinks.
- `href` specifies the destination.
- `target="_blank"` opens a new tab.
- `mailto:` creates email links.
- `tel:` creates phone links.
- `download` downloads files.
- Bookmarks allow navigation within the same page.

---

# Key Terms

| Term | Description |
|------|-------------|
| Anchor | HTML link element |
| Hyperlink | Clickable navigation |
| href | Destination URL |
| Absolute URL | Complete web address |
| Relative URL | Local project path |
| Bookmark | Link to a section of the same page |

---

# Practice Questions

### Multiple Choice

**1. Which HTML tag is used to create a hyperlink?**

A. `<link>`

B. `<href>`

C. `<a>`

D. `<url>`

**Answer:** C

---

**2. Which attribute specifies the destination of a link?**

A. `src`

B. `href`

C. `target`

D. `alt`

**Answer:** B

---

**3. Which attribute opens a link in a new browser tab?**

A. `new`

B. `blank`

C. `target="_blank"`

D. `window`

**Answer:** C

---

# Short Answer Questions

1. What is the purpose of the `<a>` tag?
2. What is the difference between absolute and relative URLs?
3. Why should `rel="noopener noreferrer"` be used with `target="_blank"`?
4. How do you create an email link?
5. What is a bookmark link?

---

# Hands-on Exercise

Create a webpage containing:

- A link to another local HTML page
- A link to Google that opens in a new tab
- An email link
- A phone link
- A bookmark link to a "Contact" section
- A download link for a PDF file

Open the page in your browser and test each link.

---

# Interview Questions

### Q1. What is the purpose of the `href` attribute?

The `href` attribute specifies the destination that the hyperlink points to.

---

### Q2. What is the difference between an absolute URL and a relative URL?

An absolute URL contains the full web address, while a relative URL points to a file within the same project.

---

### Q3. Why should meaningful link text be used?

Meaningful link text improves accessibility, user experience, and search engine optimisation by clearly describing the destination.

---

## Chapter Summary

In this chapter, you learned:

- How to create hyperlinks using the `<a>` tag
- The purpose of the `href` attribute
- The difference between absolute and relative URLs
- How to create email, phone, bookmark, and download links
- Best practices for writing accessible and secure HTML links

In the next chapter, we will learn about **HTML Images**.
