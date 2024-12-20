---
# Copyright 2024 Accellera. All rights reserved.
style: annex
---

# Annex B **(informative)** Electric Book commands

## B.1 Usage

```
npm run electric-book -- <command> [options]
 or
npm run eb -- <command> [options]

commands:
  npm run eb -- help     Show available commands and options
  npm run eb -- output   Generate a project or publication

options:
  -h, --help                Show available commands and options
  -f, --format              Format to output. Supported choices:
                              app, epub, print-pdf, screen-pdf, web (default)
  -b, --book                Relevant book or assets directory (default: book)
  -n, --name                Name of a new book  (default: new)
  -l, --language            Translation language (default: None)
  -c, --configs             Custom files in /_configs, comma-separated (default: None)
  -m, --mathjax             Enable MathJax (default: false)
  -u, --baseurl             A custom base URL, e.g. /books (default: None)
  -i, --incremental         Enable Jekyll's incremental build (default: false)
  -e, --epubcheck           Local path to folder containing epubcheck.jar (UNIX only)
                              (default: /usr/local/bin/epubcheck-4.2.6)
  -o, --app-os              Target app operating system. Supported choices:
                              android (default), ios, windows
  -d, --app-build           Create app with Cordova after building HTML (default: false)
  -r, --app-release         Make the app a signed release (default: false)
  -p, --app-emulate         Launch app in default emulator (default: false)
  -x, --export-format       File format to export to (default: MS Word)
  -s, --section-numbering   Depth of section (re)numbering in the book (default: -1)
  -j, --merged              Whether to merge HTML files for PDF output (default: true)
  -z, --pdf-debug           Enable PDF debug (PagedJS only) (default: false)
  -g, --pdf-engine          Select PDF rendering engine (default: prince)
  -y, --pdf-line-numbering  Enable PDF line numbering (PagedJS only) (default: false)
```

## B.2 Examples

Create a PDF for the Accellera standard template (`accellera-standard-template`):

```bash
npm run electric-book -- output --format screen-pdf --book accellera-standard-template
```

Create a PDF for the Accellera Style Guide (`accellera-style-guide`):

```bash
npm run electric-book -- output --format screen-pdf --book accellera-style-guide
```

Create a PDF for the Accellera Style Guide, and enable renumbering of sections and cross-references down to the 5th level:

```bash
npm run electric-book -- output --format screen-pdf --book accellera-style-guide --section-numbering 5
```

Create a PDF for the IEEE SA Standards Style Manual (`ieee-sa-standards-style-manual`):

```bash
npm run electric-book -- output --format screen-pdf --book ieee-sa-standards-style-manual
```
