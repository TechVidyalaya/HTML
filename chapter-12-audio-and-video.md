# Chapter 12: HTML Audio and Video

## Learning Objectives

After completing this chapter, you will be able to:

- Add audio to a webpage
- Embed videos using HTML
- Understand audio and video attributes
- Support multiple media formats
- Embed YouTube videos
- Follow best practices for multimedia content

---

# What are HTML Multimedia Elements?

HTML5 introduced built-in support for multimedia.

The two main multimedia elements are:

- `<audio>` – Plays audio files
- `<video>` – Plays video files

These elements allow browsers to play media without additional plugins.

---

# Supported Audio Formats

| Format | Extension |
|---------|-----------|
| MP3 | `.mp3` |
| WAV | `.wav` |
| OGG | `.ogg` |

---

# Supported Video Formats

| Format | Extension |
|---------|-----------|
| MP4 | `.mp4` |
| WebM | `.webm` |
| OGG | `.ogv` |

---

# HTML Audio

The `<audio>` tag is used to play audio files.

```html
<audio controls>
    <source src="music.mp3" type="audio/mpeg">
</audio>
```

Output:

```
▶️ Audio Player
```

---

# The `controls` Attribute

The `controls` attribute displays the built-in audio player.

```html
<audio controls>
    <source src="song.mp3" type="audio/mpeg">
</audio>
```

The player includes:

- Play
- Pause
- Volume
- Progress bar

---

# Autoplay Audio

```html
<audio autoplay>
    <source src="song.mp3" type="audio/mpeg">
</audio>
```

> **Note:** Most modern browsers block autoplay unless the audio is muted or the user has interacted with the page.

---

# Loop Audio

```html
<audio controls loop>
    <source src="music.mp3" type="audio/mpeg">
</audio>
```

The audio automatically starts again after finishing.

---

# Muted Audio

```html
<audio controls muted>
    <source src="music.mp3" type="audio/mpeg">
</audio>
```

The audio starts in muted mode.

---

# Multiple Audio Formats

```html
<audio controls>

    <source src="music.mp3" type="audio/mpeg">

    <source src="music.ogg" type="audio/ogg">

    Your browser does not support audio.

</audio>
```

The browser uses the first supported format.

---

# HTML Video

The `<video>` tag is used to play videos.

```html
<video controls width="500">

    <source src="video.mp4" type="video/mp4">

</video>
```

Output:

```
▶️ Video Player
```

---

# Video Width and Height

```html
<video
    width="600"
    height="350"
    controls>

    <source src="movie.mp4"
            type="video/mp4">

</video>
```

---

# Autoplay Video

```html
<video autoplay muted>

    <source src="intro.mp4"
            type="video/mp4">

</video>
```

> Browsers usually require `muted` when autoplay is enabled.

---

# Loop Video

```html
<video controls loop>

    <source src="demo.mp4"
            type="video/mp4">

</video>
```

---

# Poster Image

The `poster` attribute displays an image before the video starts.

```html
<video
    controls
    poster="thumbnail.jpg">

    <source src="course.mp4"
            type="video/mp4">

</video>
```

---

# Multiple Video Formats

```html
<video controls>

    <source src="video.mp4" type="video/mp4">

    <source src="video.webm" type="video/webm">

    Your browser does not support video.

</video>
```

---

# Embedding a YouTube Video

YouTube videos are embedded using an `<iframe>`.

```html
<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/VIDEO_ID"
    title="YouTube video"
    allowfullscreen>
</iframe>
```

Replace `VIDEO_ID` with the actual YouTube video ID.

---

# Complete Example

```html
<!DOCTYPE html>
<html>

<head>
    <title>HTML Multimedia</title>
</head>

<body>

<h2>Audio Example</h2>

<audio controls>

    <source src="music.mp3"
            type="audio/mpeg">

</audio>

<hr>

<h2>Video Example</h2>

<video
    width="500"
    controls
    poster="thumbnail.jpg">

    <source src="course.mp4"
            type="video/mp4">

</video>

</body>

</html>
```

---

# Common Mistakes

### Forgetting the `controls` Attribute

Incorrect:

```html
<audio>

    <source src="song.mp3">

</audio>
```

Correct:

```html
<audio controls>

    <source src="song.mp3">

</audio>
```

---

### Using Unsupported Formats

Always provide common formats such as MP3 for audio and MP4 for video.

---

# Best Practices

- Use MP3 for audio whenever possible.
- Use MP4 for videos for maximum compatibility.
- Provide multiple media formats if needed.
- Use the `poster` attribute for videos.
- Avoid autoplay unless necessary.
- Optimise media files to improve loading speed.
- Always include fallback text inside `<audio>` and `<video>` tags.

---

# Quick Summary

- `<audio>` plays audio files.
- `<video>` plays video files.
- `controls` displays playback controls.
- `autoplay` starts media automatically.
- `loop` repeats playback.
- `muted` starts media without sound.
- `poster` displays a preview image.
- `<iframe>` is used to embed YouTube videos.

---

# Key Terms

| Term | Description |
|------|-------------|
| Audio | Sound played on a webpage |
| Video | Moving visual media |
| Controls | Built-in playback buttons |
| Poster | Preview image for a video |
| Source | Media file location |
| Iframe | Embeds external content |

---

# Practice Questions

### Multiple Choice

**1. Which tag is used to play audio?**

A. `<music>`

B. `<audio>`

C. `<sound>`

D. `<media>`

**Answer:** B

---

**2. Which attribute displays playback controls?**

A. `play`

B. `controller`

C. `controls`

D. `media`

**Answer:** C

---

**3. Which HTML element is commonly used to embed a YouTube video?**

A. `<video>`

B. `<embed>`

C. `<iframe>`

D. `<object>`

**Answer:** C

---

# Short Answer Questions

1. What is the purpose of the `<audio>` tag?
2. What is the purpose of the `controls` attribute?
3. What does the `poster` attribute do?
4. Why are multiple `<source>` elements sometimes used?
5. How do you embed a YouTube video in HTML?

---

# Hands-on Exercise

Create a webpage containing:

- One audio player
- One video player
- A poster image for the video
- A looping audio file
- An embedded YouTube video using an `<iframe>`

Run the webpage and test all multimedia elements.

---

# Interview Questions

### Q1. What is the difference between the `<audio>` and `<video>` tags?

The `<audio>` tag is used to play sound files, while the `<video>` tag is used to play video files with both audio and visual content.

---

### Q2. Why should multiple `<source>` elements be provided?

Different browsers support different media formats. Multiple `<source>` elements improve compatibility by allowing the browser to choose a supported format.

---

### Q3. What is the purpose of the `poster` attribute?

The `poster` attribute specifies an image displayed before the video starts playing, providing users with a preview of the video.

---

## Chapter Summary

In this chapter, you learned:

- How to add audio and video to webpages
- The purpose of common multimedia attributes
- How to support multiple media formats
- How to embed YouTube videos
- Best practices for using multimedia in HTML

In the next chapter, we will learn about **HTML Block and Inline Elements**.
