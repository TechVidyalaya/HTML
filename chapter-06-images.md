# Chapter 6: HTML Images

## Learning Objectives

After completing this chapter, you will be able to:

- Add images to a webpage
- Understand the `<img>` tag and its attributes
- Use local and online images
- Resize images
- Add alternative text
- Create clickable images
- Follow image best practices

---

# What are HTML Images?

Images make webpages more attractive and engaging.

HTML uses the `<img>` tag to display images.

Unlike most HTML elements, the `<img>` tag does **not** have a closing tag.

---

# Basic Syntax

```html
<img src="image.jpg" alt="Description">
```

### Output

The browser displays the image.

---

# The `src` Attribute

The `src` (source) attribute specifies the location of the image.

```html
<img src="nature.jpg" alt="Nature">
```

---

# The `alt` Attribute

The `alt` attribute provides alternative text if the image cannot be displayed.

It is also used by screen readers for accessibility.

```html
<img src="student.jpg" alt="Student Learning HTML">
```

---

# Local Image

If the image is inside your project folder:

```
project/
│── index.html
│── images/
      └── logo.png
```

HTML:

```html
<img src="images/logo.png" alt="Company Logo">
```

---

# Online Image

You can also display an image from the internet.

```html
<img src="https://example.com/image.jpg"
     alt="Sample Image">
```

---

# Setting Image Width

```html
<img src="flower.jpg"
     alt="Flower"
     width="300">
```

---

# Setting Image Height

```html
<img src="flower.jpg"
     alt="Flower"
     height="200">
```

---

# Setting Both Width and Height

```html
<img src="flower.jpg"
     alt="Flower"
     width="300"
     height="200">
```

---

# Using CSS for Responsive Images

Instead of fixed sizes, use CSS.

```html
<img src="nature.jpg"
     alt="Nature"
     style="width:100%; max-width:500px;">
```

This allows the image to resize on different screen sizes.

---

# Image Title

The `title` attribute displays a tooltip when the user hovers over the image.

```html
<img src="logo.png"
     alt="Logo"
     title="TechVidyalaya Logo">
```

---

# Clickable Image

Images can be used as links.

```html
<a href="index.html">
    <img src="logo.png"
         alt="Home">
</a>
```

Clicking the image opens the linked page.

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML Images</title>
</head>

<body>

<h1>Welcome</h1>

<img src="images/student.jpg"
     alt="Student Learning HTML"
     width="400">

</body>

</html>
```

---

# Supported Image Formats

| Format | Extension |
|---------|-----------|
| JPEG | `.jpg`, `.jpeg` |
| PNG | `.png` |
| GIF | `.gif` |
| SVG | `.svg` |
| WebP | `.webp` |

---

# Image Folder Structure

```
website/
│── index.html
│── about.html
│── images/
│     ├── logo.png
│     ├── banner.jpg
│     └── profile.webp
```

---

# Common Mistakes

### Missing `alt`

Incorrect:

```html
<img src="logo.png">
```

Correct:

```html
<img src="logo.png"
     alt="Company Logo">
```

---

### Incorrect Image Path

Incorrect:

```html
<img src="logo.png">
```

Correct (if stored in an images folder):

```html
<img src="images/logo.png">
```

---

### Distorted Images

Incorrect:

```html
<img src="photo.jpg"
     width="400"
     height="50">
```

This may stretch or squash the image.

---

# Best Practices

- Always provide an `alt` attribute.
- Store images in a separate `images` folder.
- Use descriptive file names.
- Optimise images to reduce file size.
- Prefer responsive sizing using CSS.
- Use WebP where supported for better performance.

---

# Quick Summary

- `<img>` displays images.
- `src` specifies the image location.
- `alt` provides alternative text.
- `width` and `height` control image size.
- Images can be used as hyperlinks.
- Organise images inside an `images` folder.

---

# Key Terms

| Term | Description |
|------|-------------|
| Image | Visual content displayed on a webpage |
| src | Image source path |
| alt | Alternative text |
| width | Image width |
| height | Image height |
| Responsive Image | Image that adjusts to screen size |

---

# Practice Questions

### Multiple Choice

**1. Which tag is used to display an image?**

A. `<image>`

B. `<picture>`

C. `<img>`

D. `<photo>`

**Answer:** C

---

**2. Which attribute specifies the image location?**

A. `href`

B. `src`

C. `path`

D. `link`

**Answer:** B

---

**3. Why is the `alt` attribute important?**

A. It changes the image colour.

B. It resizes the image.

C. It provides alternative text and improves accessibility.

D. It makes the image downloadable.

**Answer:** C

---

# Short Answer Questions

1. What is the purpose of the `<img>` tag?
2. What does the `src` attribute do?
3. Why should every image have an `alt` attribute?
4. Name three commonly used image formats.
5. How can an image be made clickable?

---

# Hands-on Exercise

Create a webpage containing:

- One local image
- One online image
- A resized image
- A clickable logo that links to the home page
- An image with a tooltip using the `title` attribute

Run the webpage and verify the output.

---

# Interview Questions

### Q1. What is the purpose of the `alt` attribute?

The `alt` attribute provides alternative text if the image cannot be displayed and improves accessibility for users who rely on screen readers.

---

### Q2. What is the difference between JPEG and PNG?

- **JPEG** is best for photographs because it offers good compression.
- **PNG** supports transparency and is suitable for logos and icons.

---

### Q3. Why should images be optimised before adding them to a website?

Optimised images load faster, improve website performance, reduce bandwidth usage, and provide a better user experience.

---

## Chapter Summary

In this chapter, you learned:

- How to display images using the `<img>` tag
- The purpose of the `src`, `alt`, `width`, `height`, and `title` attributes
- How to use local and online images
- How to create clickable images
- Best practices for using images in HTML

In the next chapter, we will learn about **HTML Lists**.
