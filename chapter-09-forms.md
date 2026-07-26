# Chapter 9: HTML Forms

## Learning Objectives

After completing this chapter, you will be able to:

- Understand HTML forms
- Create forms using different input elements
- Use labels for form controls
- Submit form data
- Organise form fields
- Follow form best practices

---

# What is an HTML Form?

An HTML form is used to collect information from users.

Examples include:

- Login forms
- Registration forms
- Contact forms
- Feedback forms
- Job application forms

The `<form>` tag is used to create a form.

---

# Basic Form Syntax

```html
<form>

</form>
```

All form elements are placed inside the `<form>` tag.

---

# Simple Form

```html
<form>

<label>Name:</label>

<input type="text">

</form>
```

Output:

```
Name: [____________]
```

---

# The `<label>` Tag

The `<label>` tag describes an input field.

```html
<label for="name">Name:</label>

<input type="text" id="name">
```

Using `for` and `id` improves accessibility.

---

# The `<input>` Tag

The `<input>` tag is used to receive user input.

Example:

```html
<input type="text">
```

---

# Form Attributes

| Attribute | Purpose |
|-----------|---------|
| `action` | Specifies where form data is sent |
| `method` | Specifies how data is sent |
| `autocomplete` | Enables or disables autocomplete |

Example:

```html
<form action="/submit" method="post">

</form>
```

---

# GET Method

The GET method sends form data through the URL.

```html
<form action="/search" method="get">
```

Example URL:

```
search.html?name=John
```

Suitable for:

- Search forms
- Filters

---

# POST Method

The POST method sends data in the request body.

```html
<form action="/register" method="post">
```

Suitable for:

- Registration
- Login
- Payments
- Sensitive information

---

# Text Input

```html
<label>Name:</label>

<input type="text">
```

---

# Password Input

```html
<label>Password:</label>

<input type="password">
```

Output:

```
Password: ********
```

---

# Email Input

```html
<label>Email:</label>

<input type="email">
```

The browser checks whether the entered value is a valid email address.

---

# Number Input

```html
<label>Age:</label>

<input type="number">
```

---

# Submit Button

```html
<input type="submit" value="Register">
```

Output:

```
[ Register ]
```

---

# Reset Button

```html
<input type="reset">
```

It clears all form fields.

---

# Placeholder

The `placeholder` attribute displays a hint.

```html
<input
    type="text"
    placeholder="Enter your name">
```

---

# Required Field

Use the `required` attribute.

```html
<input
    type="email"
    required>
```

The browser prevents form submission until a value is entered.

---

# Readonly Field

```html
<input
    type="text"
    value="Student"
    readonly>
```

The user can view but cannot edit the value.

---

# Disabled Field

```html
<input
    type="text"
    disabled>
```

The field cannot be edited or submitted.

---

# Complete Registration Form

```html
<!DOCTYPE html>
<html>

<head>
    <title>Registration Form</title>
</head>

<body>

<h2>Student Registration</h2>

<form action="/register" method="post">

<label for="name">Name:</label>

<input
    type="text"
    id="name"
    required>

<br><br>

<label for="email">Email:</label>

<input
    type="email"
    id="email"
    required>

<br><br>

<label for="password">Password:</label>

<input
    type="password"
    id="password"
    required>

<br><br>

<input
    type="submit"
    value="Register">

<input
    type="reset">

</form>

</body>

</html>
```

---

# Grouping Fields with `<fieldset>`

The `<fieldset>` tag groups related form controls.

```html
<fieldset>

<legend>Personal Information</legend>

<label>Name:</label>

<input type="text">

</fieldset>
```

---

# Common Mistakes

### Missing Label

Incorrect:

```html
<input type="text">
```

Correct:

```html
<label>Name:</label>

<input type="text">
```

---

### Forgetting the Method

Incorrect:

```html
<form action="/save">
```

Better:

```html
<form
    action="/save"
    method="post">
```

---

# Best Practices

- Always use labels.
- Use the correct input type.
- Use `required` where necessary.
- Prefer `POST` for sensitive information.
- Group related fields using `<fieldset>`.
- Keep forms simple and easy to understand.

---

# Quick Summary

- `<form>` creates a form.
- `<input>` receives user input.
- `<label>` describes an input field.
- `action` specifies where data is sent.
- `method` specifies how data is submitted.
- `GET` sends data in the URL.
- `POST` sends data securely in the request body.

---

# Key Terms

| Term | Description |
|------|-------------|
| Form | Collects user input |
| Input | Field for entering data |
| Label | Describes an input field |
| GET | Sends data in the URL |
| POST | Sends data in the request body |
| Fieldset | Groups related form fields |

---

# Practice Questions

### Multiple Choice

**1. Which tag is used to create a form?**

A. `<input>`

B. `<form>`

C. `<fieldset>`

D. `<label>`

**Answer:** B

---

**2. Which method is recommended for submitting passwords?**

A. GET

B. POST

C. PUT

D. LINK

**Answer:** B

---

**3. Which attribute makes a field mandatory?**

A. `readonly`

B. `disabled`

C. `required`

D. `placeholder`

**Answer:** C

---

# Short Answer Questions

1. What is the purpose of the `<form>` tag?
2. What is the difference between GET and POST?
3. Why should labels be used with input fields?
4. What does the `required` attribute do?
5. What is the purpose of the `<fieldset>` tag?

---

# Hands-on Exercise

Create a **Student Registration Form** with:

- Name
- Email
- Password
- Age
- Submit button
- Reset button

Use:

- Labels
- Required fields
- Placeholder text
- Fieldset and Legend

Run the webpage and test the form.

---

# Interview Questions

### Q1. What is the purpose of the `action` attribute?

The `action` attribute specifies the URL where the form data will be sent after submission.

---

### Q2. What is the difference between GET and POST?

- **GET** sends data through the URL and is suitable for non-sensitive information.
- **POST** sends data in the request body and is recommended for sensitive or large amounts of data.

---

### Q3. Why is the `<label>` tag important?

The `<label>` tag improves accessibility, makes forms easier to use, and allows users to focus an input by clicking its label.

---

## Chapter Summary

In this chapter, you learned:

- How to create HTML forms
- The purpose of the `<form>`, `<input>`, and `<label>` tags
- The difference between GET and POST methods
- How to use attributes such as `required`, `placeholder`, `readonly`, and `disabled`
- Best practices for building user-friendly and accessible forms

In the next chapter, we will explore the various **HTML Input Types** in detail.
