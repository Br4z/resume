# Resume

Feel free to fork this repository or use it as a template for your own resume. Just edit the `main.tex` file with your information, update the `picture.jpg` and compile it with a LaTeX editor.

If you have any publications, add them to the `publications.bib` file in BibTeX format. The publications section is currently commented out in `main.tex` (`\section{Publicaciones}` and `\printbibliography` lines to include it in your resume).

## Compilation

This project uses `biblatex` for bibliography management, which requires `biber` for processing. If you do not want to modify your global latexmk configuration, create a `.latexmkrc` file in your project directory with the following settings:


```
$out_dir = "build"; # Output files to build/ directory
$pdf_mode = 1; # Generate PDF directly
$bibtex_use = 2; # Use biber instead of bibtex
```

This ensures proper compilation with LaTeX Workshop or latexmk.
