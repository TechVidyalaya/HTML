# Chapter 18: HTML5 APIs

## Learning Objectives

After completing this chapter, you will be able to:

- Understand what HTML5 APIs are
- Learn about common HTML5 APIs
- Use the Geolocation API
- Store data using Web Storage
- Understand Drag and Drop
- Explore Canvas and Web Workers
- Follow best practices when using HTML5 APIs

---

# What are HTML5 APIs?

HTML5 introduced several **Application Programming Interfaces (APIs)** that allow web applications to access browser features without additional plugins.

Some popular HTML5 APIs are:

- Geolocation API
- Web Storage API
- Drag and Drop API
- Canvas API
- Web Workers API

These APIs make websites more interactive and powerful.

---

# Geolocation API

The **Geolocation API** allows a webpage to access the user's current location (with permission).

Example:

```html
<button onclick="getLocation()">
    Get Location
</button>

<p id="location"></p>

<script>
function getLocation() {
    navigator.geolocation.getCurrentPosition(function(position) {
        document.getElementById("location").innerHTML =
            "Latitude: " + position.coords.latitude +
            "<br>Longitude: " + position.coords.longitude;
    });
}
</script>
```

> **Note:** The browser asks the user for permission before sharing their location.

---

# Web Storage API

The Web Storage API stores data directly in the browser.

It provides two storage options:

- `localStorage`
- `sessionStorage`

---

# localStorage

`localStorage` stores data even after the browser is closed.

Store data:

```javascript
localStorage.setItem("username", "John");
```

Retrieve data:

```javascript
let name = localStorage.getItem("username");
```

Remove data:

```javascript
localStorage.removeItem("username");
```

---

# sessionStorage

`sessionStorage` stores data only while the browser tab is open.

```javascript
sessionStorage.setItem("course", "HTML");
```

Retrieve:

```javascript
sessionStorage.getItem("course");
```

---

# localStorage vs sessionStorage

| localStorage | sessionStorage |
|--------------|----------------|
| Permanent until removed | Cleared when the tab closes |
| Shared across browser tabs (same origin) | Available only in the current tab |
| Suitable for user preferences | Suitable for temporary session data |

---

# Drag and Drop API

The Drag and Drop API allows users to drag elements and drop them onto another element.

Example:

```html
<div draggable="true">
    Drag Me
</div>
```

Common events include:

- `dragstart`
- `dragover`
- `drop`

---

# Canvas API

The `<canvas>` element is used to draw graphics using JavaScript.

Example:

```html
<canvas
    id="myCanvas"
    width="300"
    height="150">
</canvas>

<script>
const canvas = document.getElementById("myCanvas");
const ctx = canvas.getContext("2d");

ctx.fillStyle = "blue";
ctx.fillRect(20, 20, 120, 80);
</script>
```

Output:

```
+---------------------------+
|                           |
|  █████████████            |
|                           |
+---------------------------+
```

---

# Web Workers API

Web Workers allow JavaScript to run in the background without blocking the webpage.

Benefits:

- Improves performance
- Keeps the UI responsive
- Suitable for long-running tasks

Example:

```javascript
const worker = new Worker("worker.js");
```

---

# HTML5 Audio and Video APIs

HTML5 also provides JavaScript methods to control media.

Example:

```javascript
const video = document.getElementById("myVideo");

video.play();

video.pause();
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML5 APIs</title>
</head>

<body>

<button onclick="saveData()">
    Save Name
</button>

<script>

function saveData() {

    localStorage.setItem("username", "TechVidyalaya");

    alert("Data Saved!");

}

</script>

</body>

</html>
```

---

# Common Mistakes

### Accessing Geolocation Without Permission

Incorrect:

```javascript
navigator.geolocation.getCurrentPosition(...);
```

Always handle permission requests and possible errors.

---

### Storing Sensitive Information

Incorrect:

```javascript
localStorage.setItem("password", "123456");
```

Never store passwords or sensitive personal data in browser storage.

---

### Assuming Web Storage Never Expires

Remember:

- `localStorage` remains until removed.
- `sessionStorage` is cleared when the browser tab closes.

---

# Best Practices

- Always request user permission when using Geolocation.
- Store only non-sensitive data in Web Storage.
- Use `localStorage` for long-term preferences.
- Use `sessionStorage` for temporary session information.
- Use Web Workers for CPU-intensive tasks.
- Keep Canvas drawings efficient for better performance.

---

# Quick Summary

- HTML5 APIs extend browser capabilities.
- Geolocation provides user location (with permission).
- `localStorage` stores persistent data.
- `sessionStorage` stores temporary data.
- Canvas draws graphics.
- Drag and Drop enables interactive interfaces.
- Web Workers improve performance.

---

# Key Terms

| Term | Description |
|------|-------------|
| HTML5 API | Browser feature accessible through JavaScript |
| Geolocation | User's geographic location |
| localStorage | Persistent browser storage |
| sessionStorage | Temporary browser storage |
| Canvas | HTML element for drawing graphics |
| Web Worker | Background JavaScript thread |

---

# Practice Questions

### Multiple Choice

**1. Which API is used to store data permanently in the browser?**

A. sessionStorage

B. localStorage

C. Cookies

D. Clipboard API

**Answer:** B

---

**2. Which API is used to access the user's location?**

A. Canvas API

B. Drag and Drop API

C. Geolocation API

D. Storage API

**Answer:** C

---

**3. Which HTML element is used for drawing graphics?**

A. `<graphics>`

B. `<draw>`

C. `<canvas>`

D. `<paint>`

**Answer:** C

---

# Short Answer Questions

1. What are HTML5 APIs?
2. What is the difference between `localStorage` and `sessionStorage`?
3. Why is permission required for the Geolocation API?
4. What is the purpose of the Canvas API?
5. How do Web Workers improve application performance?

---

# Hands-on Exercise

Create a webpage that:

- Saves a username using `localStorage`
- Displays the saved username
- Includes a button to get the user's location
- Draws a rectangle using the Canvas API
- Creates a draggable element

Run the webpage and observe how each HTML5 API works.

---

# Interview Questions

### Q1. What are HTML5 APIs?

HTML5 APIs are browser-provided interfaces that allow web applications to use features such as storage, location services, graphics, media, and background processing.

---

### Q2. What is the difference between `localStorage` and `sessionStorage`?

`localStorage` persists data until it is removed, while `sessionStorage` stores data only for the current browser tab or session.

---

### Q3. Why should sensitive data not be stored in `localStorage`?

Data stored in `localStorage` is accessible through JavaScript running on the same origin and is not encrypted by default. Sensitive information such as passwords or authentication tokens should be stored securely using appropriate server-side mechanisms.

---

## Chapter Summary

In this chapter, you learned:

- What HTML5 APIs are
- How the Geolocation API works
- The difference between `localStorage` and `sessionStorage`
- The basics of the Canvas, Drag and Drop, and Web Workers APIs
- Best practices for using HTML5 APIs securely and efficiently

In the next chapter, we will learn about **HTML Best Practices**.
