# Documentation for G2U project

TODO: Include diagrams, figures, charts, and other necessary details (Swagger), other than TeX report

## Setup (Linux)

Here's the basic guide for installation and setup on Ubuntu/Debian.

```sh
sudo apt install texstudio # install the editor
find /usr/share/texlive -name stmaryrd.sty # random diagnostics

# libraries to get the most of the things done
sudo apt install texlive-latex-extra
sudo apt install texlive-fonts-extra
sudo apt install texlive-math-extra
sudo apt install texlive-science

# pip and pygments
sudo apt install python3-pip # if your system does not have pip
pip install pygments
```

Build flags to be configured on settings:
```sh
pdflatex -synctex=1 --shell-escape -interaction=nonstopmode %.tex # build setup
xdg-open %.pdf > /dev/null # to view the output PDF
```

Other notable IDE (TeXStudio) setup:
```yaml
Style: default
Color Scheme: classic
Font: DejaVu Sans
Font Size: 11
Default Compiler: PDFLaTeX
PDF Viewer: Internal PDF Viewer (Embedded)
Default bibliography tool: BibTeX
```

## Setup (Overleaf)

There's nothhing much to do in terms of setup for overleaf. Just using PDFLaTeX would be fine in most of the cases.
