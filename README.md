# image registration and combination notebooks

This is a "beta" of the machinery that will eventually be used to store STScI notebooks.

## Adding a notebook

To add a notebook, create a directory for the notebook *inside* "imregcomb". Inside that directory, place your notebook, and a "requirements" file.  In the requirements file you should put everything your notebook requires to work *including a version number*.  Include there a "known good" version number - e.g., "numpy==1.14" if you've tested on numpy 1.14.

Once you've done this, ``git add`` and ``git commit``.  *NEVER COMMIT A NOTEBOOK WITH OUTPUTS*.  That is, always clear the outputs before committing.

## Test-running notebooks

To execute your notebook and see it rendered as a web page, go to the root of this repo (where the README is) and do ``python convert.py``.  Then open up the generated index.html and follow it to your notebook.