# Questions and clarifications

**This is a repository for critical information regarding the project at hand. Formulating it into a question allows for a specific viewpoint to be addressed or an implication to be hinted at, for example**

**Is it possible install packages in an R instant installed via conda, and can this be of use?**
It is. When I was trying to get R working in a conda environment, I needed a package which only succeeded through the R installation itself. Conda probably doesn't notice this so problems may pop up in resolving environments. Thus, such installation are probably best done last, when you know that everything else is working.

**How is conda "forge" installation different from default?**

**How does seed work in code for reproducibility?**


**What is a confusion matrix and how does it relate to AUROC?**
A confusion matrix is a table with the the predicted classes on one axis and the actual classes on the other. In binary classification, this results in a handy matrix of true negative, false negative, false positive and true positive cases.
The true positive rate (TPR, true positives / true positives + false negatives) then describes the proportion of data points that are correctly classified as positive with regards to all positive cases. Conversely, the false positive rate (NPR,false positives / false positives + true negatives) describes the proportion of negative data points that are incorrectly considered positive.

Using a series of probability thresholds, the TPR is plotted against the FPR. Thus, this ROC (receiver operating characteristic curve) visually represents the false positive rate to false negative rate ratio at different probability thresholds.

There are many possible interpretations of the AUC. My preferred way to look at it is as a summary of if the overall accuracy of the test across probability thresholds.


**What is S3 in R?**
It is the first and simplest object-oriented system in R.

**Is AUC and AUROC the same thing?**
They are very commonly used interchangeably, although this

**Is ordinary least squares (OLS) and linear regression the same thing?**
No, but this is a key question illustrates a critical difference which is best kept in mind throughout data science. OLS is a technique to fit a straight line to data, while linear regression is the general case of fitting a straight line to data.

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
