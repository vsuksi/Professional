# Questions and clarifications

**This is a repository for critical information regarding the project at hand. Formulating it into a question allows for a specific viewpoint to be addressed or an implication to be hinted at, for example**


**Must your libraries be in the same folder?**
Libraries must be in the same directory or subdirectory when importing directly, for a library in another directory use sys.path or even better, install it in a local virtual environment. The latter has the advantage of reproducibility, since no local path is specified.

**How does a GitHub repository and project differ**
A git repository is where all collaboration takes place but project management is done in a Github Project within the repository.

**What is linting and why is it done?**
Linting is checking the code for subtle programming errors and stylistic considerations.

**How does pip install differ from conda?**
A pip install installs from a different repository, PyPi.

**How does a script and source code differ?**
Source code can be thought of as the pipeline whilst scripts are run as a one-off or interactively.

**How to open file from command window?**
cd followed by the complete path.

**Is it possible to jump directory in windows command window?**
Based on some experimentation and Google searches I'd say it is not possible.

**How does calcom.py and calcom.io differ?**
The .io file extension stands for Input/Output, so calcom.io is used to perform input/output operations

**What is YAML?**
YAML is a data serialization language for all programming languages, that is a program that converts an object into a stream of bytes

**Is it possible to load inline kernel results in GitHub?**
No, since you aren't running code in GitHub, has no kernel.
