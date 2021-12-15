PanLeaf - Write Pandoc Markdown and Produce LaTeX PDF in OverLeaf
===

PanLeaf is an extension of [overleaf](https://github.com/overleaf/overleaf) to compile markdown files to pdf using [pandoc](https://github.com/jgm/pandoc).

### Motivation

Markdown is more light-weight and pleasant to write for casual projects, e.g. homework and everyday slides.
Editing it collaboratively online using overleaf is made possible by this project.

### Installation 

Build the docker image in `panleaf` directory to overlay panleaf over an overleaf docker image.

### Usage

When _main document_ is set to a markdown file, pandoc is automatically enabled, and output of pandoc is redirected back to the web front-end.
Create `config.yaml` as the option setting file of pandoc.
If this file exists, a command line argument `-dconfig` is added to execute pandoc.

### TODO

Jumping between source code and PDF file is not supported, yet.
