## About.
This repo contains the source I use to automatically generate
[my curriculum vitae](http://bamos.io/cv) as a webpage and PDF
from YAML and BibTeX input.

[generate.py][generate.py] reads from [cv.yaml][cv.yaml] and
[publications.bib][publications.bib] and outputs LaTeX and Markdown
by using Jinja templates.
Statistics about my blog and github account are obtained
using [blog-info.py][blog-info.py] and [github-info.py][github-info.py].

## How to run.
The dependencies are included in `requirements.txt` and can be installed
using `pip` with `pip3 install -r requirements.txt`.
On Mac or Linux, `make` will call [generate.py][generate.py] and build
the LaTeX documents with `pdflatex` and `biber`.

The Makefile will also:

1. Stage to my website with `make stage`,
2. Start a local jekyll server of my website with updated
  documents with `make jekyll`, and
3. Push updated documents to my website with `make push`.

[generate.py]: https://github.com/bamos/cv/blob/master/generate.py
[publications.bib]: https://github.com/bamos/cv/blob/master/publications.bib
[cv.yaml]: https://github.com/bamos/cv/blob/master/cv.yaml
[blog-info.py]: https://github.com/bamos/cv/blob/master/blog-info.py
[github-info.py]: https://github.com/bamos/cv/blob/master/github-info.py
[Requirements.txt]: https://github.com/bamos/cv/blob/master/Requirements.txt
