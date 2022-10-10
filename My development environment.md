### My development environment
The intent with the repository is to store bits of code and useful information relating to my development environment for data science. Moreover, in this document, I will explain how it all works along with common pitfalls.

If you're working and feeling overwhelmed, close all the tabs in Atom and open a single to-do list.

To create a new repository in Atom, first drag the folder created in the File Explorer window into a completely empty Atom instance. Then create a file within the folder and do a detached commit. The GitHub tab should now display a "Publish on GitHub", congratulations!

Remember that you can have two files open simultaneously in Atom.

State the intent of the file (if applicable) at the beginning, this helps with clarity.

If GitHub sync starts throwing random errors, the easiest way to fix it is to remove the repositories from GitHub and initialize them again.

Save your personal Atom sessions last thing every night, this could work as a ritual to stop working for the day!

Print to pdf saves a pdf picture of the file/webpage while save as pdf produces a searchable pdf document and includes links and other fun stuff.

Atom use guidelines
Write classifiers with capital letters
Use "-" with intent, otherwise everything will simply be pushed off to the side
skriv en egen syntax cheatsheet för pandoc markdown
only write documments for others in word or powerpoint, everything else in markdown
make .qmd only files which you want to present to other people
Notation of forking in scripts? First numbers (1) then if the next step includes alternatives, do 2a and 2b and 2c and so forth. If there are several of the same, 2b for example, it means that they are optional.

#Email

Remember to not answer emails too quickly; information exchange between two parties will be more efficient and use up less brain capacity if more material is communicated at a time, so let the material build up a bit.

quarto render hello.qmd --to html
open file (html) in app

When committing to an ordinary file, just put in the date.

When you've completed a project, move it into the professional archives and remove the git file to remove the commit history.

Write your commits in an imperial mood, as git works in the same way. For example: Debug the data cleaning, clean your room

##Setup
Atom is the bedrock of my development environment. In Atom, I manage my all of my material which is organized in GitHub repositories. Synchronization with GitHub reduces the amount of switching back and forth between windows. Since it is also possible to run scripts in Atom, even using Conda virtual environments, most of my coding will happen in Atom. Coding is facilitated by the easy installation of various plug-ins in Atom. I also prefer the look and feel of the website, in comparison to
On occasion I might make GitBooks,

Have current projects as independent repositories, which will be added to the archive of professional when they are completely done. This allows you to use the Git functionalities like branching to maximum effect including collaboration while still keeping all your stuff in a single cloud system.

Common, stupid problems in your workflow:
The debug you made isn't working because you didn't save the file!
One can't fetch a new repository directly from GitHub to Atom. To start working on a new repository in GitHub, the new repository is cloned using the GitHub tab in Atom.

A small blue dot is shown in the Atom tab if it has not been saved.

Github workflow:
In trunk-based development, everyone has access to the main branch of the project, from which they branch out making only a small number of commits in the develop branch before merging to the main branch. Any problems that arise in merging back to the main branch can easily be tracked to one of the few commits in the develop branch.

In Gitflow, on the other hand, a whole feature may be constructed in a development branch before merging back to the main branch. This increases the risk of problems when merging to the main branch and the causes of problems can be harder to identify.

When a project works as intended but is being developed further, release branches are used to export the project.

Fork is used when a project is split and not intended to be merged in the near future.

If running code is slow, use Advanced Systemcare to perk up your computer, put on boost mode and and eliminate all applications you don't need.

_List here the packages and instructions for someone to do this themselves.
How to install and use GitHub in Atom
How to install script in Atom
How to conda environment in Atom

Perhaps I could write this in a way that encourages non-duality or at least discourages the self? Howbowdah?
Remember, this document was planned to be written in Atom!
