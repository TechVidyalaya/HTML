# Chapter 8: HTML Tables

## Learning Objectives

After completing this chapter, you will be able to:

- Understand HTML tables
- Create rows and columns
- Use table headers
- Merge rows and columns
- Add captions to tables
- Build well-structured tables
- Follow table best practices

---

# What is an HTML Table?

An HTML table is used to display data in rows and columns.

Examples include:

- Student records
- Employee details
- Product lists
- Timetables
- Marksheets

---

# Table Structure

An HTML table is created using the following tags:

| Tag | Purpose |
|------|---------|
| `<table>` | Creates the table |
| `<tr>` | Creates a table row |
| `<th>` | Creates a table header |
| `<td>` | Creates a table data cell |
| `<caption>` | Adds a table title |

---

# Basic Table

```html
<table>
    <tr>
        <td>Java</td>
        <td>Spring Boot</td>
    </tr>
</table>
```

Output:

```
-------------------------
| Java | Spring Boot |
-------------------------
```

---

# Table with Multiple Rows

```html
<table>

    <tr>
        <td>John</td>
        <td>22</td>
    </tr>

    <tr>
        <td>Alice</td>
        <td>24</td>
    </tr>

</table>
```

---

# Table Headers

Use the `<th>` tag for column headings.

```html
<table>

    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

    <tr>
        <td>John</td>
        <td>22</td>
    </tr>

</table>
```

Output:

```
---------------------
| Name | Age |
---------------------
| John | 22  |
---------------------
```

---

# Adding Borders

The `border` attribute is commonly used for learning purposes.

```html
<table border="1">

    <tr>
        <th>Name</th>
        <th>Course</th>
    </tr>

    <tr>
        <td>Rahul</td>
        <td>HTML</td>
    </tr>

</table>
```

> **Note:** In modern websites, CSS is used instead of the `border` attribute.

---

# Table Caption

The `<caption>` tag provides a title for the table.

```html
<table border="1">

    <caption>Student Details</caption>

    <tr>
        <th>Name</th>
        <th>Age</th>
    </tr>

</table>
```

---

# Column Span

The `colspan` attribute merges multiple columns.

```html
<table border="1">

<tr>
    <th colspan="2">
        Student Details
    </th>
</tr>

<tr>
    <td>Name</td>
    <td>Rahul</td>
</tr>

</table>
```

Output:

```
------------------------
| Student Details      |
------------------------
| Name | Rahul         |
------------------------
```

---

# Row Span

The `rowspan` attribute merges multiple rows.

```html
<table border="1">

<tr>
    <th rowspan="2">Name</th>
    <td>Rahul</td>
</tr>

<tr>
    <td>Rohan</td>
</tr>

</table>
```

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>Student Table</title>
</head>

<body>

<table border="1">

<caption>Student Details</caption>

<tr>
    <th>ID</th>
    <th>Name</th>
    <th>Course</th>
</tr>

<tr>
    <td>101</td>
    <td>Alice</td>
    <td>HTML</td>
</tr>

<tr>
    <td>102</td>
    <td>Bob</td>
    <td>CSS</td>
</tr>

<tr>
    <td>103</td>
    <td>Charlie</td>
    <td>JavaScript</td>
</tr>

</table>

</body>

</html>
```

---

# Modern Table Structure

HTML5 provides semantic tags for tables.

| Tag | Purpose |
|------|---------|
| `<thead>` | Header section |
| `<tbody>` | Table body |
| `<tfoot>` | Footer section |

Example:

```html
<table border="1">

<thead>
<tr>
    <th>Name</th>
    <th>Marks</th>
</tr>
</thead>

<tbody>
<tr>
    <td>Rahul</td>
    <td>90</td>
</tr>
</tbody>

<tfoot>
<tr>
    <td colspan="2">
        End of Report
    </td>
</tr>
</tfoot>

</table>
```

---

# Common Mistakes

### Forgetting Table Rows

Incorrect:

```html
<table>

<td>Java</td>

</table>
```

Correct:

```html
<table>

<tr>
    <td>Java</td>
</tr>

</table>
```

---

### Using `<td>` Instead of `<th>`

Incorrect:

```html
<tr>

<td>Name</td>

<td>Age</td>

</tr>
```

Correct:

```html
<tr>

<th>Name</th>

<th>Age</th>

</tr>
```

---

# Best Practices

- Use `<th>` for headings.
- Add a `<caption>` when appropriate.
- Use `<thead>`, `<tbody>`, and `<tfoot>` for large tables.
- Avoid using tables for page layout.
- Use CSS for styling instead of the `border` attribute.

---

# Quick Summary

- `<table>` creates a table.
- `<tr>` creates a row.
- `<th>` creates a header cell.
- `<td>` creates a data cell.
- `<caption>` adds a title.
- `colspan` merges columns.
- `rowspan` merges rows.
- `<thead>`, `<tbody>`, and `<tfoot>` improve table structure.

---

# Key Terms

| Term | Description |
|------|-------------|
| Table | Data arranged in rows and columns |
| Row | Horizontal group of cells |
| Column | Vertical group of cells |
| Header Cell | Column heading |
| Data Cell | Table content |
| Caption | Title of a table |

---

# Practice Questions

### Multiple Choice

**1. Which tag creates a table?**

A. `<tr>`

B. `<table>`

C. `<td>`

D. `<th>`

**Answer:** B

---

**2. Which tag creates a table header?**

A. `<td>`

B. `<thead>`

C. `<th>`

D. `<caption>`

**Answer:** C

---

**3. Which attribute merges two columns?**

A. `rowspan`

B. `merge`

C. `colspan`

D. `span`

**Answer:** C

---

# Short Answer Questions

1. What is the purpose of the `<table>` tag?
2. What is the difference between `<th>` and `<td>`?
3. What does the `colspan` attribute do?
4. What does the `rowspan` attribute do?
5. Why should tables not be used for webpage layouts?

---

# Hands-on Exercise

Create a webpage containing:

- A table with 5 students
- Columns for ID, Name, Course, and Marks
- A table caption
- One merged column using `colspan`
- One merged row using `rowspan`
- A table using `<thead>`, `<tbody>`, and `<tfoot>`

Open the webpage in your browser and verify the output.

---

# Interview Questions

### Q1. What is the difference between `<th>` and `<td>`?

`<th>` defines a table header cell, while `<td>` defines a normal data cell. Browsers usually display `<th>` content in bold and centred by default.

---

### Q2. What are `<thead>`, `<tbody>`, and `<tfoot>` used for?

They divide a table into header, body, and footer sections, making the table easier to read, style, and maintain.

---

### Q3. What is the purpose of `colspan` and `rowspan`?

- `colspan` merges multiple columns into a single cell.
- `rowspan` merges multiple rows into a single cell.

---

## Chapter Summary

In this chapter, you learned:

- How to create HTML tables
- The purpose of `<table>`, `<tr>`, `<th>`, `<td>`, and `<caption>`
- How to merge rows and columns
- How to structure tables using `<thead>`, `<tbody>`, and `<tfoot>`
- Best practices for creating clean and accessible tables

In the next chapter, we will learn about **HTML Forms**.
