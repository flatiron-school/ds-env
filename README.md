## Environment Files: Machine Learning, Artifical Intelligence, & Large Language Models

* `ml` subfolder for the courses **Introduction to Machine Learning** _and_ **Machine Learning with Scikit-Learn**
* `ai` subfolder for the courses **MLP, Time Series, & Neural Networks** _and_ **Neural Networks & Similar Models**
* `llm` subfolder for the courses **Large Language Models**

### Conda Environment

A **conda environment** is like a separate workspace on your computer where you can keep all the tools, libraries, and settings you need for a specific project — especially different versions of Python and Python packages.

For example, one of your projects might need `Python 3.10` with `TensorFlow 2.12`, while another project might require `Python 3.8` with `PyTorch`. Normally, it’s very hard (or even impossible) to have different versions of Python and their packages installed side by side without causing conflicts.

A conda environment solves this problem by creating an isolated space just for that project. You can "enter" that environment, work with exactly the Python version and packages you specified, and then "exit" without affecting anything else on your computer.

In other words, it’s like having separate mini-Python setups, each designed exactly for the needs of a particular project.

### YAML files

A YAML file (stands for _YAML Ain’t Markup Language_) is a human-readable text file used to store data in a structured way. It uses indentation to show hierarchy (like nested lists or dictionaries), making it easy to read and edit. They are denoted by `.yml` and we use them to create conda environments.

Using YAML files are ideal for data science and artificial intelligence for the following reasons:

* **Reproducibility**
   * YAML files can capture exactly which packages and versions are needed for an environment
   * This means you (or collaborators) can recreate the same environment anywhere, avoiding "it works on my machine" issues
* **Portability**
   * You can share your consda environment by simply sharing one .yaml file
* **Clarity**
   * The file is easy to read and modify — you can clearly see dependencies, Python version, and channels 

### Conda Environment Creation from a YAML file

Depending on the machine that you are working on, run this code:

`conda env create -f [NAME].yml`

in your terminal/prompt after activating `conda`.

*  `Conda` [documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) can be found here
    * Scoll down to "Creating an environment from an environment.yml file"
*  When running the above environment creation code, make sure you are in the same location as the downloaded YAML file

*Make sure to replace `[NAME]` with the appropriate file depending on whether you have a PC (Windows), Mac with M silicon chip, or Mac with Intel chip*.

### Words of caution

Due to the dynamic nature of updates to not only PCs and Macs but also to `conda` and the packages/libraries themselves, the .yml files will inevitably need to be updated, or in the case of Mac with Intel no longer updated since it is in the process of being deprecated.
