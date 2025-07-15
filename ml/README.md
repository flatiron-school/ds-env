### Conda Environment Creation from a YAML file

Depending on the machine that you are working on, run this code:

`conda env create -f ml-env_[suffix].yml`

in your terminal/prompt after activating `conda`.

*  `Conda` [documentation](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) can be found here
    * Scoll down to "Creating an environment from an environment.yml file"
*  When running the above environment creation code, make sure you are in the same location as the downloaded YAML file

*Make sure to replace `[suffix]` with the appropriate ending for the file depending on whether you have a PC, `win`, Mac with M silicon chip, `mac-silicon`, or Mac with Intel chip, `mac-intel`.*
