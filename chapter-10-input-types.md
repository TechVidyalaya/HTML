# Chapter 10: HTML Input Types

## Learning Objectives

After completing this chapter, you will be able to:

- Understand different HTML input types
- Choose the appropriate input type for user data
- Use built-in browser validation
- Create user-friendly forms
- Follow best practices for form inputs

---

# What are Input Types?

The `<input>` tag supports different **input types**.

Each type is designed to collect a specific kind of information.

Example:

```html
<input type="text">
```

---

# Common HTML Input Types

| Input Type | Purpose |
|------------|---------|
| text | Single-line text |
| password | Password input |
| email | Email address |
| number | Numeric values |
| tel | Telephone number |
| url | Website URL |
| search | Search box |
| date | Select a date |
| time | Select a time |
| datetime-local | Date and time |
| color | Colour picker |
| range | Slider |
| radio | Single selection |
| checkbox | Multiple selections |
| file | Upload files |
| hidden | Hidden data |
| submit | Submit form |
| reset | Reset form |
| button | Generic button |

---

# Text Input

```html
<label>Name:</label>

<input type="text">
```

Output:

```
Name: [____________]
```

---

# Password Input

```html
<label>Password:</label>

<input type="password">
```

Characters are hidden while typing.

---

# Email Input

```html
<label>Email:</label>

<input type="email">
```

The browser validates the email format.

---

# Number Input

```html
<label>Age:</label>

<input
    type="number"
    min="18"
    max="60">
```

---

# Telephone Input

```html
<label>Phone:</label>

<input type="tel">
```

Useful for mobile numbers.

---

# URL Input

```html
<label>Website:</label>

<input type="url">
```

Example:

```
https://www.example.com
```

---

# Search Input

```html
<input
    type="search"
    placeholder="Search...">
```

Used for search boxes.

---

# Date Input

```html
<input type="date">
```

Displays a calendar picker.

---

# Time Input

```html
<input type="time">
```

Allows users to select a time.

---

# Date and Time

```html
<input type="datetime-local">
```

Allows users to select both date and time.

---

# Colour Picker

```html
<input type="color">
```

Displays a colour selection dialog.

---

# Range Slider

```html
<input
    type="range"
    min="0"
    max="100">
```

Useful for selecting values within a range.

---

# Radio Buttons

Radio buttons allow only one option to be selected.

```html
<label>

<input
    type="radio"
    name="gender">

Male

</label>

<label>

<input
    type="radio"
    name="gender">

Female

</label>
```

---

# Checkboxes

Checkboxes allow multiple selections.

```html
<label>

<input type="checkbox">

Java

</label>

<label>

<input type="checkbox">

Python

</label>
```

---

# File Upload

```html
<input type="file">
```

Allows users to upload files.

---

# Hidden Input

```html
<input
    type="hidden"
    name="userId"
    value="101">
```

The field is not visible to the user.

---

# Submit Button

```html
<input
    type="submit"
    value="Save">
```

---

# Reset Button

```html
<input
    type="reset"
    value="Clear">
```

---

# Generic Button

```html
<input
    type="button"
    value="Click Me">
```

Typically used with JavaScript.

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>Input Types</title>
</head>

<body>

<form>

<label>Name:</label>

<input type="text">

<br><br>

<label>Email:</label>

<input type="email">

<br><br>

<label>Password:</label>

<input type="password">

<br><br>

<label>Age:</label>

<input type="number">

<br><br>

<label>Date of Birth:</label>

<input type="date">

<br><br>

<label>Gender:</label>

<input
    type="radio"
    name="gender"> Male

<input
    type="radio"
    name="gender"> Female

<br><br>

<label>Skills:</label>

<input type="checkbox"> HTML

<input type="checkbox"> CSS

<input type="checkbox"> JavaScript

<br><br>

<input
    type="submit"
    value="Register">

</form>

</body>

</html>
```

---

# Common Input Attributes

| Attribute | Purpose |
|-----------|---------|
| placeholder | Displays hint text |
| required | Makes field mandatory |
| readonly | Prevents editing |
| disabled | Disables the field |
| value | Sets the default value |
| min | Minimum value |
| max | Maximum value |
| maxlength | Maximum number of characters |
| minlength | Minimum number of characters |
| step | Increment value |

Example:

```html
<input
    type="number"
    min="1"
    max="100"
    step="5">
```

---

# Common Mistakes

### Using the Wrong Input Type

Incorrect:

```html
<input type="text">
```

For email addresses, use:

```html
<input type="email">
```

---

### Missing Name Attribute

Incorrect:

```html
<input type="text">
```

Correct:

```html
<input
    type="text"
    name="username">
```

The `name` attribute is required when submitting form data.

---

# Best Practices

- Use the correct input type.
- Always provide labels.
- Use browser validation where possible.
- Keep forms simple.
- Use meaningful placeholders.
- Add `required` for mandatory fields.

---

# Quick Summary

- HTML provides many input types.
- Each input type is designed for specific data.
- Browser validation improves user experience.
- Radio buttons allow one selection.
- Checkboxes allow multiple selections.
- File inputs enable file uploads.

---

# Key Terms

| Term | Description |
|------|-------------|
| Input Type | Type of user input |
| Radio Button | Single-choice option |
| Checkbox | Multiple-choice option |
| Placeholder | Hint text |
| Validation | Ensures correct input |

---

# Practice Questions

### Multiple Choice

**1. Which input type is used for passwords?**

A. text

B. password

C. email

D. hidden

**Answer:** B

---

**2. Which input type displays a calendar?**

A. datetime

B. date

C. calendar

D. month

**Answer:** B

---

**3. Which input type allows users to upload a file?**

A. upload

B. image

C. file

D. attachment

**Answer:** C

---

# Short Answer Questions

1. What is the purpose of the `email` input type?
2. What is the difference between radio buttons and checkboxes?
3. Why is the `name` attribute important?
4. What does the `required` attribute do?
5. Which input type is used for selecting a colour?

---

# Hands-on Exercise

Create a **Student Registration Form** containing:

- Name
- Email
- Password
- Mobile Number
- Date of Birth
- Favourite Colour
- Skills (Checkboxes)
- Gender (Radio Buttons)
- Resume Upload
- Submit Button

Test the form in your browser and observe the built-in validation.

---

# Interview Questions

### Q1. Why should you use specialised HTML input types instead of only `text`?

Specialised input types provide better user experience, built-in validation, and appropriate keyboards or controls on different devices.

---

### Q2. What is the difference between radio buttons and checkboxes?

Radio buttons allow users to select only one option from a group, while checkboxes allow multiple selections.

---

### Q3. What is the purpose of the `name` attribute?

The `name` attribute identifies form fields when data is submitted to the server. Without it, the field's value is not included in the submitted form data.

---

## Chapter Summary

In this chapter, you learned:

- The different HTML input types
- How to collect different kinds of user input
- The purpose of common input attributes
- The difference between radio buttons and checkboxes
- Best practices for creating user-friendly forms

In the next chapter, we will learn about **HTML Semantic Elements**.
