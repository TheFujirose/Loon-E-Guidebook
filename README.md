# Loon-E Guidebook

This repository contains the LaTeX source for the Loon-E ASV guidebook maintained by HumberASV. The document covers the vehicle overview, software architecture, development workflow, glossary, and supporting references for the project.

## Overview

The main entry point is [main.tex](main.tex), which assembles the document from the modular section files under [sections/](sections). Shared formatting, custom commands, and bibliography setup live in [preamble.sty](preamble.sty).

Current content includes:

* Introduction and document conventions
* Systems overview
* Software architecture and base station details
* Development setup and contribution guidance
* Glossary and bibliography

## Requirements

You need a LaTeX distribution to build the PDF. TeX Live is recommended, but any distribution with support for `biblatex` should work.

## Build

From the repository root, compile the document with your LaTeX editor or from the command line:

```bash
latexmk -pdf main.tex
```

If you build manually, run `pdflatex`, then `biber`, then `pdflatex` twice more so the bibliography and references resolve correctly.

## Repository Layout

```bash
Loon-E-Guidebook
├── citations/        # BibTeX bibliography files
├── code/             # Code snippets and examples
├── images/           # Figures used in the guidebook
├── sections/         # Modular LaTeX content
├── main.tex          # Document entry point
└── preamble.sty      # Shared packages and custom commands
```

## Editing Content

* Update section text in the relevant file under [sections/](sections).
* Add or adjust references in [citations/](citations).
* Place new figures in [images/](images) and reference them from the section files.
* Rebuild the document after making changes to confirm the PDF renders as expected.