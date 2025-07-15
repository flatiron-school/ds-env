## Pytorch and Transformers Environment Set-Up

For this course, the version of `PyTorch` is 2.6.0 and `transformers` should be 4.49.0 or higher. In particular, we have successfully tested both 4.49.0 and 4.52.2 of `transformers`.

You can verify the versions, respectively, by running the following in your notebook after installing the necessary libraries:

`import torch` <br>
`torch.__version__`

and 

`import transformers` <br>
`transformers.__version__`

If you are having trouble with your environment, here are three solutions:

 1. Using your current environment, make sure that `PyTorch` and `transformers` are set the the appropriate versions
  2. With the appropriate `pip install`s, use an IDE like Colab to run the code
  3. Create a conda environment using the appropriate .yml file

We discuss this 3rd option in more detail immediately below.

### Environment Creation from a YAML file

Depending on the machine that you are working on, run this code:

`conda env create -f environment_ds10_[ADD THIS].yml`

in your terminal/prompt after activating `conda`.

*  `Conda` [documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) can be found here
    * Scoll down to "Creating an environment from an environment.yml file"
*  When running the above environment creation code, make sure you are in the same location as the downloaded YAML file

*Make sure to replace `[ADD THIS]` with the appropriate ending for the file depending on whether you have a PC, `win`, Mac with M silicon chip, `silicon`, or Mac with Intel chip, `intel`.*

### Words of caution

Due to the dynamic nature of updates to not only PCs and Macs but also to `conda` and the packages/libraries themselves, the .yml files (for Mac Silicon and PC Windows) will inevitably need to be updated.

#### Regarding Macintosh Computers with the Intel chip

As of `PyTorch` 2.3.0, official pre-built binaries for macOSX x86_64 (Intel) has been deprecated, which means that using PyTorch and related libraries with an Intel chip is going to become more and more difficult to run correctly. As such, while the current YAML file for Macs with Intel chips works (with warnings), it will not be updated in the future due to `PyTorch`'s deprecation.

