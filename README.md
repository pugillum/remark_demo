# Remarkjs

A little demo I made to show what's possible with [remark](https://github.com/gnab/remark),
a tool for rendering markdown as an HTML slideshow.

To run you'll need a light http server, Python's [http.server](https://docs.python.org/3/library/http.server.html)
works well. To run:

```
python -m http.server
```

Some keyboard shortcuts:

- P - Presenter mode
- C - Clone for multiple screen
- h - help
- f - fullscreen

## What I like

- it's free
- it's configurable, plus good to play around with HTML and CSS now and then
- can be hosted on your website
- instant dark mode with Dark Reader (a chrome plugin)

## Styling

The default screen ratio can be changed to 16:9 (see the `index.html` file)

## Extra Features

- Hugo - [integrate with Hugo](https://github.com/gnab/remark/wiki/Using-with-Hugo)

## PDF printing

As mentioned in the [documentation](https://github.com/gnab/remark), printing to PDF
can be done using Google Chrome's print but will not have a great layout. To correct
this, add the following to the CSS:

```
@page {
  size: 1210px 681px;
  margin: 0;
}

@media print {
  .remark-slide-scaler {
    width: 100% !important;
    height: 100% !important;
    transform: scale(1) !important;
    top: 0 !important;
    left: 0 !important;
  }
}
```

## CSS

Note that the CSS I've included here is a real mish-mash of me trying things out!
