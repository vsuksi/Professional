# My development environment

**This document covers the functioning of my development environment. More general computer-nerd content does not belong here.**

## Setup
Atom is the bedrock of my development environment. In Atom, I manage my all of my material which is organized in GitHub repositories. Since it is also possible to run scripts in Atom, even using Conda virtual environments, most of my coding will happen in Atom. Coding is facilitated by the easy installation of various plug-ins in Atom. Writing in markdown allows for easy generation of various types of documents via Quarto, and the limited amount of formatting encourages focus on the writing.


## Quarto
It is not possible to specify different virtual environments for code in the same Quarto (.qmd) file. However, you can render documents in a Quarto project using different virtual environments, and include code from documents run in said virtual environments by using "{{< include _content.qmd >}}" in your master document. Then render the whole project using "freeze: true". Using "freeze:auto", if a change is made, the whole project is rendered.

## Conda
In the beginning of a new project, create environments tree-trunk style. For example, for binary classification of Lyme's disease, I created a main environment, "lyme_main". When installing local packages, installing packages using R or using Pip install, create a clone of the main environment. These branched environments are best named according to the application; "lyme_main_CoDaCoRe" was fitting when most of the project was done using R except for a SSVM-model for which a classifier was only available in Python. If the branched environments happen to work for all your scripts, then all the better as all scripts can be included in a single Quarto document.

Remember to save your environment in a folder ("Environments") in the project at hand for the sake of reproducibility.

## From repositories to folders to files
Each new project gets its own repository. Files useful across all repositories include "Braindump", "To-do", "People" and Questions and Clarifications". A brief intent-setter is found at the beginning of each file.

In each project repository, create directories that organize the material that your project draws on; "PDF", "Code" and "Data", for example. For output, create a directory and organize files in their own directories therein. A directory for a script is best named the same as the script. Keeping the presentation or document that you're working on in the main output directory allows for easy referral of code and files from other folders in the output directory.

Name files using underscores between words, avoiding special characters and capital letters. Scripts are best named in an imperial mood, "test_features.py", for example. When developing a script, you'll probably be working line-by-line in the terminal. Tidy up scripts by using descriptive, whole-sentence comments and write results to the same file each time. After each run, transfer the results to a dedicated result file, where each run is detailed under the date of the run.

Deleting unimportant files readily and without much hesitation will make for better organization. If you still need a file, you can retrieve it from the recycling bin. When a project is completed or set aside, move it to the "Archives" folder in the "Professional" repository.


## Github
Github workflow:
In trunk-based development, everyone has access to the main branch of the project, from which they branch out making only a small number of commits in the develop branch before merging to the main branch. Any problems that arise in merging back to the main branch can easily be tracked to one of the few commits in the develop branch.

In Gitflow, on the other hand, a whole feature may be constructed in a development branch before merging back to the main branch. This increases the risk of problems when merging to the main branch and the causes of problems can be harder to identify.

When a project works as intended but is being developed further, release branches are used to export the project.

Fork is used when a project is split and not intended to be merged in  the near future.

If running code is slow, use Advanced Systemcare to perk up your computer, put on boost mode and and eliminate all applications you don't need.

_List here the packages and instructions for someone to do this themselves.
How to install and use GitHub in Atom
How to install script in Atom
How to conda environment in Atom

Perhaps I could write this in a way that encourages non-duality or at least discourages the self? Howbowdah?
Remember, this document was planned to be written in Atom!

## From folders to files

The file name in tree-view and Git becomes orange when a file has been modified and saved. Separate each word in file names with "_".
The intent with the repository is to store bits of code and useful information relating to my development environment for data science. Moreover, in this document, I will explain how it all works along with common pitfalls.

If you're working and feeling overwhelmed, close all the tabs in Atom and open a single to-do list.

To create a new repository in Atom, first drag the folder created in the File Explorer window into a completely empty Atom instance. Then create a file within the folder and do a detached commit. The GitHub tab should now display a "Publish on GitHub", congratulations!

Remember that you can have two files open simultaneously in Atom.

State the intent of the file (if applicable) at the beginning, this helps with clarity.

