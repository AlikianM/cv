# cv

Copy of a jekyll-based markdown CV, which currently looks something like [this](https://byronmews.github.io/cv).

All credit to [blm](http://blm.io/blog/markdown-academic-cv/), and original markdown CV fork from [elipapa](https://github.com/elipapa/markdown-cv).

### How to use

To build run jekyll:

```bash
jekyll serve
```
(You may need to [install jekyll](https://jekyllrb.com/docs/installation/).)

Point browser to [127.0.0.1:4000](http://127.0.0.1:4000).

### HTML version

The HTML version is generated by Jekyll under `_site` using `media/cv-screen.css`.


### PDF version

Separate CSS for print and screen media (see `media/cv-print.css`). Print PDF properly using firefox.

Another problem with the PDF is pagebreaks, they're often not handled gracefully so I've added one in explicitly. Say you want a pagebreak before the section titled "education" (`h2` text is set to `id` so use unique section headers!), the print media CSS would be:

```CSS
#education {
	page-break-before: always;
}
```

