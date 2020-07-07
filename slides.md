class: demo, center, middle


# Remark
A presentation about a presentation tool

???

A few weeks ago, discussion about presentation 
- Googled, found a tool
- Rens contacted me asking if I'd used the tool - which I hadn't
An interesting way to make a slide deck using Remark

---

### 1. Content, layout and styling in markdown


```markdown
    ---
    class: center, middle

    # .white[Cover slide]
    background-image: url(images/slides/background.jpg)
    background-size: contain

    ---
    
    # **meme**
    ![](images/slides/meme.jpg)
    
    ---

    # This
    1. Has 
    2. A
    3. List
    4. Mindblowing stuff, eh?

    ---
```
???

Setup is effectively a 2 step process:
- Firstly, create a markdown file using triple dashes to indicate page separators
- Simple layout can be defined using a class key-value pair
- CSS styling can be linked by wrapping in square brackets and referencing the CSS class
- Everything else can just follow markdown

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

???

Secondly define your layout in an HTML file
- You can link in any styles to configure the look and feel
- Link in the remark.js library to provide the mapping of the markdown (and quite a few extras)
- The markdown can added directly into the HTML or linked

---

### 3. Open your file
- directly in browser, or
- or use a static server like `http.server`

---
class: center, middle
background-image: url(images/slides/background.jpg)
background-size: contain

# .white[Cover slide]

---

# Slide with **meme**
![](images/slides/meme.jpg)

---

# This

1. .red[has]
--

2. .orange[a]
--

3. .yellow[list]
--

4. .green[using]
--

5. .blue[incremental]
--

6. .indigo[slides]
--

7. which could get annoying if overused...

---
class: center, middle
layout: true

---

# Keyboard shortcuts FTW!

???

# Here be some notes
- P = presentation
- C = bring on the clones
- F = Full screen

> "A quote to inspire generations will not be said at this point in time"

---
layout: true

---
## Additionally
- template slides
- slide referencing
- events
- timers
- comments

<div class="my-footer"><img src="images/slides/gdd.png" /><-- Behold, a footer</div>

---

## Code formatting and highlighting
```python
class MockRequest(object):
    def __init__(self, request):
        self._r = request
        self._new_headers = {}
        self.type = urlparse(self._r.url).scheme
    
    def get_full_url(self):
        # Only return the response's URL if the user hadn't set the Host
        # header
        if not self._r.headers.get('Host'):
            return self._r.url
        # If they did set it, retrieve it and reconstruct the expected domain
*       host = to_native_string(self._r.headers['Host'], encoding='utf-8')
        parsed = urlparse(self._r.url)
        # Reconstruct the URL as we expect it
        return urlunparse([
            parsed.scheme, host, parsed.path, parsed.params, parsed.query,
            parsed.fragment
        ])
```

---

class: nord-dark, center, middle

# Dark Mode

<small>For those serious moments</small>

---

## Table styling

.bla[
| Name | Price | Number |
| ---- | ---- | ----: |
| Banana | €1  | 5    |
| Apple | €1  | 6    |
| .red[Strawberry] | €1  | 7    |
]

---

## Columns

.left-column[
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
]

.right-column[
Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
]

???

Things like columns and picture layouts require a bit more work though there are some good samples available

---

## GIFs

<iframe src="https://giphy.com/embed/94iS62lx8CRQA" width="700" height="471" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>

---
.left-column[# Pros
- Free
- Simple
- Markdown
- Can host anywhere
- HTML and CSS]
.right-column[# Cons
- extremely sensitive to scrolling
- no drag-n-drop
- layout requires effort
- it may lead to fiddling until midnight on a 5 minute presentation
]


---

# And a last nifty feature...

