# Introduction

Author: [dreampuf](https://github.com/dreampuf/)

[GraphvizOnline](https://github.com/dreampuf/GraphvizOnline) could let you debug the graphviz languages online. [DEMO](https://raw.githack.com/denim2x/GraphvizOnline/devel/index.html)

# Usage

The URL has the following format:
`<protocol>://<host>#<hash>`, where `hash` may be one of:
- actual Graphviz [code](https://graphs.grevian.org/reference) (_optionally_ URL-encoded)
- a [Gist](https://docs.github.com/en/github/writing-on-github/creating-gists) ID, _optionally_ followed by a _filename_ (e.g. `#aa5a315d61ae9438b18d/file.gv`)
- a [Gist](https://docs.github.com/en/github/writing-on-github/creating-gists) ID, _optionally_ follwed by a _hash reference_ (e.g. `#aa5a315d61ae9438b18d#file-file-gv`) - like the URL of a public Gist

In case the _filename_ is missing, a _dialog_ is shown with a listing of all files within the Gist; any file selected henceforth is subsequently loaded and rendered.

# Implementation

- [viz.js](https://github.com/mdaines/viz.js) This repo has compile graphviz(C) to javascript via [emscripten](https://github.com/kripken/emscripten).
- [ACE-editor](http://ace.ajax.org/) An amazing online editor.

# License

GraphvizOnline licensed under BSD-3 license. The dependencies:

- [viz.js](https://github.com/mdaines/viz.js/blob/master/LICENSE) MIT
- [ACE-editor](https://github.com/ajaxorg/ace/blob/master/LICENSE) BSD-2
