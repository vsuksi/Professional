Feature selection methods:
Filter methods are independent of any machine learning algorithms, and are selected based on statistical tests for their correlation with the outcome

Wrapper methods use a subset of features to make a model, and go through various combinations of features as subsets to choose the optimal features. This is quite computationally expensive.

Embedded methods combine filter and wrapper methods, resulting in feature selection influenced by statistical methods and trying out different subsets of features.

Embedded feature selection: feature selection is integrated into the training phase so that the best features are generated.

When learning this stuff, remember that people are very confident in THEIR usage of terminology

To install a python package locally, navigate to the folder and do pip install -e.

It does not matter whether you save a conda environment as a .yml, .yaml or .txt; it will be exactly the same

Please stand while working, it will lessen pain, frustration and fatigue resulting in a better day. Moreover, typing feels more effortless when standing up.

Computational markdown simply means a markdown document with a kernel.

A nice thing about markdown is that you can avoid formatting to a larger extent. For example, when uploading a word file to a cloud service, it may be shown differently, which is annoying. Better not format at all before

The Quarto preview is updated as you change the code!

Running conda after pip has the potential to overwrite and potentially break packages installed via pip. Similarly, pip may upgrade or remove a package that conda has installed. This is because conda and pip do not know about each other's codependecies.
If a package isn't available in a conda repository, conda build can be used to create a package for said software.
Pip can also be used with the argument "--upgrade-strategy only-if-needed" to avoid conda packages from being upgraded unnecessarily.
In summary, install conda packages first, and then complement with pip using the "--upgrade-strategy onle-if-needed" argument.
the argument "conda list -e > requirements.txt" can be used to save environment to a text file for easy reproducibility.
Package requirements can be passed to conda via the --file argument from a text file.

IPython is an interactive command shell for Python. To run R interactively, type R in the command window.

Remember to use the "Publish on Github" -functionality when creating a new repository.

You can delete files in the "Downloads" folder; if a file is important, you will have organized it somewhere else!

A shell script is a computer program designed to run on the Unix-shell, which is a command line interpreter for Unix-like operating systems, including Linux.

.md is the markdown file extension

.qmd is the R markdown/Quarto extension

When using "from ses import sus", one can use sus directly instead of ses.sus

wb opens a file in Python in binary format for writing

# Data science tool updates
Jupyter Notebook is being replaced by JupyterLab
Atom will be discontinued in december 2022

# Learning resources

Learn R using "Telling stories with data", https://tellingstorieswithdata.com/

# File extensions
.md is the markdown file extension
.qmd is the R markdown/Quarto extension
