# Scope

[Awesome CV](https://github.com/posquit0/Awesome-CV) is LaTeX template for CVs inspired by Fancy CV and it is one of the templates available in [vitae](https://github.com/mitchelloharawild/vitae) (`vitae::awesomecv`). The vitae package makes creating and maintaining a Résumé or CV with R Markdown simple. It provides a collection of LaTeX and HTML templates, with helpful functions to add content to the documents.

The codes in this repository recreate headers and styles from Awesome CV while allowing more direct control on the .tex code that runs underneath. 

This is achieved by directing the output of your rmarkdown file to `awesome.tex` which controls format and styles:

```
output:
  pdf_document:
    latex_engine: xelatex
    template: "awesome.tex"
```

`awesome.tex` is a simplified version of `awesome-cv.cls`, with a few minor adds (for example hypersetup, tolerance, emergencystretch, etc).  


It requires `tinytex`:

```
install.packages("tinytex")
tinytex::install_tinytex()
```



# Preview

[![](./img/preview.png)](https://github.com/mlombardi6/awesome-template/blob/main/awesome-template.pdf)



