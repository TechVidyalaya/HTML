# Chapter 16: HTML Entities and Symbols

## Learning Objectives

After completing this chapter, you will be able to:

- Understand HTML entities
- Display reserved characters in HTML
- Use common HTML symbols
- Insert emojis using HTML
- Follow best practices for special characters

---

# What are HTML Entities?

Some characters have a special meaning in HTML and cannot be displayed directly.

For example:

- `<` starts an HTML tag.
- `>` ends an HTML tag.
- `&` begins an HTML entity.

To display these characters as text, HTML entities are used.

---

# Entity Syntax

HTML entities can be written using:

- Entity Name
- Entity Number

Example:

```html
&lt;
```

or

```html
&#60;
```

Both display:

```
<
```

---

# Why Use HTML Entities?

HTML entities help to:

- Display reserved characters
- Show mathematical symbols
- Display currency symbols
- Add copyright and trademark symbols
- Insert emojis and special icons

---

# Common HTML Entities

| Character | Entity Name | Entity Number |
|-----------|-------------|---------------|
| `<` | `&lt;` | `&#60;` |
| `>` | `&gt;` | `&#62;` |
| `&` | `&amp;` | `&#38;` |
| `"` | `&quot;` | `&#34;` |
| `'` | `&apos;` | `&#39;` |

---

# Displaying HTML Code

Without entities:

```html
<p>This is <b>bold</b></p>
```

The browser interprets `<b>` as an HTML tag.

Using entities:

```html
&lt;b&gt;Bold&lt;/b&gt;
```

Output:

```
<b>Bold</b>
```

---

# Non-Breaking Space

The `&nbsp;` entity creates a space that the browser does not collapse.

Example:

```html
Tech&nbsp;Vidyalaya
```

Output:

```
Tech Vidyalaya
```

The two words stay together on the same line.

---

# Copyright Symbol

```html
&copy;
```

Output:

```
©
```

---

# Trademark Symbol

```html
&trade;
```

Output:

```
™
```

---

# Registered Symbol

```html
&reg;
```

Output:

```
®
```

---

# Currency Symbols

```html
&pound;
```

Output:

```
£
```

```html
&euro;
```

Output:

```
€
```

```html
&#8377;
```

Output:

```
₹
```

---

# Mathematical Symbols

```html
&plusmn;
```

Output:

```
±
```

```html
&times;
```

Output:

```
×
```

```html
&divide;
```

Output:

```
÷
```

```html
&deg;
```

Output:

```
°
```

---

# Arrows

```html
&rarr;
```

Output:

```
→
```

```html
&larr;
```

Output:

```
←
```

```html
&uarr;
```

Output:

```
↑
```

```html
&darr;
```

Output:

```
↓
```

---

# Emojis in HTML

HTML supports Unicode emojis.

Example:

```html
<p>&#128512;</p>
```

Output:

```
😀
```

Another example:

```html
<p>&#128640;</p>
```

Output:

```
🚀
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML Entities</title>
</head>

<body>

<h2>Special Characters</h2>

<p>&lt;HTML&gt;</p>

<p>&copy; 2026 TechVidyalaya</p>

<p>Price: &#8377;999</p>

<p>Temperature: 30&deg;C</p>

<p>Success &check;</p>

<p>Rocket: &#128640;</p>

</body>

</html>
```

---

# Common Mistakes

### Using Reserved Characters Directly

Incorrect:

```html
<p>5 < 10</p>
```

Correct:

```html
<p>5 &lt; 10</p>
```

---

### Forgetting the Semicolon

Incorrect:

```html
&copy
```

Correct:

```html
&copy;
```

---

# Best Practices

- Use entities for reserved HTML characters.
- Always end entities with a semicolon (`;`).
- Use Unicode for emojis.
- Use named entities where possible for readability.
- Test symbols across different browsers.

---

# Quick Summary

- HTML entities display reserved and special characters.
- `&lt;` displays `<`.
- `&gt;` displays `>`.
- `&amp;` displays `&`.
- `&copy;`, `&reg;`, and `&trade;` display legal symbols.
- Unicode numbers can be used for emojis.

---

# Key Terms

| Term | Description |
|------|-------------|
| HTML Entity | A code representing a special character |
| Reserved Character | Character with special meaning in HTML |
| Unicode | Universal character encoding standard |
| Non-Breaking Space | Prevents automatic line breaks |
| Entity Name | Text representation such as `&copy;` |

---

# Practice Questions

### Multiple Choice

**1. Which entity displays the `<` symbol?**

A. `&gt;`

B. `&lt;`

C. `&amp;`

D. `&copy;`

**Answer:** B

---

**2. Which entity displays the copyright symbol?**

A. `&copy;`

B. `&reg;`

C. `&trade;`

D. `&deg;`

**Answer:** A

---

**3. What is the purpose of `&nbsp;`?**

A. Adds a new line

B. Creates a non-breaking space

C. Displays a tab

D. Displays a quotation mark

**Answer:** B

---

# Short Answer Questions

1. What is an HTML entity?
2. Why are HTML entities required?
3. What is the difference between an entity name and an entity number?
4. What is a non-breaking space?
5. How do you display the copyright symbol?

---

# Hands-on Exercise

Create a webpage that displays:

- The `<`, `>`, and `&` characters
- A copyright notice
- Trademark and registered symbols
- Three currency symbols
- Three mathematical symbols
- Two emojis

Run the webpage and verify that all symbols are displayed correctly.

---

# Interview Questions

### Q1. Why are HTML entities used?

HTML entities are used to display reserved characters and special symbols that would otherwise be interpreted as HTML code.

---

### Q2. What is the difference between `&lt;` and `<`?

`<` is interpreted as the start of an HTML tag, while `&lt;` displays the less-than symbol as plain text.

---

### Q3. What is the purpose of `&nbsp;`?

`&nbsp;` creates a non-breaking space, preventing the browser from splitting words across different lines.

---

## Chapter Summary

In this chapter, you learned:

- What HTML entities are
- How to display reserved characters
- Common symbols and currency entities
- How to use Unicode emojis
- Best practices for using special characters in HTML

In the next chapter, we will learn about **HTML Accessibility**.
