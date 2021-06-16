# Resume

If I gave you my resume, this is what makes it! It's a latex document I modified to my liking, and when I tag a commit it triggers a workflow that compiles the .tex file into a .pdf, uploads it as an artifact and attaches it as a release.

 See releases to download the final product, or clone and compile using latex:

```bash
# compile? with pdflatex and view with mupdf
pdflatex resume.tex
mupdf resume.pdf  
```

```bash
# get latex
pacman -S texlive-most
````

template from:
https://github.com/jankapunkt/latexcv/tree/master/sidebarleft
