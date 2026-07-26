# Chapter 20: Mini Project – Personal Portfolio Website

## Learning Objectives

After completing this chapter, you will be able to:

- Build a complete HTML website
- Apply semantic HTML elements
- Create a professional webpage structure
- Organise content effectively
- Prepare the project for CSS and JavaScript
- Build a portfolio suitable for showcasing your skills

---

# Project Overview

In this mini project, you will build a **Personal Portfolio Website**.

The website will include:

- Header
- Navigation Menu
- About Section
- Skills Section
- Projects Section
- Contact Information
- Footer

By completing this project, you will apply everything learned in the HTML module.

---

# Project Folder Structure

```
portfolio/
│── index.html
│── images/
│     └── profile.jpg
```

---

# Website Layout

```
-----------------------------------------
|               Header                  |
-----------------------------------------
| Navigation Menu                       |
-----------------------------------------
| About Me                              |
-----------------------------------------
| Skills                                |
-----------------------------------------
| Projects                              |
-----------------------------------------
| Contact                               |
-----------------------------------------
| Footer                                |
-----------------------------------------
```

---

# Step 1: Create the HTML Structure

```html
<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta
        name="viewport"
        content="width=device-width, initial-scale=1.0">

    <title>My Portfolio</title>

</head>

<body>

</body>

</html>
```

---

# Step 2: Add the Header

```html
<header>

    <h1>John Doe</h1>

    <p>Java Full Stack Developer</p>

</header>
```

---

# Step 3: Add Navigation

```html
<nav>

    <a href="#about">About</a>

    <a href="#skills">Skills</a>

    <a href="#projects">Projects</a>

    <a href="#contact">Contact</a>

</nav>
```

---

# Step 4: About Section

```html
<section id="about">

<h2>About Me</h2>

<img
    src="images/profile.jpg"
    alt="Profile Photo"
    width="180">

<p>

I am a passionate software developer interested in Java, Web Development, and AI.

</p>

</section>
```

---

# Step 5: Skills Section

```html
<section id="skills">

<h2>Skills</h2>

<ul>

<li>HTML</li>

<li>CSS</li>

<li>JavaScript</li>

<li>Java</li>

<li>Spring Boot</li>

<li>SQL</li>

</ul>

</section>
```

---

# Step 6: Projects Section

```html
<section id="projects">

<h2>Projects</h2>

<article>

<h3>Student Management System</h3>

<p>
A Java application for managing student records.
</p>

</article>

<article>

<h3>Portfolio Website</h3>

<p>
A responsive personal portfolio website.
</p>

</article>

</section>
```

---

# Step 7: Contact Section

```html
<section id="contact">

<h2>Contact Me</h2>

<p>Email: john@example.com</p>

<p>Phone: +44 7000 123456</p>

</section>
```

---

# Step 8: Footer

```html
<footer>

<p>

© 2026 John Doe. All Rights Reserved.

</p>

</footer>
```

---

# Complete HTML Page

```html
<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta
name="viewport"
content="width=device-width, initial-scale=1.0">

<title>My Portfolio</title>

</head>

<body>

<header>

<h1>John Doe</h1>

<p>Java Full Stack Developer</p>

</header>

<nav>

<a href="#about">About</a>

<a href="#skills">Skills</a>

<a href="#projects">Projects</a>

<a href="#contact">Contact</a>

</nav>

<main>

<section id="about">

<h2>About Me</h2>

<img
src="images/profile.jpg"
alt="Profile Photo"
width="180">

<p>
Passionate software developer interested in Java and Web Development.
</p>

</section>

<section id="skills">

<h2>Skills</h2>

<ul>
<li>HTML</li>
<li>CSS</li>
<li>JavaScript</li>
<li>Java</li>
<li>Spring Boot</li>
</ul>

</section>

<section id="projects">

<h2>Projects</h2>

<article>

<h3>Portfolio Website</h3>

<p>Created using HTML.</p>

</article>

</section>

<section id="contact">

<h2>Contact</h2>

<p>Email: john@example.com</p>

</section>

</main>

<footer>

<p>© 2026 John Doe</p>

</footer>

</body>

</html>
```

---

# Possible Enhancements

You can improve this project later by adding:

- CSS styling
- Responsive design
- Animations
- Contact form
- Social media icons
- Download Resume button
- Dark mode
- JavaScript interactivity

---

# Common Mistakes

### Forgetting IDs for Navigation

Incorrect:

```html
<section>

<h2>About</h2>

</section>
```

Correct:

```html
<section id="about">

<h2>About</h2>

</section>
```

---

### Missing Image Alternative Text

Incorrect:

```html
<img src="profile.jpg">
```

Correct:

```html
<img
src="profile.jpg"
alt="Profile Photo">
```

---

# Best Practices

- Use semantic HTML elements.
- Keep navigation simple.
- Organise content into sections.
- Use meaningful headings.
- Add descriptive `alt` text to images.
- Validate your HTML before publishing.

---

# Quick Summary

- A portfolio showcases your skills and projects.
- Use semantic HTML for better structure.
- Organise content into logical sections.
- Navigation links improve usability.
- Keep the design simple and easy to read.

---

# Key Terms

| Term | Description |
|------|-------------|
| Portfolio | A personal website showcasing work and skills |
| Navigation | Links used to move between sections |
| Section | A logical grouping of related content |
| Article | Independent piece of content |
| Footer | Bottom section of a webpage |

---

# Practice Questions

### Multiple Choice

**1. Which element is best for the main navigation menu?**

A. `<div>`

B. `<nav>`

C. `<span>`

D. `<aside>`

**Answer:** B

---

**2. Which element is suitable for listing technical skills?**

A. `<ul>`

B. `<table>`

C. `<iframe>`

D. `<video>`

**Answer:** A

---

**3. Which section usually contains copyright information?**

A. `<header>`

B. `<main>`

C. `<footer>`

D. `<article>`

**Answer:** C

---

# Short Answer Questions

1. What is the purpose of a portfolio website?
2. Why should semantic elements be used?
3. Why are IDs important for navigation?
4. Which HTML element represents an independent project?
5. Name five sections commonly found in a portfolio website.

---

# Hands-on Exercise

Build your own portfolio website that includes:

- Header with your name
- Navigation menu
- About Me section
- Skills list
- At least three projects
- Contact details
- Footer

Validate the HTML and ensure all navigation links work correctly.

---

# Interview Questions

### Q1. Why is a portfolio website important for a developer?

A portfolio website demonstrates technical skills, showcases projects, and provides recruiters with a central place to learn about the developer's experience.

---

### Q2. Which semantic elements are commonly used in a portfolio website?

Common semantic elements include `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, and `<footer>`.

---

### Q3. How can this portfolio be improved later?

The portfolio can be enhanced by adding CSS for styling, JavaScript for interactivity, responsive layouts, animations, a contact form, and backend functionality.

---

## Chapter Summary

In this chapter, you built a complete HTML portfolio website using semantic elements and the concepts learned throughout this course. You organised content into sections, created navigation, displayed projects, and prepared the website for future enhancements using CSS and JavaScript.

In the next chapter, we will revise the entire HTML module with **HTML Interview Questions and Answers**.
