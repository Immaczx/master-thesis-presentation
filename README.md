# Master Thesis Presentation — An Embedded Deep Learning Approach for Seed Image Segmentation

**Author:** Camilo Pelaez Garcia  
**Institution:** Universidad Nacional de Colombia  
**Program:** Master in Systems and Computing Engineering  

## Overview

Beamer presentation for the master thesis defense. Built with the custom Oxygen theme and UNAL branding.

## Repository Structure

```
├── main.tex                    # Main presentation file
├── References.bib              # Bibliography
├── beamerthemeOxygen.sty       # Custom Beamer theme
├── unal_header.png             # UNAL header logo
├── EscudoUN-2016.png           # UNAL shield
├── Tesis_presentation/
│   └── Figures/               # All presentation figures
└── .github/workflows/         # CI/CD: auto-compile PDF on push
```

## Compiling Locally

Requires **TeX Live 2024+** with XeLaTeX:

```bash
# Arch Linux
sudo pacman -S texlive-basic texlive-latexextra texlive-xetex \
               texlive-fontsextra texlive-bibtexextra
```

Then compile:

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

## CI/CD

Every push to `master` or `develop` triggers a GitHub Actions workflow that compiles the PDF and uploads it as a build artifact. Pushes tagged `v*` create a GitHub Release with the PDF attached.

## License

© Camilo Pelaez Garcia — Universidad Nacional de Colombia. All rights reserved.
