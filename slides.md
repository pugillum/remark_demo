class: center, middle

# Remark
An alternative to PowerPoint or Deckset

---
class: center, middle

# How it works
---

1.Define your content, layout and styling in a markdown file


```markdown
    ---
    class: center, middle
    # Cover slide
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

2.Create an HTML wrapper linking `remark.js`
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
class: center, middle
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

# Presentation mode with the touch of a button (the P key)

???

And look you can add some notes too

---

# But 2 screens?

---

# Cloning with the touch of a button (the C key)

---
layout: true

---
# Some other nice features
- comments
- template slides
- slide properties
- inline CSS
- syntax highlighting

---


