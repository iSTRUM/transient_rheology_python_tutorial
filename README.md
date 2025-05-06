## Python tutorials & intro to transient rheology

This is a draft of a jupyter-book introducing some python packages in the context of transient rheology, part of the iSTRUM broader impacts efforts. 

## requirements

```
pip install -r tutorial_content/requirements.txt
```

## building the book 

```
jupyter-book build tutorial_content
```

note: if you've previously built and have since updated chapters, you may need to clear out the old builds first.

check the rendered versions in `tutorial_content/_build/` and open `tutorial_content/_build/html/index.html` in a browser 

## hosting the book 

when ready, copy over the html folder at `tutorial_content/_build/html` to the main istrum repo. 



