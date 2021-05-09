# Remarkjs

A little demo I made to show what's possible with [remark](https://github.com/gnab/remark), 
a tool for rendering markdown as an HTML slideshow.

To run you'll need a light http server, Python's [http.server](https://docs.python.org/3/library/http.server.html)
works well.  To run:
```
python -m http.server
```

Some keyboard shortcuts:
- P - Presenter mode
- C - Clone for multiple screen
- h - help


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
can be done using Google Chrome's print
but there may be some issue with styling.