If GitHub sync starts throwing random errors, the easiest way to fix it is to remove the repositories from GitHub and initialize them again.

Save your personal Atom sessions last thing every night, this could work as a ritual to stop working for the day!

Print to pdf saves a pdf picture of the file/webpage while save as pdf produces a searchable pdf document and includes links and other fun stuff.

Atom use guidelines
make .qmd only files which you want to present to other people
Notation of forking in scripts? First numbers (1) then if the next step includes alternatives, do 2a and 2b and 2c and so forth. If there are several of the same, 2b for example, it means that they are optional.

To add picture from same directory:
![alt text](image.png)

To add picture from subdirectory:
![image info](./subdirectory/image.png)

#Email

Remember to not answer emails too quickly; information exchange between two parties will be more efficient and use up less brain capacity if more material is communicated at a time, so let the material build up a bit.

Make powerpoints with the same onedark theme and font as Atom

quarto preview document.qmd

quarto render hello.qmd --to html
open file (html) in app

When committing to an ordinary file, just put in the date.

When you've completed a project, move it into the professional archives and remove the git file to remove the commit history.

Write your commits in an imperial mood, as git works in the same way. For example: Debug the data cleaning, clean your room. More generally, having a standard mood for text or file names makes for less ambiguity.

Github workflow:
In trunk-based development, everyone has access to the main branch of the project, from which they branch out making only a small number of commits in the develop branch before merging to the main branch. Any problems that arise in merging back to the main branch can easily be tracked to one of the few commits in the develop branch.

In Gitflow, on the other hand, a whole feature may be constructed in a development branch before merging back to the main branch. This increases the risk of problems when merging to the main branch and the causes of problems can be harder to identify.

When a project works as intended but is being developed further, release branches are used to export the project.

When using the "include" functionality, a single change in the document will cause the document to rerender the "included" Quarto documents as well.

Fork is used when a project is split and not intended to be merged in the near future.

If running code is slow, use Advanced Systemcare to perk up your computer, put on boost mode and and eliminate all applications you don't need.

_List here the packages and instructions for someone to do this themselves.
How to install and use GitHub in Atom
How to install script in Atom
How to conda environment in Atom

Metadata of individual Quarto documents overrides global project metadata!

In Quarto code block execution options, use "warning: false" and "error: false" to exclude annoying errors, for example I was able to exclude "Loaded Tensorflow Version blaa.blaa"

You will need r-markdown, installed through R itself, in an environment if you want to render a Quarto document.

The ideal is that writing code would be as fluent as using a point and click user interface for your statistics and machine learning. For example, think of a function as a a single button in a user interface, although you have the ability to modify the button's behavior when working in code. But still, it is a single button, which is a good perspective for not getting bogged down in the nitty gritty of coding.

Focus more on defining/formulating the problem that you will be solving, so each problem becomes more like a Rosalind-style problem.

Ctrl-K *direction arrow* opens a pane in the wanted direction!
Ctrl-W closes panes. This is good to use, since I might have been opening several panes on top of each other, which probably slows down Atom!

Files with spurious names are a sign that they are temporary and can be deleted without hesitation

What to use for data storage? SQL?

You can create a subdirectory named /.env containing your environment file for conda to activate.  https://carpentries-incubator.github.io/introduction-to-conda-for-data-scientists/02-working-with-environments/index.html

%>% can be read as "and then"

To install a local python package: include the calcom directory in the same directory as the environment folder and create a virtual environment from the .yml environment file. Or navigate to the file and do pip install -e calcom.

You can also make webpages with Quarto!

Remember, even when using warnings:false and errors:false in the execution options of a code chunk, you can view errors and warnings in the terminal during render.

In Quarto, Use eval:false to include code blocks without executing them; write the result instead. Where is this applicable in the project at hand? Or can you simply run it once you are completely certain of it working?

There are web services for converting a .yml file to a .txt file if needed.

Beware when installing R through conda; vanilla installs an old version; use conda forge instead.

When making contributions to longer snippets of code, it might be worth using commit in the way that it is intended to be used: comment what has been done and why.

Your desktop is your repository for temporary files, to be dumped directly after use.
