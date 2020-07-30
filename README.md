# Latex Literature Review Template
Literature review template in latex. This template is from my qualification exam proposal I wrote for my dissertation while a graduate student at UC Davis. I has been cut down in a few places, and some what extensively commented

## Files structure

```
- main.tex
- custom_lit_style.sty
- pages/
	- intro.tex
	- img_test.tex
	- ref_test.tex
	- table_test.tex
	- eqn_test.tex
- img/
	- test01.png
	- test02.jpg
	- test03.tiff
	- test04.eps
	- page.pdf
```

The file structure is fairly straight forward. The `main.tex` file should be compiled in the root of this project. 

- Here you include the pieces of your project using the `standalone` package that are in the `pages/` subdirectory. This template comes with files that test most of the functionality that I've incorporated.
- Images should all exist the subdirectory `img` and they are imported with the `graphicx` package.
- You bibliography file should be a `.bib` file. I use `bibdesk` to manage my library, and any formated `.bib` should work. I provide one here called `sample.bib` since I've exported it from `bibdesk`.

## Formatting options

Some of the custom formatting options are done via excellent customizable packages, while others are completely from Stack Overflow. Most of these are documented in the `custom_lit_style.sty` 

### Sections

In this section, we will go over some of the use cases for the `titlesec` and `titletoc` pieces that I've utilized to customize the section headings and make the table of contents.

### Images

Images are handled using the `graphicx` package., but there are additional packages that I use to modify image captions: `subcaptions` and `captions`.

For some modifications, see the style file  `custom-lit-style.sty` under the heading `% Setting custom figures and table captions etc.` 

Mainly, caption setup for the `figure` and `subfigure` environments are defined.

### Tables

Tables are created from the following website: [https://www.tablesgenerator.com/](https://www.tablesgenerator.com/) because it was easier than making my own. However, it can be buggy at times. Use at your own discretion. Working on `jinja2` python integrations for templating. Will report back at some future time

Captions are also handled with the same `caption` setup as above for images. Under the same header, you can see the table caption set up.

### Equations

Equations are not too complex, just using the `equation` environment. Nothing fancy here.

### Bibliography

This is probably the hardest of them all, but I've come accustomed to using `natbib` for the bibliography. 

## References

Here I will add the links where I found most of the info, but there are many. Will document them as they become available.