## Building the Project

To compile the dissertation PDF:

1. Ensure you have a LaTeX distribution installed (e.g., TeX Live, MiKTeX).
2. Install `latexmk` and `biber` (for bibliography).
3. Open the project folder in VS Code with the LaTeX Workshop extension installed.
4. Compile using the build command (usually `Ctrl+Alt+B` or auto-build on save).
5. The output PDF and auxiliary files will be generated in the `build/` directory.

Alternatively, from the terminal:

```bash
latexmk -pdf -outdir=build main.tex
biber build/main
latexmk -pdf -outdir=build main.tex
