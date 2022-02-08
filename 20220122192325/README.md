# Type of python packages inside PyPI

-   source tree, contains all project files available on the developers' 
    machine/repository
-   wheel, generated directory structure and metadata compressed into single
    file that is to be deployed on pypi. User of the package's machine only need
    to extract the folders inside \<interpreter-folder-path\>/site-packages.
    Example Format: pugs-0.0.1.tar.gz.
-   sdist, archive containing package source, metadata and build scripts
    required to generate the installable directory structure. A lot more work to
    do for end user's interpreters: 
    -   extract the archive,
    -   run builder,
    -   copy directory structure.
    Example Format: pugs-0.0.1-py2.py3-none-any.whl

## Pros and cons

Source tree packages depends higly on what one knows about the installation
pipeline and what the dependency of the package are: if the package contains
some external C/C++ references, users are obliged to provide references to
those. See also [git protocol for
pip](https://duckduckgo.com/?t=ffab&q=git+protocol+for+pip&ia=web)

For sdist packages, the developer might provide build scripts used to detect
missing *stuff* on the user machine, still much pain for pure python packages,
namely python packages that depends only on python code and python packages.

Wheel packages are super dooper good for pure python packages, since they
depends only on python and other python packages, so no need for them to know
C/C++ related stuff, such as compilers include directory and so forth.

## PEP to read

-   [517](https://www.python.org/dev/peps/pep-0517/)
-   [518](https://www.python.org/dev/peps/pep-0518/)
