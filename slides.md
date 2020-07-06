class: center, middle

# Remark
A presentation about a presentation tool

---
class: center, middle

# How it works
---

### 1. Content, layout and styling in markdown


```markdown
    ---
    class: center, middle
    # Cover slide
    background-image: url(images/slides/background.jpg)
    background-size: contain
    ---
    # Slide with **meme**
    .width-80[
        ![](images/slides/meme.jpg)
    ]
    ---
    # This
    1. Has 
    2. A
    3. List
    4. Mindblowing stuff, eh?
    ---
```
---

### 2. Create an HTML file
```html
<!DOCTYPE html>
<html>

  <head>
    <style type="text/css">
      /* Here be styles */ 
    </style>
  </head>

  <body>
    <script src="remark.js"></script>
    <script>
       var slideshow = remark.create({
            sourceUrl: 'slides.md'
       });
    </script>
  </body>
</html>
```
---

### 3. Open your file
- directly in browser, or
- using something like `http.server`

---
class: center, middle
background-image: url(images/slides/background.jpg)
background-size: contain
# Cover slide
---
# Slide with **meme**
.width-80[
    ![](images/slides/meme.jpg)
]
---
# This

1. has
--

2. a
--

3. list
--

4. using
--

5. incremental
--

6. slides
--

7. which could get annoying if overused...

---
class: center, middle
layout: true

---

# Presentation mode (the P key)

???

# And look you can add some notes too

---

# But 2 screens?

---

# Cloning (the C key)

---
layout: true

---
## Some other nice features
- comments
- template slides
- slide properties
- inline CSS
- syntax highlighting
- slide linking

---
# But wait, there's more!

---

## Code formatting and highlighting
```ts
def add_some_numbers(a,b):
*   a, b = "wtf!", "wtf!"
    return a + b
```

---

class: nord-dark, center, middle

# Dark Mode

<small>.letter-spacing-20[Though can also do this with a browser plugin]</small>

---

## LaTex Support

$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

---
# I like because
- Simple
- Markdown
- Can host on your blog
- HTML and CSS
- It's free

---

# It works on a tablet or phone

